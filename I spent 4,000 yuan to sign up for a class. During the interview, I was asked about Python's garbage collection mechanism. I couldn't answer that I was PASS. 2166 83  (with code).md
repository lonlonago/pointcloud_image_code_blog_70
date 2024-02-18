Last night, I chatted with a senior fan late in the morning. The young man was asked about Python's garbage collection mechanism during the interview, but he was speechless. In the end, he was unfortunately dropped by PASS... (The article has been approved by fans to post chat records) 

![avatar]( 20210717010954245.jpg) 

Have you ever wondered why we frequently use Python to code and do projects, in fact, we have been producing objects and constantly occupying memory, and we rarely clean Python's memory. In theory, it will one day run out of memory (overflow), but every time you open Python, it is "safe and sound"? Is it really just that your computer has a lot of memory? 

No, a mature software will have its own memory management and garbage collection mechanism, rather than relying solely on hardware to provide absolute support. 

![avatar]( 20210716155802554.jpg) 

  Python also has its garbage collection mechanism, which is also a question that interviewers like to ask during interviews: What is the principle of Python's memory management and garbage collection mechanism? 

Too often we focus too much on the surface and neglect the inside. 

Just like when we drive, if you only know the superficial operations of refueling, turning the key, stepping on the accelerator, braking, and steering, and know nothing about the engine compartment, you are not an old driver. Sooner or later, you will have to spend the night on the main road. 

Today, I will tell you how Python's memory management and garbage collection mechanism work, and learn more about Python to avoid being asked this question next time. 

![avatar]( 75b3ad0da356edc805696b7d5bb10cfc.png) 

In the Python C source code, there is a doubly linked list called refchain. This list is rather awesome because once an object is created in the Python program, it will be added to the refchain list. That is to say, it keeps all the objects. For example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
![avatar]( 4a0c51ae64560dc2304f8ad78f7bdcaa.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

All objects in refchain have a reference counter inside ob_refcnt to hold the current object, as the name implies, the number of times they are referenced, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
The above code indicates that there are two values of 18 and "Zhang San" in memory, and their reference counters are: 1 and 2, respectively. 

![avatar]( 984aa2aa389114625718448259874cd2.png) 

When the value is referenced multiple times, the data will not be created repeatedly in memory, but the reference counter + 1 will be used. When the object is destroyed, the reference counter -1 will be used at the same time. If the reference counter is 0, the object will be removed from the refchain list and destroyed in memory (regardless of special cases such as caching). 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
![avatar]( 161a5f8c1be7d74b2fda15c98d7cad31.png) 

Garbage collection based on reference counters is very convenient and simple, but it still has the problem of circular references, which makes it impossible to collect some data normally, such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
For the above code, it will be found that after performing the del operation, no variables will use the two list objects again, but due to the problem of circular references, their reference counters are not 0, so their status: never used, nor destroyed. If there is too much of this code in the project, it will cause the memory to be consumed until the memory is exhausted and the program crashes. 

In order to solve the problem of circular references, markup removal technology is introduced to handle objects that may have circular references. Types that may have circular applications include lists, tuples, dictionaries, collections, custom classes, and other types that can be nested with data. 

![avatar]( 8f64f7ca98c7f63ecdf3d91685a53b95.png) 

Mark clearing: Create a special linked list specifically for storing objects such as lists, tuples, dictionaries, collections, custom classes, etc. Then check whether the objects in this linked list have circular references, and if so, let the reference counters of both parties be -1. 

Generational collection: the mark in the linked list to optimize the removal of those objects may be a circular reference is split into three linked list, linked list is called: 0/1/2 three generations, each generation can store objects and threshold value, when the threshold value is reached, it will do a scan for each object in the corresponding linked list, except for the circular reference each subtract 1 and destroy the reference counter is 0 of the object. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
Special attention: the significance of threshold and count for generation 0 and generation 1 and 2 is different. 

According to the C language and the underlying diagram to explain the detailed process of memory management and garbage collection. 

Step 1: When the object age = 19 is created, the object is added to the refchain list. 

![avatar]( 2670f27782c4ed5349fe30c245777cdf.png) 

Step 2: When the object num_list = [11, 22] is created, the list object is added to the refchain and generations 0. 

![avatar]( 7df2e061eb58293ba1d5ad9442f96b29.png) 

Step 3: When the newly created object makes the number of objects on the 0-generation linked list of generations greater than the threshold 700, the objects on the linked list should be scanned and checked 

When generation 0 is greater than the threshold, the bottom layer does not directly scan generation 0, but first determines whether 2 and 1 also exceed the threshold 

When scanning the spliced linked list, it is mainly to remove circular references and destroy garbage. The detailed process is as follows: 

At this point, the process of garbage collection comes to an end. 

![avatar]( db22db316a478d1d37dc74e0d0d046f4.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

From the above, we can understand that when the reference counter of the object is 0, it will be destroyed and the memory will be freed. In fact, it is not so simple and crude, because repeated creation and destruction will make the execution efficiency of the program low. 

Python introduced a "caching mechanism". 

For example, when the reference counter is 0, the object is not actually destroyed, but it is placed in a linked list called free_list. When the object is created later, it will not be re-opened in memory, but will be used in the free_list. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
![avatar]( 0735b5cbe5441eb3b4c6859aeb41e0e6.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596229
 ```  
The above is Python's memory management and garbage collection mechanism. Although an interview is not a question that can comment on the whole person, if you ask a few more questions that you don't know, it is very likely that you will fail. 

Regarding Python's memory management and garbage collection mechanism, don't you guys understand? Is this car fast? 

![avatar]( 81c3acd990dabf83bb2097ecd4f7bdae.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( 20210715192030488.png) 

