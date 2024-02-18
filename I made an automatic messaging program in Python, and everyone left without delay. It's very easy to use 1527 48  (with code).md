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

