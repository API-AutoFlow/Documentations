---
layout: default
title: Lesson 2 API Docs
parent: Prerequisites
grand_parent: Tutorials - Video
published: true
---
<h6>Prerequisites: Things you need to know before using API AutoFlow</h6>
<h1 style="margin-top:0">Lesson 2: Understanding API Documentations</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/CuE1sqryl_4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you have gone through my previous lessons,

You will understand that API Documentations are like a menu in a restaurant.

Well, API documentations looks very similar.

This API documentation is from an online OpenWeather.com service

You can see it’s very similar to a set menu.

Let’s select the current weather API from the menu

One of the first thing you see is an instruction on how to make the request or make the API call.

This is like an instruction on how to place your order.

This is how most of the web based APIs will look like

So, obviously, as a person creating the API

you’ll need to know what each parts of this URL mean because you have to create them.

Again, I guarantee you, you’ll be easily creating your own API after you finish these lessons.

Let’s look at each part of the API.

This time, let’s use food delivery app as an example

The domain address. It’s like I’m ordering from a restaurant called openweathermap.org. This is like the building or postal address. So this happens outside your API in what’s called Domain Name Service or in short DNS. I have a separate lesson on DNS for those you want to learn more, but for now think of it as a postal address to find my server.
Within the shop, I’m ordering from the API section. Similar to saying I’m ordering from meat section of the restaurant.
http is like how am I going to make the order? Some of you might have heard of things like FTP for transferring files, SMTP for emails, and so on.

This is simply a standardized way of receiving the order. We’ll go a little deeper into HTTP later because understanding your order is important when creating API.

Now, What am I ordering? I am ordering current whether version 2.5  This is like I am ordering beef prime grade farm raise steak.

Finally we have these something equals something. These are what’s called queries parameters to specify how you want the data. It’s like I want my steak medium rare with vegies on the side.

The question mark is simply indicating that query is starting, get it?  

Question mark => Query
and & is simply saying “and” there’s another query parameter

Once again, this is like a menu that the creator of the API specified.

When you create your own APIs, you will be specifying these parts.

For example If you build this on API AutoFlow,

You’ll have the DNS pointing to your server

Create an endpoint with the path /data/2.5/weather

And chain actions to provide the data.

For our purpose, since we don’t have access to the weather data, let’s create an action to respond with simple a message This is HOT!

You’ll learn how to apply queries and other cool things in later lessons.

Let’s first try the API we created.  Here we go, the API we created worked and we got the message This is HOT!

Now, let’s try the openweathermap.org API

Note, the way to indicate the things that you need to change is in Curly brackets.

For example,

Here, it is asking for a city name. Put anything else it wouldn’t work.  Let’s put London here
And “appid” we put the API key

When an API provider asks for an API Key, they generally provide it in your account section.

In a browser, enter the URL with the London and API Key

You will get the weather information of London.

Like anything, there are variations to how APIs can be made.

And we will go through them in our lessons



{: .fs-6 .fw-300 }

