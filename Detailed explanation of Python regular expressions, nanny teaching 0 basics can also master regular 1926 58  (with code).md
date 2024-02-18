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

