---
layout: default
title: Lesson 4 Types of Data Used in API
parent: Prerequisites
grand_parent: Tutorials - Video
---
<h6>Prerequisites: Things you need to know before using API AutoFlow</h6>
<h1 style="margin-top:0">Lesson 4: Types of Data Used in API</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/3pF43lMA018" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

When working with APIs, you’ll come across different types of data.
For example, your normal text, numbers, lists and so on.
Since creating an API is all about working with data,
It’s important to have a solid understanding of each data types
Let’s jump right in.

First let’s get the obvious ones out of the way.
Text in the data world is called “String”.  Why String? You can think of it as a string of characters.
Number is just a number. Like 1,2,3
Note, String 1 is different Number 1.
This is a very commonly made mistake

For example,
You get string 1 in your request body. 
If you are not familiar with HTTP request and response, I recommend you go back to my previous lesson before moving forward.
You want to do some calculation or comparison with another number.
Let’s use an action that compares two numbers and tells us which is larger.
Notice you get an error.  That’s because String 1 a text, not a number
So, we’ll have to convert the String 1 to a Number 1.
You can do that by using the string to integer action.
Problem solved.

The next two data types Boolean and Null are simple,
But they are extremely important and comes in handy when working with data.
For example. Boolean data type is just True and False.
As you can imagine, when working with condition like IF do that,
boolean data becomes the base for making the decision.
Null or Empty is maybe not a data type.
But, there are many cases when you get no data.
So, knowing when you have so data is important.
Again
String True is different Boolean True.
And
No number is not same as Null

So far we’ve looked at data types that has single value,
But what data types are there for storing multiple values.
The two most commonly used data types are Array and Object.
Don’t be fooled by their names. 
Array is just a list
and Object is a value wait a key.
And to differentiate the two,
They used different encapsulation
List uses Square bracket
And Objects use  Curly braces
Let’s take a look at List first.

Let’s say, I have a list of numbers here.
When working with list, you simply refer to value in a position. 
For example, I want to get value in the 2nd position, which is 1
I want to add number 5 to the back of the list, and so on.
So for list, everything works based on the positions.
Now, those of you who have worked with lists before may be thinking,
The value in the 2nd position is not 2? It’s 2.
What is the confusion here?
Well, that’s because with lists, the position numbering start from Zero, not One.
Confusing right? But you just have to remember that about Lists. Position starts from Zero.
Technical term for position is called “Index”.
So, value in index 2 is 2.
That’s all you have to remember about List.
Cool thing about List is that you can have any value in there.
Whether it’s a number, text or object.
Can you guess what the value is in the index 1?
Yes you are correct, it is letter “b”, because index starts from 0

On API AutoFlow
You can define list by simply adding more values.

Another way to store multiple value is by using Object.
Object is simply putting name to the value.

Don’t be confused with the URL variable. That’s just letting you know it’s something you have to fill in.

Another way to store multiple value is by using Object.
Object is simply putting key to the value.  Key is simply a name you give to a value.
So unlike List that uses position index,
Objects uses the keys to get the value.

For example, to get the my first name peter, I would refer to key first_name.

You might have heard of JSON before.
You can think of JSON as a text representation of Object.
It looks like an Object, but it’s really a text. 

Most of the time when you receive data, you will get it as a JSON format.
So, you’ll need to decode JSON into an Object to get data from a specific key.

Finally, let’s look at two other data types Binary Digit and Hexadecimal.
Binary digit is your 0s and 1s, the smallest unit of data in a computer.  You need this when working with IoT or Industrial use cases.
Hex is a 16 symbols  more numeral system to make binary more human readable
There’s a separate lesson on how to read binary and hex later in the course.

We’ve went through some of the commonly used data types.
You’ll get used to them once you start making APIs.


## About this Course
[Image]
Instructor
Peter Jung
Chief Product Officer
Interactor.com

{: .fs-6 .fw-300 }

