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

