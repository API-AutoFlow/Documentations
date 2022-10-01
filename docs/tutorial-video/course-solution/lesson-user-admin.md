---
layout: default
title: Lesson 4 User Sigup
parent: Course 2 Full Stack
grand_parent: Tutorials - Video
nav_order: 4
published: true
---
<h6>Course 2: Creating solutions for your project</h6>
<h1 style="margin-top:0">Lesson 4: Enable Signup and Login</h1>

Now that you have a good understanding of the full stack, you get started to create the functions you need. 

The first set of functions that we'll develop is user management including signup and login.

[Video]

## Lesson Outline

1. **Database**
* Creating a User Table

2. **Backend**
* User Signup
* User Login
* Username Duplicate Check
* User Info Get
* User Update
* User Delete
* Change Password

3. **Frontend**
* VueJS Nuxt Authentication setup example


## 1\. Database

### Creating a User Table

MySQL example
```sql
CREATE DATABASE authentication_backend;
USE authentication_backend;
CREATE TABLE user(
    id                  BIGINT             AUTO_INCREMENT,
    username            VARCHAR(255)       NOT NULL,
    email               VARCHAR(255)       NOT NULL,
    first_name          VARCHAR(255)       NOT NULL,
    last_name           VARCHAR(255)       NOT NULL,
    password            VARCHAR(255)       NOT NULL,
    status              INT                DEFAULT 0,
    PRIMARY KEY(id)
);
CREATE TABLE test_data(
    id                  BIGINT             AUTO_INCREMENT,
    title               VARCHAR(255)       NOT NULL,
    PRIMARY KEY(id)
);
```

## 2\. Backend

In most cases, the configuration is hidden in the authentication package and you would simply download the configuration and use it. But it's good to understand what is going on under the hood if you want to add more functionalities and security.

Note that the user admin also has all the **CRUD** functions with some additional features based on the application needs.

![User Authentication](/assets/images/tutorial-user-admin.png)

Note
* `data/log` action is placed at the start of each flow during development for easier debugging.
* [check_input_type](/docs/tutorial-video/course-solution/lesson-signup/#input-type-check) is placed in each `POST` call to validate the input format.
* [authentication_token](/docs/tutorial-video/course-solution/lesson-signup/#authentication-token-check) is placed in all other calls to check the token's validity.
* [check_parameter](/docs/tutorial-video/course-solution/lesson-signup/#parameter-check) is placed in Signup and Login to validate that the Username and Password exist.

### User Signup

* Check User Duplicate

If Match (User exists)
* Failure response

If No-match (No user exists)
* Refer to the below [Hash password](/docs/tutorial-video/course-solution/lesson-user-admin/#hash-password)
* Insert User to the Database

### User Login

* Refer to the below [Hash password](/docs/tutorial-video/course-solution/lesson-user-admin/#hash-password)
* Check If User Exists

If Match (User exists)
* Refer to the below [Create Token](/docs/tutorial-video/course-solution/lesson-user-admin/#create-token)

If No-match (No user exists)
* Failure response

### Username Duplicate Check

* Check If User Exists

If Match (User exists)
* Success response

If No-match (No user exists)
* Failure response

### User Info Get

* Refer to below [Authenticate Token](/docs/tutorial-video/course-solution/lesson-user-admin/#authenticate-token)
* Check If User Exists

If Match (User exists)
* Success response

If No-match (No user exists)
* Failure response

### User Update

* Refer to below [Authenticate Token](/docs/tutorial-video/course-solution/lesson-user-admin/#authenticate-token)
* Check If Token Expired

If not-expired
* Update the username and password from database

If expired
* Token expired notice

### User Delete

* Refer to below [Authenticate Token](/docs/tutorial-video/course-solution/lesson-user-admin/#authenticate-token)
* Check If Token Expired

If not-expired
* Delete the user from the database

If expired
* Token expired notice

### Custom Actions

#### Input Type Check

The data needs to be in an object type.

If array
* Get the first value

If anything else
* Decode into an Object

#### Parameter Check

Check that input has all the required values.

Use the `iteration/all-are-true` + `data/is-non-empty-string` to validate there's no empty fields.

#### Hash Password

There are many ways to hash the password. Below is an example of using `SHA3_256` hashing method.

* **Hash password**: Use `security/hash` action to hash password with SHA3_256
* **String encode**: Use `string/base-16-encode` action to encode the hashed password

#### Create Token

It's interesting to see how the tokens are created in the backend. Below is an example of how a token gets created using the user `id`, `name`, and `expiration` date.

* **Get Current Unix Time**: Use `datetime/current-unix-time` action to get current unix time to set expiration date
* **Add time to current time**: Use `array/sum` action to add time to expiration date based (default 30 days or 2,592,000 seconds)
* **Create a data set**: Combine user id, username, and expiration as the base information for the token
* **Encode the base information**: Use `json/encode` to encode the base information
* **Encrypt to create token**: Use `security/encrypt` to encrypt the base information into a token.
* **String encode**: Use `string/base-16-encode` action to encode the encrypted token

#### Authenticate Token

Authenticate token is a reverse of [Create Token](/docs/tutorial-video/course-solution/lesson-user-admin/#create-token)

* **String Decode**: Use `string/base-16-decode` action to decode the token
* **Decrypt the token**: Use `security/decrypt` to decrypt the base information into a token.  Note that the `key`, `cipher`, `handle data`, and `handle key` need to be the same as when the token was encrypted in [Create Token](/docs/tutorial-video/course-solution/lesson-user-admin/#create-token)
* **Decode the base information**: Use `json/decode` to decode the base information
* **Get Current Unix Time**: Use `datetime/current-unix-time` action to get current unix time to compare with the expiration date

If < 30 days (Not expires)
* Success response + [Create Token](/docs/tutorial-video/course-solution/lesson-user-admin/#create-token)

If > 30 days (expired)
* Failure response

### Making Authenticated API Calls

* Refer to below [Authenticate Token](/docs/tutorial-video/course-solution/lesson-user-admin/#authenticate-token)
* Check If Token Expired

If not-expired
* Perform the desired actions

If expired
* Token expired notice

## 3\. Frontend

The below configuration is a [VueJS Nuxt](/docs/tutorial-video/course-supplementary/vuejs-nuxt/) package example.

```js
export default {
  // Modules for dev and build (recommended): https://go.nuxtjs.dev/config-modules
  buildModules: [
    "@nuxtjs/auth-next",
  ],
  
  // Modules: https://go.nuxtjs.dev/config-modules
  modules: [
    "@nuxtjs/auth-next",
  ],

  auth: {
    redirect: {
      // Login page. Redirect to this page if login required
      login: "/login",
      // redirect after logout
      logout: "/",
      // redirect URL for OAuth
      callback: false,
      // redirect after login
      home: "/profile",
    },
    strategies: {
      local: {
        httpOnly: true,
        token: {
          property: "token",
          global: true,
          maxAge: 36000,
          // required: true,
          // type: 'Bearer'
        },
        user: {
          property: "user",
          // autoFetch: true
        },
        endpoints: {
          login: {
            url: "/sessions/login",
            method: "post",
            propertyName: "result.token",
          },
          logout: {
            url: "/sessions/users",
            method: "delete",
            propertyName: "result.token",
          },
          user: {
            url: "/sessions/users",
            method: "get",
          },
          tokenType: "bearer",
        },
      },
    },
  },
  router: {
    middleware: ["auth"],
  },
};
```


{% include in_line_banner_config.html config_title="Organization" config_url="/assets/configs/_____.json" %}


[NEXT >> Lesson 11: Scheduling Flow Execution Using Timers](/docs/tutorial-video/course-1-basics/lesson-11-timers/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }