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

