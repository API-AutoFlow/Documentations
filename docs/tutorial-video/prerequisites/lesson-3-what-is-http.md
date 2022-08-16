---
layout: default
title: Lesson 3 What is HTTP
parent: Prerequisites
grand_parent: Tutorials - Video
---
<h6>Prerequisites: Things you need to know before using API AutoFlow</h6>
<h1 style="margin-top:0">Lesson 3: What is HTTP</h1>


<iframe width="560" height="315" src="https://www.youtube.com/embed/ya4fFjBq4g4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Have you ever wondered what http in front of every URL means?
If you have gone through my previous lessons,
You will have a good understanding that API is like a food delivery order.
You have an agreed way of making the order like an APP
You have a set menu and you have some options to specify how you want it served.
But if the parameters were the only way to specify your request, it will be very limiting right?
For example, the APP needs to have ways to update your order, delete your order, and so on?
Similarly, APIs have agreed upon ways of making these requests and responses.
That is called HTTP protocol.

For those of you who don’t know what protocol means in technology.
It simply means and agreed way of doing thing.
For example, when sending a letter, there’s a agreement that you
1. Write the addresses on the outside
2. Recipient address goes on the bottom right
3. Sender’s address goes on the top left.
Any deviation from this protocol, you run the risk of letter not getting delivered

HTTP protocol works in a similar way.
In a request, there are specific places that you have to put the information.
It’s a rule.  If you don’t put the information in the right field, things are just not going to work.
Understanding HTTP is not hard, they are just fields you get the user of your API to fill in.
Query we’ve looked at. This is where you specify how you want the data to be served.
Method is where you specify whether the API is for getting the information, editing, deleting, and so on.
Depending on what you specify here, the API can have different set of actions, even if the URL is the same.

For example,
I have three actions with same URL but different methods
Here you see /test GET method has a different set of actions to POST and DELETE

Header is normally used to include authentication information
Body is where you put the information you want to send.
For example, if you have an API that can write to a database or file,
You’ll need to receive the information somewhere.
Normally body is where you’d have a way to include that information.
There’s a standard way APIs respond as well.
The status code is a way to tell the user of your API what went wrong or right.
For example, APIs respond with 400 range when request is wrong
But if you get number in the range of 500s, it means something went wrong in the API.
200 indicates that everything went as expected.
Response body is where the information is store.

For example,
When we made a call to openweather API,
What you see here is what’s be sent back in the response body.
Pretty simple right?
Again, HTTP is not hard.  They are just fields.

API testing tools like Postman made this easy to test APIs
And they provide HTTP request field you can fill in.

You have the tabs to just put in the HTTP request fields and you’ll get the response.
Here I will put the query parameter in the tabs provided instead of the URL.
I get the same response.

For creating and integrating APIs to a solution,

API AutoFlow provides the HTTP request and response fields for you to create the solution.
You can simply dragndrop the actions for your API to perform when it receives a request..
Here I have an action that simply copies the information in  HTTP request body.
Let’s go back to the postman and see if our newly created API works?
I’ll put Hello in the request body and see what response I get.
There you go! We have successfully created an API that copies information in the request body field to the response body.
Even when you are integrating API,
you can use the HTTP request action like you would with Postman.
Difference is that we are not just testing the API, we are using the API.
Just fill in the HTTP request information and you’ll get the response back from the API.  (Use the openweather API)
You see that the Openweather gave back the information in the response body
Now you can use this information as part of your solution.

As you can see, creating and integration APIs is not hard.
A quick recap,
* HTTP is a protocol on how to make request and response
* There are fields for different purposes.
* As a creator of the API, you can utilize any of these fields. (show dragndrop of data into action)
If the video was helpful, please share with someone could also benefit from this tutorial. And don’t forget to press follow for the latest updates.



{: .fs-6 .fw-300 }

