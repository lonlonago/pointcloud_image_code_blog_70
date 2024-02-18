##  Python basics (a full set of nanny-level tutorials) 

###  Chapter IV 

Closure: Essentially, an inner function uses local variables of an outer function. In this case, the inner function is called a closure function 

![avatar]( aeab558bc22e4aa3819392ca93d5e109.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957451762
 ```  
Summary: 1. Can make a variable resident in memory 2. Can avoid global variables being modified 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter IV 

![avatar]( 9a4dfd49a7a24a8ba97c3415e57cff7c.png) 

 Content review: 1. Functions can be passed as parameters 2. Functions can be returned as return values 3. Function names can be assigned as variables 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574569150
 ```  
![avatar]( 3040fb95cff046789f3ee9f6bac79c5f.png) 

 The push-to-process of the decorator  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574569150
 ```  
Summarize: 

Decorator: - > Required to remember the final conclusion, the decorator is essentially a closure, function: without changing the original function call. Add new functions to the function. Straightforward: You can add new functions before and after the function, but do not change the original code 

Where the user logs in, log. How to write the universal decorator: def wrapper (fn): wrapper: decorator, fn: objective function def inner (* args, ** kwargs): #before the objective function is executed... ret = fn (* args, ** kwargs) #Execute the objective function #After the objective function is executed... return ret return inner Never add () ** 

###  Remember the conclusion, the process doesn't matter, it depends on personal interests... 

** 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter IV 

Parameter issues for functions with decorators: *, ** args, kwages, see the code for details and see the conclusion. 

![avatar]( bb7ee49559194bc7af5938787ce4228c.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957456226
 ```  
![avatar]( 9427805fc0764157b2c49ab7ede50f5a.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957456226
 ```  
Summary: The meaning of the parameters before and after is different. The inner * args in front, ** kwargs in the back mean that all parameters are received, packaged into tuples and dictionaries, and the game * args in the back, ** kwargs means that the args tuple and kwargs dictionary are broken up, and the positional parameters and keyword parameters are passed in. Inner adds parameters, args must be a tuple, kwargs must be a dictionary 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter IV 

The return value of the decorator: 

A function can be decorated by multiple decorators. @wrapper1 @wrapper2 def target (): print ('I am the target') 

![avatar]( 258401f2e6c34e488cb544a638ad69a6.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555340
 ```  
Summary: Here is wrapper1 entering, here is wrapper2 entering, I am the target, here is wrapper2 going out, here is wrapper1 going out, rules and laws wrapper1 wrapper2 TARGET wrapper2 wrapper1 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter IV 

![avatar]( 70c56479b9434e86870c449708142e89.png) 

 Log in to the account, add employee information...  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574518305
 ```  
Get familiar with it slowly, I don't know much about normal, remember first, how to use the decorator!! Summary: Knowledge points of decorators, content review: 1. Functions can be passed as parameters 2. Functions can be returned as return values 3. Function names can be assigned as variables 

Decorator: - > Required to remember the final conclusion, the decorator is essentially a closure, function: without changing the original function call. Add new functions to the function. Straightforward: You can add new functions before and after the function, but do not change the original code 

In the place where the user logs in, log. How to write the universal decorator: def wrapper (fn): wrapper: decorator, fn: objective function def inner (* args, ** kwargs): #Before the objective function is executed... ret = fn (* args, ** kwargs) #Execute the objective function #After the objective function is executed... return ret return inner Do not add () 

@Wrapper def target (): pass target () # => inner () A function can be decorated by multiple decorators. @wrapper1 @wrapper2 def target (): print ('I am the target') 

Rules and regularities wrapper1 wrapper2 TARGET wrapper2 wrapper1 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter II 

![avatar]( d329fc6b045c4d1f961a24aed8a51b90.png) 

 Strip () removes whitespace at the left and right ends of the string (spaces,\ t,\ n)  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574561163
 ```  
Strip () is very important. The following is the case of removing the left and right spaces when logging in to the account as follows 

![avatar]( 6623cf0981914431a2fdb73c9736b739.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574561163
 ```  
![avatar]( 4aebb4850ca74d75a242bfba6c06f461.png) 

 Replace (old, new) string Replace, remove all spaces  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574561163
 ```  
Split (what to cut) string cut, what to cut, who will lose. 

![avatar]( 008816f88ccb44c98e8d72e543dee5f3.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574561163
 ```  
Summary: strip () can remove the whitespace (spaces,\ t,\ n) replace () string at the left and right ends of the string, it can also remove all whitespace split () to cut the string, split (what to cut) string cutting, what to cut, will lose who. 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter II 

![avatar]( 9ebba0982faf453cb07b9d40947034f5.png) 

 Join () concatenates the contents of a list into a new string  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563534
 ```  


--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter II 

![avatar]( 0fe1888198be4e7da189572dcc59c974.png) 

 List addition, deletion, modification (*) addition: add content to the list 1.append () append (*) 2.insert () insert 3.extend () can merge two lists and add in batches  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553535
 ```  
![avatar]( 2cfc25ebe8a643608a2407bdd89541f4.png) 

 Delete: pop gives the deleted index. Returns the deleted element remove removes an element (*)  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553535
 ```  
![avatar]( 273b5a43924c49abbdc91a9cc41131c9.png) 

 Modify: You can modify the operation directly with the index  

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553535
 ```  
Query: directly use the index for query operations 

![avatar]( 539d96700e8b494cb504237d20521f12.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553535
 ```  
Summary: 1. append () append () 2. insert () insert 3. extend () can merge two lists, add in batches 4. pop gives the deleted index. Return the deleted elements 5. remove delete an element () 6. directly use the index to modify the operation 7. Directly use the index to query the operation, practice, do one, change all the people with the surname Zhang to the surname Wang lst = ['Zhao Min', 'Zhang Shaogang', 'Zhang Wuji', 'Wu Zetian', 'Ying Zheng', 'Ma Chao'] 



--------------------------------------------------------------------------------

##  Python basics (a full set of nanny-level tutorials) 

###  Chapter II 

Encoding and decoding 1. str.encode ("encode") to encode 2. bytes.decode ("encode") to decode gbk and utf-8 cannot be directly converted. Our military codebook - > text - > enemy codebook 

![avatar]( 0fb3058a12ae4a1588ee92bba54e76b6.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574527308
 ```  


--------------------------------------------------------------------------------

###  foreword 

Over the years, I have maintained a habit of organizing my knowledge and making notes. Although we search for a lot of information online, we can find a large number of them, and then collect them if we think they are good, such as some good blogs. When I think about using them, I will read them again. 

But in this process, there will be problems often encountered, such as the collection of articles is missing (deleted), and then to find other articles and have to re-understand the new author's thinking; for example, although I have collected some articles, but some of the articles in the partial content will be outdated, tasteless and discarded, if you can modify it, it would be nice, but unfortunately not the author. 

![avatar]( f6316fa41255433cad61525d1e249463.jpg) 

So later, I went to organize my own information, constantly updating and making notes, such as some syntax or other commands, etc. Although the process was a bit troublesome, when I needed to check the information, I directly opened the file and searched for keywords to quickly find them. At the same time, I also saw some of my own remarks. Basically, I could use them immediately after seeing them. 

Today, I would like to share with you the commonly used functions of MySQL in my database, which basically includes the functions I usually use. They have been with me for many years, coming and going in the wind and rain, and sewing and mending for several years. 

![avatar]( dc372dfac1464252bd92df628b7c9a16.jpg) 

In order to make them more concise and clear to everyone, I have done a lot of work on the old documents, removing a lot of things that only I can understand, and trying to restore something that everyone can understand. 

At the end of the article, I will also attach my own source files, which can be flexibly modified and annotated on the basis of the files to form my own data notes. 

### 

article directory

Introduction @[toc] 1. Flow control function 2. Aggregation function 3. Encryption function 4. Date function 5. Numeric function 6. String function 7. Other function source files

###  First, the process control function 

Example: IF (test, v1, v2) returns the result v1 if the expression expr holds; otherwise, returns the result v2 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
###  Aggregate function 

Example: SUM (expression) returns the sum of the specified fields 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  III. Encryption function 

Example 1: Implementing the ENCODE function on a string. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
###  IV. Date function 

Example: DAYNAME (d) returns the day of the week, such as Monday, Tuesday 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Number function 

Example: CEIL (x)/CEILING (x) returns the smallest integer greater than or equal to x 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  The string function 

Example: INSERT (s1, x, len, s2) string s2 replaces the string of length len starting at the x position of s1 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
###  VII. Other functions 

Example: CONV (x, f1, f2) returns f1 to f2 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
Result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566394
 ```  
###  source file 

The following is the source file, which can be picked up by yourself for everyone to play freely. If you don't like it, don't spray it, and seek common ground while reserving differences. 

Link: https://pan.baidu.com/s/1QseiLFanbTsBjQflbxJWag Extraction code: w7el 

Writing is not easy, if you can help, I am grateful! 

![avatar]( 660cb9f496cf4dbca6196b988d03c201.png) 



--------------------------------------------------------------------------------

First of all, this article does not have marketing, nor does it advertise training institutions, purely celebrating their breakthrough 20,000 fans, pet powder, things can be used in vain. 

I have been preparing for this matter for a long time, I have always wanted to give my fans a free and valuable gift when my CSDN fans break through 10,000 fans, but this gift is not easy to take, has been negotiating, fans came to 20,000 powder, this time must be given! 

![avatar]( 20210610121322172.png) 

Let me be blunt. The fan benefit prepared for you this time is the 130-session Python introductory + crawler + data analytics course. Note that it is 130 sessions! Not a dozen sessions of fooling people. 

And it's free to use! 

If you can complete it, you will not only have a solid foundation in Python, but also have the skills of crawlers and data analytics, which are two of the most popular skills. 

![avatar]( 20210610130652737.png) 

 The following is the syllabus of the course:  

###  First, this thing is not easy to come by 

I don't have time to specifically record classes for fans, and I haven't recorded them, nor do I have the energy to do them. I have the same idea as many of you. I want to use it for nothing, but I have to avoid copyright issues. 

I negotiated with eight third-party organizations, some directly refused, some asked for my price, and sure enough, there is no free lunch in the world... In the end, I found real-world friends to get in touch, and I got these 130 courses, which can be provided without copyright. 

###  Second, what is the value of this item? 

Since it is used for nothing, is it worthless in itself? 

I can say with certainty that this thing is free to use for the first time on the whole network. Those who spend money may already have these courses, but those who don't spend money definitely don't. 

130 main lessons, with theories and projects in practice, definitely not the kind of things that fool people like more than a dozen lessons, and I don't bother to say that I use these things to tease my fans. If you can learn it, you will have a solid foundation in Python, crawler skills, and data analytics. Of course, it doesn't mean that you have fully mastered crawlers and data analytics after learning these things, but at least crawlers no longer ask for people, multi-threading, anti-picking, etc. The matplotlib, numpy, and pandas commonly used in data analytics are also covered. 

After all, this is for nothing. When you have the ability in the future, you can advance more and learn other things easily. 

![avatar]( 20210610134016361.jpg) 

 If you don't get it this time, you can only wait for the next time I have 100,000 fans, and then I will definitely give you a bigger gift for free use.  

###  III. How to use it for nothing? 

I originally wanted to give the link directly for everyone to use in vain, but I thought it was inappropriate. The link is easy to be F, and after giving it like this, maybe some unruly blogger will take this and send it everywhere. Therefore, if you want to take this thing, please do 2 more operations. 

The first step is to leave a message. 

Leave a message under the comment area of my article "I am an Uncle Long fan, thank you for sharing", and then take a screenshot to prove that you are a fan, not an advertisement. 

Step 2: Find my assistant. 

There are too many things to do these days, so I can't be busy, so I hired a part-time assistant. You can directly ask her for this welfare course, and show her a screenshot of your message to prove that you are a fan. 

QQ：3163194867 

Alternate QQ: 2590434047 

The participation time ends at 24:00 on June 18th. There are too many people to receive, and my assistant is a little busy, but if you add friends before June 18th, you will finally agree. 

###  IV. Looking back and looking forward 

Since I started writing articles in April, I have received a lot of feedback from fans one after another, met a lot of people, and even caught up with one-third of the people I have known for more than ten years. During the interaction, I felt a lot of emotion. There are friends who are still discussing with each other at two or three o'clock in the middle of the night, aspiring young people who study while working, and college students who are at a loss, etc., which reminds me of a lot of my past experiences and makes me re-examine myself. Originally, writing articles on CSDN and other platforms was just a pastime, but now I have to reposition and plan myself. I hope that in the future, I can write more good articles and give every person who trusts me the help they can. 

![avatar]( 20210610134132324.png) 



--------------------------------------------------------------------------------

As a practical tool for dealing with strings, regular expressions are often used in Python, such as crawlers Crawling the data to retrieve strings and so on. Regular expressions are already embedded in Python and can be used by importing the re module. As newbies to Python, most of them have heard of the term "regular". 

Today, I would like to share with you a more detailed collection of Python regular expressions. After learning it, you will become proficient in regular expressions. 

![avatar]( 85fe1001262f476eae84421661e56e6d.jpeg) 

###  The re-module 

Before we talk about regular expressions, we must first know where to use regular expressions. Regular expressions are used in the findall () method, and most string retrievals can be done through findall (). 

1. Import the re module. Before using the regular expression, you need to import the re module. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
2. the syntax of findall (): 

After importing the re module, you can use the findall () method, so we must be clear about the syntax of findall (). 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
It is not difficult to see that findall () is composed of a regular expression and a target string. The target string is what you want to retrieve, so how to retrieve it is performed through a regular expression, which is our focus today. 

The result returned after using findall () is a list of strings that meet the regularization requirements 

###  Second, regular expressions 

Most letters and characters can match themselves. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Metacharacters refer to special characters such as .^ $ ?+ {} \ [], through which we can personalize the search of the target string and return the result we want. 

Here I will introduce to you 10 commonly used metacharacters and their usage. Here I will give you a simple summary for easy memorization. The following will explain the use of each metacharacter one by one. 

![avatar]( 8c37aa9d37e14e9880b384e5b85721e3.png) 

（1） [] 

[] 的使用方式主要有以下三种： 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
For example, to select the abc element in the string "abcabcaccaac": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
For example, to select "caa" in the string "caabcabcaabc": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Note: When in the first position of [], it means that everything except a is matched, such as changing the position of a in []: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
（2）^ 

^ is usually used to match the beginning of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
![avatar]( 724785f6d8f5422e8c52eaef8b552226.jpg) 

(3) $$is usually used to match the end of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
![avatar]( 8ca641e45b994987a9a23ba070981eee.jpg) 

（4）\ 

After the backslash, different characters can be added to represent different special meanings. Common ones include the following three. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
\ can be escaped into normal characters, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Match any whitespace characters such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Matches any alphanumeric and underscore, equivalent to [a-zA-Z0- 9_], for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
![avatar]( 1e9ee27672ed489dafb11d1c71a02a02.jpg) 

（5）{n} 

{N} can avoid repeated writing. For example, we wrote\ w 3 times when we used\ w earlier, but here we need to use {n}. N represents the number of matches, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
（6）* 

* Means zero or more matches (as many as possible), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
**（7） + ** 

+ means match one or more times, e.g. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
（8） . 

. is a dot, which is not obvious here. It is used to manipulate any character other than a newline character, such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
(9) ？ 

? means one match or zero 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Pay attention to greedy and non-greedy patterns here. 

Greedy pattern: Match as much data as possible, expressed as\ d followed by a metacharacter, such as\ d *: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Non-greedy mode: Match as little data as possible, expressed as\ d followed by?, such as\ d? 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
(10) {m, n} m, n refers to a decimal number that is repeated at least m times and at most n times, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Add? means to match as little as possible 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
There are other flexible ways to write {m, n}, such as: 

![avatar]( 14d7db206f8943418d2a43026521c828.jpg) 

Regarding the commonly used metacharacters and how to use them, let's take a look at the other knowledge of regular rules. 

###  (2) The use of regular rules 

In Python, the re module can compile regulars through the compile () method, re.compile (regular expression), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The use of regular objects is not only through the findall () method we introduced earlier, but also through other methods. The effect is different. Here is a simple summary: 

(1) findall () finds all strings that re match and returns a list 

(2) search () scans the string to find the position where the re matches (just the first one found) 

(3) match () determines whether re is at the beginning of the string (matches the beginning of the line) 

Let's take the example of the object returned by compile () after compiling the regular. Instead of findall (), let's use match () to see how the result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
It can be seen that the result is a match object, the starting subscript position is 0~ 13, and the match is 010-123456789. Since the object is returned, let's talk about some operation methods of this match object. 

![avatar]( 511fa5bb3d9e404398729084f797a7d6.jpg) 

Here are the methods first, and I will give examples later. Common methods of using Match objects are as follows: 

(1) group () returns the re-matched string 

(2) start () returns the starting position of the match 

(3) end () returns the position where the match ends 

(4) span () returns the position of a tuple: (start, end) 

Example: Use span () to operate on the object returned by search (): 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
The result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
In addition to the findall () function introduced above, there are other functions in the re module to provide an introduction: 

(1) findall () returns all the strings that match according to the regular expression. I won't say much about this. I have introduced it earlier. 

(2) sub (regular, new string, original string) The function of sub () is to replace the string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
(3) subn (regular, new string, original string) The function of subn () is to replace the string and return the number of replacements 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
(4) split () split () split string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535490
 ```  
![avatar]( 1b31fa941d2944b8a9131f06c72a5cd8.jpg) 

###  III. Conclusion 

Regarding regularity, I have said so much. Regularity is an indispensable foundation in almost all directions of Python. I wish you all the best in your Python journey! 

Thank you for reading and liking. I have collected a lot of technical dry goods that can be shared with friends who like my articles. If you are willing to take the time to study, they will definitely help you. The dry goods include: 

![avatar]( 17baf34c84e4483f9f9b3d9bb3341c44.png) 

![avatar]( 521e60d8459b40f2bd654b1a410926db.png) 

 Click on the business card at the end of the article to take it away.  



--------------------------------------------------------------------------------

###  foreword 

Crawling is a very interesting technology. You can use crawling technology to obtain things that others can't get or need to pay to get. You can also automatically crawl and save large amounts of data, reducing time and effort to do some tiring work manually. 

It can be said that many people learn programming, and it is indeed a lot less interesting to not play with crawlers. Whether it is amateur, private work or professional crawlers, the crawler world is indeed quite exciting. 

Today, I will give you a brief talk about reptiles, with the aim of enabling friends who are ready to learn reptiles or who are just starting out to have a deeper and more comprehensive understanding of reptiles. 

![avatar]( 91d7d6f79869466bb4723831776f29de.jpg) 

###  First, get to know reptiles 

Let me introduce you to the famous crawler in one sentence: an automated program that requests websites and extracts data. 

Let's take it apart and understand the reptile: 

To request a website means to send a request to the website, such as going to Baidu to search for the keyword "Python", at this time our browser will send a request to the website; 

Extracting data, including pictures, text, videos, etc., is called data. After we send the request, the website will present the search results to us, which is actually returning the data. At this time, we can extract the data. 

The automated program, that is, the code we wrote, realizes the automatic extraction process data, such as downloading and saving the returned pictures in batches, replacing us with manual operations one by one. 

![avatar]( 9cebb87320ed46d68878f11d1ba63761.jpg) 

According to the usage scenario, crawlers can be divided into three categories: 

General-purpose crawlers (large and comprehensive) have powerful functions and a wide range of collection surfaces, and are usually used in search engines. For example, Baidu Browser is a large crawler program. 

Focused crawlers (small and precise) have relatively simple functions, only crawling specific content for specific websites, such as going to a website to obtain certain data in batches, which is also the most commonly used crawler for us personally. 

③ Incremental crawler (only collects updated content) This is actually an iterative crawler that focuses on crawlers. It only collects updated data and does not collect old data. It is equivalent to always existing and running. As long as there is data that meets the requirements, it will automatically crawl new data. 

![avatar]( d09e742346404877922be58300d02665.jpg) 

There is a protocol called Robots that needs to be paid attention to in crawlers, also known as "web crawler exclusion standards". Its function is to tell you what can and cannot be crawled by websites. 

In general, you can directly add/robots.txt after the homepage URL of the website to view, such as Baidu's Robots protocol https://www.baidu.com/robots.txt, you can see that there are many URLs that cannot be crawled, such as Disallow:/shifen/indicating that the current Disallow:/shifen and Disallow:/shifen subdirectory pages below cannot be crawled. 

![avatar]( dcd3d7b7153c41d18f622ee6d79941c2.png) 

  In fact, this Robots agreement belongs to a gentleman's agreement. For crawlers, it is basically a verbal agreement. If you violate it, you may be held legally responsible, but if you do not violate it, crawlers will not be able to crawl any data. Therefore, both parties usually turn a blind eye and don't be too arrogant. 

![avatar]( afda73d38b7d4f7dab59982cd0716d40.jpg) 

###  Second, the basic process of crawlers 

How do crawlers work? A crawler program can be roughly divided into four steps: 

① Initiate a request, make a request to the target site through the HTTP library, that is, send a Request, the request can contain additional headers and other information, and wait for the server to respond. 

② Get the response content. If the server can respond normally, it will get a Response. The content of the Response is the page content to be obtained, and the types may include HTML, Json string, and binary data (such as images and videos). 

③ Parse the content, the resulting content may be HTML, which can be parsed with regular expressions and web page parsing libraries. It may be Json, which can be directly converted to Json object parsing, and may be binary data, which can be saved or further processed. 

④ Save data, there are many styles of saved data, which can be saved as text, saved to a database, or saved as a file in a specific format. 

So that's basically the four steps that a crawler has to follow. 

Request and Response are the most important parts of a crawler. What is the relationship between Request and Response? The relationship between the two is as follows: 

![avatar]( 3eac43fa1c8642539c38020a54516f85.jpg) 

  To put it simply, when we search for something on the computer's browser, such as the aforementioned search for "Python" on Baidu, you click on Baidu and send a Request request to Baidu's server. Request contains a lot of information, such as identity information, request information, etc. After the server receives the request, it makes a judgment and then returns a Response to our computer, which also contains a lot of information, such as whether the request was successful or not, such as the information results we requested (text, pictures, videos, etc.). 

This should be easy to understand, right? Next, let's take a closer look at Request and Response. 

###  III. Understanding the Request 

What does Request contain? It mainly includes the following things: 

The request method can be understood as the way you greet a website. If you want to get data from a website, you have to greet it in the correct way so that it can care about you. Just like if you want to borrow something from someone's house, you have to knock on the door first. Hello, you can directly climb the window and enter. Anyone who sees it has to be kicked out. 

![avatar]( bf7bf87ba69f4633aea4f614a96ea043.gif) 

The main request methods include GET and POST, as well as HEAD/PUT/DELETE/OPTIONS and other methods. The most commonly used request method is GET. 

>  I have hidden a lot of technical dry goods and moved them to the CSDN community to pick them up by myself. 

What is a URL? The full name of a URL is Uniform Resource Locator. For example, a web page document, picture, video, etc. has a unique URL. In crawlers, we can understand it as a URL or a link. 

What is a request header? The English name Request Headers usually refers to the header information contained in the request, such as User-Agent, Host, Cookies, and so on. 

These things are equivalent to your identity information when you send a request to a website. It is often necessary to disguise yourself as an ordinary user to prevent your target website from recognizing that you are a crawler, avoid some anti-theft problems, and obtain data smoothly. 

The official version is the additional data carried in the request, such as the form data when the form is submitted. 

How to understand? For example, if you go to your father-in-law's house to propose marriage, you can't go there empty-handed to propose marriage, right? You have to bring something to make it look like a proposal, and your father-in-law will betroth your daughter to you. This is a common etiquette and is indispensable. 

![avatar]( 0d9b1f08eb1144fd9f2cd48182b82e17.jpg) 

For example, on certain pages, you have to log in first or you have to tell me what you are requesting. For example, if you search for "Python" on Baidu's webpage, then the keyword "Python" is the request body you want to carry. Only when you see your request body will Baidu know what you want to do. 

Of course, the request body is usually used in the POST request method. In the GET request, we usually splice it in the URL. Here, you can understand it first, and subsequent specific crawlers can deepen their understanding. 

Since we have already talked about the theory of Request, we can go to practice to see where the Request is and what it contains. 

Take Google Chrome Chrome as an example, I enter the keyword "Python" to search for a bunch of results, let's use the console window that comes with the web page to analyze the Request request we sent. 

Press and hold F12 or right-click "Check" in the blank space of the webpage, and then you can see that there are many options in the console. For example, there is a menu bar in the upper column. For primary crawlers, we usually use Elements (elements) and Network (networks) more commonly. Other things are temporarily unavailable. When you learn advanced crawlers, you will use them. For example, when JS is reversed, you may use the Application window. Later, you will learn more about it. 

Elements contains every element of all request results, such as the source code for each image, especially when you click the small arrow in the upper left corner, every place you move to will be displayed under the Elements window. 

![avatar]( aa615005ebc54e7b94cb03291946e34b.png) 

Network is the network information commonly used by crawlers, including our Request. Let's take a look. Under the Network window, check Disable cache and click All. 

![avatar]( 72f22cca45314a1980f52bbc7e14eae3.png) 

Refresh the webpage to see the effect. It can be seen that we sent 132 Request requests. There is no need to be curious about this. Although we only sent a "Python" request to Baidu, some of them were requests attached to the webpage. 

![avatar]( b996faab01814662b6ea45e068af0d32.png) 

Although there are many types, such as png, jpeg, and so on, you can swipe to the top. In the Type column, there is a document type, which means web document. Click to enter and get our Request information. 

![avatar]( 1880f8417100403bb627892cd4db8d16.png) 

After clicking on document to enter, there is a new menu bar. Under the Headers column, we can see the Request URL, which is the request URL we mentioned earlier. This URL is the URL we actually request from the webpage. Then there is the request method, which can be seen as the GET request method. 

![avatar]( 5f766040932f42eab333809e9863d0c2.png) 

Swipe down again, and you can also see the Request Headers we talked about earlier. There is a lot of information, but the User-Agent, Host, and Cookies we talked about earlier are all available. These are the information we give to the server. 

![avatar]( 9153afba20f24b0cbb2e0569478e3bd9.png) 

Although there is a lot of content in Request Headers, we also need to do camouflage work in this regard when writing a crawler program, but not all the information we have to write, just write some important information selectively, such as User-Agent must bring, Referer and Host are selective zones, cookies will be brought in the case of login, and there are only 4 commonly used items to be camouflaged. 

As for the request body, I will not check it for the time being, because our request method here is a GET request, and the request body can only be viewed in the POST request. It doesn't matter. You will naturally understand when the crawler uses it. 

###  IV. Understanding the Response 

Response mainly includes three pieces of content, let's take a look at them one by one. 

After we send a request, the website will return us a Response, which includes the response status code. The response status can be roughly divided into the following categories: 

① A range of 200, such as a response status code of 200, indicates success. 

② 300 range, such as 301 indicates a jump. 

③ 400 range, such as 404 can not find the page. 

④ 500 range, such as 502 can not find the page. 

For crawlers, two or three hundred is the response state we most want to see, and it is possible to get data. Four or five hundred is basically cold and can't get data. 

For example, when we just sent the previous Request request, in the document file, we can see that the response status code is 200 in the General under the Headers window, indicating that the webpage successfully responded to our request. 

![avatar]( 1ebac61f45244a4d823831c8ec222d57.png) 

The information the server gives us will also contain a response header, which includes content type, content length, server information, and setting cookies, among others. 

In fact, the response head is not that important to us. Let's take a look here. 

This is very important, in addition to the response state of the first point, because it contains the content of the requested resource, such as web page HTML and image binary numbers, etc. 

Where is the response body? It is also in the Response column in the document file. You can swipe down to see that there is a lot of response data in it. This is the data we have obtained. Some can be downloaded directly, while others require technical analysis to obtain. 

![avatar]( b7069ed3bbcf4736bd6153b6e3a0f81b.png) 

###  What kind of data can crawlers obtain? 

What kind of data can crawlers obtain? Basically, it can be divided into the following categories: 

Web documents, such as HTML documents, Json format text, etc. 

② Picture, what you get is a binary file, just save it in picture format. 

③ Video, which is also a binary file, can be saved as a video format. 

④ Others, anyway, other things that can be seen can theoretically be obtained by crawlers, depending on the difficulty. 

###  How to parse the data? 

After the request is successfully sent, the webpage will return a lot of data to us, including thousands or even tens of thousands of codes. How can we find the data we want in so many codes? Common methods include the following: 

① Direct processing. When the data returned by the webpage is some text, which is the content we want. There is no need for filtering processing, just process it directly. 

② Json parsing. If the webpage returns not HTML data but Json data, then Json parsing technology is required. 

③ Regular expression. If the returned data is data that conforms to the regular expression, you can use the regular to parse. 

④ Other parsing methods. Commonly used are XPath, BeautifulSoup, and PyQuery, which are commonly used parsing libraries by crawlers. 

###  How to save the data? 

After obtaining the data, there are several commonly used methods for saving the data: 

① Text. Can be directly saved as plain text, EXCEL, Json, Xml and other types of text. 

② Relational database. Data can be saved to relational databases such as MySQL and Oracle. 

③ NoSQL database. Such as MongoDB, Readis and Key-Value storage. 

④ Binary files. Such as pictures, videos, audio, etc. can be directly saved to a specific format. 

Regarding crawlers, let's talk about it here today. Welcome to leave a message in the comment area below. 

>  I have hidden a lot of technical dry goods and moved them to the CSDN community to pick them up by myself. 

![avatar]( a2bbaba094b240c2b896d3d781a2e0a3.png) 



--------------------------------------------------------------------------------

Do you know a few parsing libraries or a little bit of framework knowledge to become a crawler? No, in fact, a qualified crawler is not as simple as he thinks. It takes time and technology to precipitate and constantly polish programming skills. 

So today I'm going to tell you "What skills do you need to learn to go from beginner to qualified reptilian. 

![avatar]( 3d6b3b563f2e4025899f7fc8d086e9a3.png) 

###  First, the Python language 

Any programming technology requires language support. Among the many computer programming languages, it is not said that only Python can be used for crawling, it is not the only one, such as Java, C, etc. These can be used for crawling development, but in contrast, Python is the most suitable for crawling development. 

The Python language is the foundation, and if you have a solid grasp of the basic knowledge, there will be no problem in the later learning. Then one of the more important knowledge points at this stage is "object-oriented programming thinking", which is the most difficult thing. Therefore, students can spend more time on this stage of the Python language, and they must have programming thinking, so that the following things can get twice the result with half the effort. 

![avatar]( 8246471217d34102b3b1da11965ed676.png) 

###  Programming Linux environment 

Linux has always been a leader in the server field, which is largely due to its stability, security and low total cost of ownership, and whether it is a web project in the enterprise, or a database, and the deployment of crawlers, not to mention big data processing, and even artificial intelligence, the vast majority of them run in Linux system, so lay a good Linux foundation is a must-have skill. 

We can Linux, familiar with the relevant common commands, such as learning how to configure Linux system network, common basic commands, or skilled administrators of Linux systems, after all, we are to do professional crawlers, not operation and maintenance. 

![avatar]( d7b43311e82b479ba168c62611aa8329.png) 

###  III. Database programming 

All projects rely on databases, which are essential skills for programmers, such as MySQL, PostgreSQL, SQL Server, etc. However, the most widely used database is MySQL. 

But no matter what kind of database you learn, whether it is MySQL or SQLserver, SQL language is something we must firmly grasp, such as the most basic addition, deletion, modification, and search of databases, as well as the design ideas and three paradigms of databases (1NF~ 3NF). 

![avatar]( 2b200429d01ced4c2e2fe9bc74bb5513.png) 

###  IV. Web programming 

Nowadays, we are familiar with the B/S architecture and the C/S architecture. These two architectures vary widely in terms of hardware environment, security requirements, program architecture, and processing issues. The current browser implementation shows that most of them are based on the B/C architecture. At the same time, web programming is also a skill that every programmer must understand. 

For a crawler, we don't need to say that we want to be as proficient as a front-end programmer, but we also need to be familiar with this part. 

![avatar]( 6856ecb100b8c109c746fcdd1257219b.png) 

###  Django Web Framework 

We all know that Django is a Python-based web development framework. So first of all, we need to specify what web development is. Web development refers to the development of applications based on B/S architecture that display the data of the back-end server to the front-end user through the cooperation of the front-end and back-end. 

Django is an open-source web framework written in Python with full web capabilities. With Django, you can easily complete most of the content required for a website with very little code, and further develop a fully functional web service. 

![avatar]( 312fc6755bf4a808ab66a1d070edddf7.png) 

###  Tornado programming framework 

Tornado is the open source version of our web server and its common tools at FriendFeed. Tornado and the current mainstream web server frameworks (including most Python frameworks), Tornado is also a commonly used Python web development framework. 

In the process of writing a project, it is common to mix the two frameworks of Django and Torndao, making full use of the convenience and speed of Django and the high load of Tornado to solve practical problems in the project. 

![avatar]( 8070bdb801f4a78289ec88b666e3988d.png) 

###  Seven, mobile end technology 

For a qualified crawler developer, it is not enough to only crawl the data on the web. With the development of the Internet, the data on mobile devices is also of reference value, and the two must be developed in a balanced manner. 

From the basic knowledge of Android, such as what controls Andrond has, as well as network programming and HTTP protocol, six basic principles and common design patterns, etc. 

![avatar]( ac2dd1fd648541e49210a523157e5d24.png) 

###  Eight, reptile development 

In recent years, with the development of big data and artificial intelligence, especially artificial intelligence, there is an increasing demand for crawler engineers. Experienced crawler engineers can easily start at 20k. Postgraduate degrees in artificial intelligence will have great advantages and require further study. 

Speaking of which, we also need to understand the most basic crawler principles and routines, understand the various problems of web crawler programming, deal with anti-crawler technology, be able to deal with dynamic website crawling, be able to deal with websites with verification codes, and so on. 

![avatar]( 331edfe4fcb04cbfa69bec956e07d397.png) 

>  I have hidden a lot of technical dry goods for all fans (click here). 

###  And finally. 

We still have a long way to go on the crawler road. I hope you will persevere and continue to refine your skills, and eventually become a qualified crawler engineer. 

Technology is not guilty, but if you crawl around, you will get caught. 

![avatar]( 20210421162557587.png) 



--------------------------------------------------------------------------------

Learn to program and deal with code. If you don't know how to use GitHub, you may need to reinvent it. Many newbies have not yet realized the power of GitHub. Whether it is learning, setting up, or working, they can find many useful project resources on it. 

But finding projects has always been the most troublesome problem for beginners, especially blind search projects, which is even more difficult. So today, teach you a few GitHub tips to quickly find the project you want. 

![avatar]( 74fc6eb691b0429bbcfd2c3f77a9a8a6.png) 

###  Smooth use of GitHub 

Before we start teaching skills, we will help you solve a common problem: web pages open GitHub and circle around, and even many times they cannot be opened. 

Recommend a free gadget, dev-sidecar, on GitHub. 

First open Gitee's website, then enter "dev-sidecar" to search, and click "docmirror/dev-sidecar", which is a tool that can solve the problem of unsmooth website access. 

![avatar]( afac6f5d507f495e817993f1fc543161.png) 

Find "Download and Install Package" in the menu bar, then click "Gitee Release", and then select the version corresponding to your computer system type to download. After the download is completed, start the installation. 

Once you're done, you'll be able to open GitHub stably, and then we'll start learning some tips for finding projects on GitHub. 

###  Second, GitHub's tips for finding projects 

The difference with blind search projects is that you will use tricks to filter out some items you don't want on GitHub and find what you want directly. 

When searching, you can use keywords to search for relevant content, such as using in: name redis, you can search for projects that contain springboot in the project name. 

![avatar]( b2339fc3382241f89be86f1e1c4e24d2.png) 

For more excellent and popular projects, the number of stars and forks will be higher. Use the keyword to search for redis stars > = 200 to filter out related projects with more stars and forks than the specified value. 

![avatar]( 1bdbeb73b11b4f8095c8abbc13c93a93.png) 

  Obviously, there are not many projects with more than 20,000 stars, only 7. 

When searching blindly, the project you find may be an old project that no one maintains and is in disrepair, so you can add the conditional search of time, such as entering redis pushed: > 2022-01-01 

![avatar]( 46c1c370d4ce46f6a2ba4c8c71d69de9.png) 

The methods mentioned above can also be mixed and used, and multiple qualifications can be added together to find the item you want in a smaller range. Or take redis as an example to find items after January 1, 2021 with more than 2000 stars and redis in the description. You can search like this: 

in:discription redis stars:>2000 pushed:>2022-01-01 

Finally, we can check the language we want, such as Python, and find projects related to Python that meet the above conditions. 

![avatar]( 2a60cf7208124142a1c6d25a4e0eb2f1.png) 

  There are only 15 eligible projects, which is much better than finding a needle in a haystack from hundreds or thousands of projects. 

>  I have hidden a lot of technical dry goods for all fans (click here). 

So today's sharing is here first. If you think it will be helpful to you, please don't hesitate to share it three times! 

![avatar]( 4173ebd33d4e40bbbdcfbd80f73ed390.png) 



--------------------------------------------------------------------------------

###  foreword 

When you first came into contact with HTML, were you surprised by its many tags? In particular, HTNL5 tags have been added a lot, and many HTML4 tags will not be used after cross-version. It is impossible to remember so many tags. We only need some commonly used tags, and the rest can be queried when used. 

![avatar]( 0bcf5ec7eda4477fb1cf539f408b5e1b.jpg) 

![avatar]( dc51e32242e4452ca5b1e36e48c9a7ba.jpg) 

 But sometimes the technical webpages that I collect are often 404. Although you can go to Baidu, you have to look it up line by line. So lazy people like me always want to do it once and for all. I used to organize some things that I might use in my work into document notes and upload them to my online disk and GitHub.  

Today, I will share with you the HTML5 tag notes that I have sorted out before, and provide the source documentation. When you need it, you can Ctrl + F to find keywords, and you can also make your own remarks by the way. 

Without further ado, go directly to the goods! 

###  Media-related labels 

![avatar]( fcceaaf0e27f425399b9f22243a7f8e6.png) 

###  Global attribute related tags 

![avatar]( 0693131420cf45c285d973f0953bd49b.png) 

###  III. Windows-related tags 

![avatar]( aac227adac56498d9a4162d70bed4378.png) 

###  IV. Keyboard and mouse related labels 

![avatar]( 3eb23a33d1d34128a35bf002cf52cf59.png) 

###  Form related labels 

![avatar]( 1c6d2b71f1f743149a5bc1d5a2d9d160.png) 

>  Fan benefits, click to view 

###  Other commonly used labels 

![avatar]( efa64e65a32a41818ceba4dab3cb36e8.png) 

###  HTML4/HTML5 Universal Labels 

![avatar]( 365399b6d4834a718e7b1266819cd877.png) 

###  VIII. Source documents 

The above picture is just for better display in the article. I think it is still the md source file that is really easy to use. Here is the link for you. If you need it, you can pick it up by yourself: 

Link: https://pan.baidu.com/s/1p1FFzn-9HYIXFqRpViWfyA Extraction code: u2o6 

Finally, I wish you all the best in your work and study. If the article is useful to you, I hope you will be grateful! 

![avatar]( 07a6cb514190446bb20fb8ca5f6c8eda.png) 



--------------------------------------------------------------------------------

##  foreword 

Dear friends, hello everyone. Uncle Long, I often receive private messages in the background asking what is Python? Is it necessary to learn this language? Today, I will tell you what Python is and how to learn it through this article? If you are also interested in python, please subscribe to my column. If you think my article is well written, remember to give me a like and support! 

##  What is Python? 

![avatar]( dfeb65aafb424a028c0a0241820c7c07.png) 

Python is an object oriented, interpreted high-level programming language with concise, clear, and easy-to-read syntax, which is widely used in web development, data science, and artificial intelligence. 

Python's design philosophy emphasizes readability and simplicity. Because Python code is particularly readable, it is widely used in many fields because it is very efficient to develop and maintain applications in Python. At the same time, Python also has a large community and excellent third-party libraries and frameworks, which can easily complete the development of various tasks and projects. 

##  Origin of Python 

![avatar]( b48b1d002ffd468fb3cf44a73fd9d9a6.png) 

 When many people hear the word python, the first thing that comes to mind is the python, so why is python called python (python)? We have to ask this boss - Guido van Rossum  

Guido van Rossum created Python in order to solve the problems he faced at the Amsterdam Institute (CWI). At the time, CWI's IT system did not have a development language that could complete various tasks, and various development languages had some limitations and flaws, which annoyed Guido. Therefore, he began to design his own programming language to better solve these problems. During Christmas 1991, he completed the first version of Python and named it after a comedy group called Monty Python from his favorite TV series "Monty Python Flying Circus". After that, he promoted Python within CWI, and it was quickly recognized and used by everyone. Since then, Python has gained popularity and become a globally popular programming language, widely used in web development, data science, artificial intelligence, and many other fields. 

##  Why should we learn Python? 

![avatar]( b431ce64bf514d7e95026f22dbfc7211.png) 

According to the six-month programming language rankings for 2023, it is not difficult to find that, regardless of the changes in the rankings of other languages, Python has always occupied the first place. From these data, we can see the popularity of the Python language. 

So why is Python so popular? It depends on its following advantages: 

>  1. Python is an easy-to-learn language, and its syntax is very concise and clear. For beginners, it is easy to master its basic syntax and programming principles.

2. Python has a strong development community and a wide range of application scenarios, which can be used for data analytics, web development, scientific computing, artificial intelligence, etc., covering a wide range of fields.

3. Python is portable and can be used on various operating systems and platforms, whether it is Windows, Linux or MacOS, etc., you can run Python programs.

4. Python has a wealth of third-party modules and libraries, making it easy for developers to use and use more widely.

5. Python is highly customizable, allowing for more complex and advanced programming tasks through a variety of modules and tools. 

What's more, Python has a wealth of data processing libraries and tools: Python has a wealth of data processing libraries and tools, such as Numpy, Pandas, Matplotlib, Scikit-Learn, etc. These libraries can help developers quickly process, visualize and analyze data. Today, we are in the era of big data, and we are in contact with big data all the time, so the processing of data becomes particularly important. 

##  Websites that help with Python learning 

##  summarize 

Having said so much, the purpose is to tell everyone that Python is a category that overwhelms other languages in terms of functionality and ease of use. As the most suitable programming language for beginners with zero basics, if you want to learn it, you can't just talk about it on paper. You have to settle down and study it in depth. 

![avatar]( 4a04b048cc0e49e4b84d248e4a0da216.png) 

 Just tell everyone what to learn but do not give direction is tantamount to playing hooligans, here is also to share my collection of technical dry goods, you can share with friends who like my articles, if you are willing to take the time to sink your heart to learn, they will definitely help you, dry goods content includes: All the above information I have packaged and uploaded to the CSDN official, click 👇 to get it if you need it! 



--------------------------------------------------------------------------------

###  I. Introduction 

Sometimes we let go of our hands and let the computer automatically send us some of the messages we want to send, which is rather labor-saving. 

>  For example, after writing a speech during the day and giving a text speech in the group at night, we can use the script to automatically copy, paste and send text, thus freeing ourselves from having to do the tiring work of CV repeatedly on the computer.. For example, in the live stream, you need someone to send bullet comments, and the automatic message sending program can replace the manual. You can also send the specified content after a fixed time, so you don't have to sit in front of the computer and send bullet comments.. For example, there are always some people coming in to advertise in your fan group, and they will not change after repeated teachings. Then you can use this automatic messaging program to bomb their group. By the time he notices, you have already sent thousands of messages, and withdrawing the message can make him withdraw to collapse... 

![avatar]( 90f34a3eb6884d0a84c82fe6b94a7f35.jpg) 

How often to send 1 message, or how many messages to send in 1 second, can be set freely. If the time is set short, it is no problem to send dozens of messages a second, but too fast will form the effect of swiping the screen... 

Today, I will share this trick with you. It is very simple and there is not much code. 

###  Effect 

Let's take a look at the effect first. What I set here is to start sending after a 2s delay, and send it once every 0.5s. 

![avatar]( 660e0f9369cd41f9be2121e60e9f374a.gif) 

###  III. The development environment 

###  IV. Analysis of key steps 

There are two main code files to achieve, the purpose is: to obtain the location of the chat window and to achieve the automatic sending of messages. The libraries used have been mentioned above. Before starting to write code, first download and install the libraries to be used. This will not be discussed below. 

Before we send a message, we need to know where the chat window is located, that is, where the mouse stays to locate the input interface of the chat window, that is, what are the x and y coordinates of the mouse. 

Here I use the three libraries os, time, and pyautogui to obtain the real-time position of the mouse: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538198
 ```  
As long as the program is running, every time we move the mouse, the mouse's x and y values will automatically sound and change and print out. We only need to call up the chat window and position the mouse at the input position of the chat window to obtain the current x and y values. With this x and y value, we can tell the following messaging program where to paste and push. 

![avatar]( ae6dd97eafea4d6699d93e57aa522c31.gif) 

  Of course, there are many ways to obtain the mouse position, and you can also try other methods to obtain it. 

After obtaining the values of x and y, what we need to do is, of course, to write a program to achieve "copy text → paste text → send messages". Here, we need to use pyautogui to control the keyboard and mouse, use pyperclip to control the computer to copy and paste, and use the time library to control the time. 

First of all, we prepare the content that needs to be sent in advance and put it in the content. At that time, we can use it directly. The content can be customized and modified, such as this: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538198
 ```  
We need to switch to the chat interface after running the code, and it takes time to do this manually. Therefore, before copying and pasting and sending the code, we need to set aside some time for ourselves. I have set a time lag of 4s here, and of course, we can also set it to start sending messages after a few hours. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538198
 ```  
The next step is how to implement copy, paste and send: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538198
 ```  
At this point, everything is done. If you feel that 5s is sending 1 message too fast, you can modify the value of 5 in time.sleep (5), for example, 10s sends a message; if you set it to 0.01 seconds, then it will be a quick message swipe effect... 

The "* 10" in the for loop controls the number of loops, that is, let it send text 10 times, or you can set it not to loop, and change the list (content.split ("\ n")) * 10 to content.split ("\ n"). 

The general method is the above. If you need the source code, you can chat with me privately. You can also try other ways to achieve it. To put it bluntly, it is to automatically send messages. There are many ways to achieve it, such as more advanced ones that directly bring xookie to adjust the API to send, etc., and the button wizard can also achieve this function. More exciting, waiting for you to dig it yourself. 

###  V. Summary 

The essence of this script is to automatically send messages to the computer, but the setting of the interval makes it also have the function of sending messages quickly, not only QQ, but also WeChat. 

The basic principle is this. You can also think about how to start the program after a few hours and send it every few minutes to completely free yourself. 

Thank you for reading and liking. I have collected a lot of technical dry goods that can be shared with friends who like my articles. If you are willing to take the time to study, they will definitely help you. The dry goods include: 

![avatar]( 17baf34c84e4483f9f9b3d9bb3341c44.png) 

![avatar]( 521e60d8459b40f2bd654b1a410926db.png) 

 Click on the business card at the end of the article to take it away.  



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

Python has once again won the title of "programming language of the year" by TIBOE, becoming the most popular programming language in 2021. Although I have always been optimistic about C #in 2021, I can't deny the global data thing, but I am not surprised at all. Instead, I am more convinced of certain things. 

![avatar]( 58aa175b2d464458ad7cfd42fcbfdb94.png) 

Although the trend of Python is only increasing, there are some things that are not clear to everyone. Although Uncle Long has written many articles about Python, it does not mean that I have to praise it. There is a reason why Python has such a high popularity and ranking. I hope my sharing this time can solve some doubts for everyone. 

###  The reasons why Python is gaining momentum may not be obvious to some people 

Many people think that the reason why Python has become popular is the rise of artificial intelligence and big data, but I think this is not the whole reason. Although Python is a programming language that is very suitable for the field of artificial intelligence, artificial intelligence is still in the early stage, and there is still a long way to go before the real landing, especially in China. Although the number of talents in artificial intelligence is increasing, but also because there are not many positions available, there is no graduate degree or above. No matter how good you learn Python, you will not be able to find a job in this area. 

Of course, this doesn't mean that it can't be implemented on a large scale in the future. It just means that if you rely on artificial intelligence and big data alone, Python is far from being as hot as it is now, at least I think so. 

![avatar]( 5dc85f1cb4f64416b5388c07d4c16b68.png) 

So why is Python still stronger than other languages? I think the non-programmer aspect also plays a big role. 

In addition to the C station, I also have accounts on platforms such as Douyin Kuaishou Xiaohongshu. When communicating with many fans on other platforms, I found that they are also learning Python, but they are not programmers and do not want to be programmers. The main reason for learning Python is that Python is easy to learn and can improve work efficiency and workplace competitiveness. 

![avatar]( a21b2a21d8514275bf8808ab20e8faed.png) 

They are positioned to learn Python as an auxiliary tool, and these groups already cover a wide range of positions, including operations, marketing, finance, new media, etc. These positions are in demand in almost every industry, which means that learning Python is no longer exclusive to programmers. 

Going back to the programming language ranking published by TIOBE, if you look closely, you will find that TIOBE's language ranking indicators include courses, the number of third-party providers, and the calculated ratings of major search engines. In fact, whether you are a programmer or not, as long as you are interested in Python and make relevant Internet behaviors, you are likely to contribute a piece of data to this score. 

![avatar]( 2f6f5be4d3a641ff8c77b82d241e3d90.png) 

  In fact, the answer here is already obvious. Programmers are just one profession in all walks of life in society, and there are many other professions. If many professions are learning or using a certain language, then the popularity of this language will definitely rise. In contrast to other programming languages such as C language, it is rare to hear that there are non-programmers who say they want to learn and use it in their work, so the popularity gap between Python and other languages is widened. 

The reason why Python is gaining so much momentum is that it also has a large data impact on non-programmers. 

This actually reflects some problems, since there are a lot of data from outside the industry, then in the IT industry, Python has not yet reached the appearance of the above so strong, at least at present can not shake the Java and other big-name languages, so want to be a programmer, the Java or continue to learn your Java, want to learn C #to learn C #, there is no need because of the strength of Python feel confused or deny anything. 

I don't mean to discredit Python, and it doesn't do me any good. I just want more people to have a good idea and look at current trends rationally. 

###  Second, should I learn Python? 

There are a lot of people who start to say "Python is seriously overrated", "Python has its own appearance, in fact, it can't do anything", and some people say "you can't find a job learning Python", some people may be very torn, so should you learn Python? 

I think it is extreme and undesirable to overhype Python, but is it not misleading to overly deny it? 

Can Python find a job on the recruitment website a search will know, I here to worry about the future as an example, were searched for Java, C++ and Python three keywords, the results are as follows: 

![avatar]( d4913482db67469fb87af1e0b4f63ba2.png) 

Java is currently the most used programming language on the market, recruitment needs have 1614 pages; C++ page is the old recruitment needs of a large programming language, there are 1260 pages; and the so-called Python can not find a job, the search results have reached 1012 pages, if learning Python can not find a job, then these recruitment is for those who can not breathe to see? 

If you say that learning PHP is hard to find or can't find a job, I can still understand, because its recruitment requirements are currently only more than 100 pages in the country, but Python is almost ten times that much. The daily data of the recruitment platform will not be the work of a certain organization, right? 

The original intention of making Python was not to use it to compare speed and performance, but to make it easier for more people to use it to solve problems, so there is no need to compare it with a certain language in terms of its incompetence. 

![avatar]( 5d5646964c114b37bbfbaa733ed5b0cd.png) 

Just like using a small bridge car and a large truck to compare speed or load, there is no comparison at all, and the positioning is different. What is the point of comparison? It is the most important thing to be able to solve the actual needs. 

Therefore, it is more rational to choose whether to learn Python or not. 

Python is still very good in crawling, data analytics, automated testing, and artificial intelligence (note what I said earlier), and there are many job requirements. Those who want to learn Python can consider these aspects. 

![avatar]( 98f5d8af4e1d4c8fb909282c65143fe8.png) 

 Of course, if you only want to use Python as an auxiliary tool or a secondary skill, there's nothing to talk about. Just learn it. Python is really useful.  

>  I have hidden a lot of technical dry goods for all fans (click here). 

Today's sharing is here first. If my sharing is helpful to you, please don't hesitate to share three times! 



--------------------------------------------------------------------------------

