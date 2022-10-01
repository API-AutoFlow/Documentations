---
layout: default
title: Lesson 2 Frontend
parent: Course 2 Full Stack
grand_parent: Tutorials - Video
nav_order: 2
published: true
---
<h6>Course 2: Creating solutions for your project</h6>
<h1 style="margin-top:0">Lesson 2: Integrating Frontend</h1>

The frontend is what the users see or experience.  The frontend calls the backend APIs built on API AutoFlow.  Based on the type of frontend, there are different ways to call the APIs.

{% include in_line_banner.html url="/docs/tutorial-video/course-supplementary/vuejs-nuxt/" title="Learn how to use VueJS in 15 mins" button_name="Watch a training" message="! Get started with full VueJS setup instruction video" %}


## Lesson Outline

1. Javascript example
2. VueJS example

---

### API Spec

Using the **Hello World** example from the previous lesson.
* **Address**: `localhost:27836`
* **Method**: GET

---

### Javascript API Call Example
Below is a simple Javascript example of the API call

```html
<!DOCTYPE html>
<html>
<body>
  <p id="demo">Fetch a file to change this text.</p>
<script>
  let url = "http:\\localhost:27836"
  // Fetch data
  fetch (url)
  .then(x => x.text())
  // Display data
  .then(y => document.getElementById("demo").innerHTML = y);
</script>
</body>
</html>

</script>

```


### VueJS  API Call Example
There are several ways to do so, but a very popular approach is to use axios, a promise-based HTTP client.
[Learn how to install and use VueJS](/docs/tutorial-video/course-supplementary/vuejs-nuxt/)

```java
new Vue({
  el: '#app',
  data () {
    return {
      info: null
    }
  },
  mounted () {
    axios
      .get('http:\\localhost:27836')
      .then(response => (this.info = response))
  }
})
```

```java
<div id="app">
  {{ info }}
</div>
```

Reference

https://v2.vuejs.org/v2/cookbook/using-axios-to-consume-apis.html?redirect=true


### Important!!  CORS policy
If you see the below error, check to make sure you set the [ACCESS CONTROL](https://www.interactor.com/support/forum/4) on API AutoFlow Server.

```html
Access to fetch at 'http://localhost:27836/' from origin 'null' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource. If an opaque response serves your needs, set the request's mode to 'no-cors' to fetch the resource with CORS disabled.
```

## CRUD

When creating APIs, there are some basic methods that the application should support. 

| CRUD       | Method           |
| ------------- |:-------------:
| **C**reate  | POST  |
| **R**ead | GET  |
| **U**pdate | PUT (Replace) ,  PATCH (Modify) |
| **D**elete  | DELETE  |

In the API AutoFlow, the 4 methods are created to do the CRUD functions.
![CRUD API Methods](/assets/images/tutorial-frontend.png)


[NEXT >> Lesson 2: Integrate a Database](/docs/tutorial-video/course-2-solution/lesson-2-database/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }





