# Notes-Week6-Revision-Best-Practice-Software-Internationisation
Notes-Week6-Revision-Best-Practice-Software-Internationisation

## Content

Slide 9/37 [![static/images/Screenshot-2023-10-16-202738-Best-Prac-Slide-1.png](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/blob/main/static/images/Screenshot-2023-10-16-202738-Best-Prac-Slide-1.png)](https://learn.ul.ie/d2l/le/lessons/10835/topics/457621)

Slide 10/37 [![static/images/Screenshot-2023-10-16-202738-Best-Prac-Slide-2.png](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/blob/main/static/images/Screenshot-2023-10-16-202738-Best-Prac-Slide-2.png)](https://learn.ul.ie/d2l/le/lessons/10835/topics/457621)

Slide 11/37 [![static/images/Screenshot-2023-10-16-205511-Best-Prac-Slide-3.png](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/blob/main/static/images/Screenshot-2023-10-16-205511-Best-Prac-Slide-3.png)](https://learn.ul.ie/d2l/le/lessons/10835/topics/457621)

Slide 23/37 [![static/images/Screenshot-2023-10-16-232100-Best-Prac-Slide-Tranlatable-xml.png](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/blob/main/static/images/Screenshot-2023-10-16-232100-Best-Prac-Slide-Tranlatable-xml.png)](https://learn.ul.ie/d2l/le/lessons/10835/topics/457621)


usually an xml fiile

ml = markup language.

xml container to transport text and meta info

so that you can determinee which cols can be translated and which should be imported

because don't want the label back.

what not ant to end up in xml

status of strings:
	- anything never translated
	- anything changed since translated
	- if found bug
	- changed English string
	- want translators to tranlslate
	- needs exported.
![image](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/assets/32943259/62eb0658-b68f-43cb-9fdb-56ac25572160)

in the next weeks in terms of CAP tools

1st of all will look at things like 

xml files.

______

what would see 

xml file

what want to visit

purple no

grey.

xml works like:

version of 

encoding="UTF-8">	

orange

<?xml version="1.0" encoding="UTF-8"?>


[CS4093_Week03_LiveLecture - CS6381 - BEST PRACTICE SOFTWARE INTERNATIONALISATION 2023/4 SEM1 (ul.ie)](https://learn.ul.ie/d2l/le/lessons/10835/topics/457621)


lecture slides
![image](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/assets/32943259/ad7400e6-b842-4511-a48f-f84e52a9c4d6)

_____

BREAK
_________

Is XML  programming language?

It is a markup language

if want to get stuff in  aformat 

that you can put back into your database

without stuff getting overwritten.

If don't have something like that
then you are
manually copying things

________

Parties involved

________

Who is involved in Software Development

Generally distinguish between the doing team

and the client

_____

the doing team

designers
e.g.
UI Designer

often in large companies 

someone who does the design
![image](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/assets/32943259/8d6d380a-2276-4e23-a325-badf4ba848b8)

_____

####### Extra notes from ChatGPT3_5

How do I make an HTTP request in Javascript?
In JavaScript, you can make an HTTP request using the XMLHttpRequest object or the fetch API.
Using XMLHttpRequest:

javascriptCopy code
constxhr = newXMLHttpRequest(); xhr.open('GET', 'https://example.com/api/data'); xhr.onload= () =>{ if(xhr.status=== 200) { console.log(xhr.responseText); } else{ console.log('Request failed. Returned status of '+ xhr.status); } }; xhr.send(); 
Using fetch API:

javascriptCopy code
fetch('https://example.com/api/data') .then(response=>{ if(!response.ok) { thrownewError('Network response was not ok'); } returnresponse.json(); }) .then(data=>console.log(data)) .catch(error=>console.error('Error:', error)); 
In both cases, you can replace the URL with the endpoint you want to send the request to and modify the request method (e.g. POST, PUT, DELETE) if needed.

please explain the code used for the fetch API in the previous response
Certainly! Here's a more detailed explanation of the code used for the fetch API example:

javascriptCopy code
fetch('https://example.com/api/data') .then(response=>{ if(!response.ok) { thrownewError('Network response was not ok'); } returnresponse.json(); }) .then(data=>console.log(data)) .catch(error=>console.error('Error:', error)); 
The fetch function is used to make an HTTP request. It takes the URL of the resource to fetch as its first argument, and returns a Promise that resolves to the Response object representing the server's response.
The then method is called on the Promise returned by fetch, which takes a callback function that is executed when the Promise is fulfilled. This callback function takes the Response object as its argument, which can be used to check the status of the response and extract its data.
In the callback function, the ok property of the Response object is checked to see if the request was successful. If it is not, an error is thrown.
If the response is OK, the json method is called on the Response object, which returns a Promise that resolves to the parsed JSON data. This is done assuming that the response body is in JSON format. If the response body is in a different format, you would use a different method to parse the data (such as text).
Another then method is called on the Promise returned by json, which takes a callback function that is executed when the Promise is fulfilled. This callback function takes the parsed JSON data as its argument, which can be used as needed (in this case, it's logged to the console).
If there was an error at any point in the chain of Promises (for example, if the network request failed), the catch method is called on the Promise returned by fetch, which takes a callback function that is executed when the Promise is rejected. This callback function takes the error object as its argument, which can be used to handle the error (in this case, it's logged to the console).![image](https://github.com/CoderSales/Notes-Week6-Revision-Best-Practice-Software-Internationisation/assets/32943259/306be2cc-d685-4927-b0a6-50968d43f047)

____

## References
