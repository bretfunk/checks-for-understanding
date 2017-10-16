## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?
arrow functions

2. What's the difference between asynchronous and synchronous JavaScript? 
asynchronous can run multiple things at the same time totally independant of each other

3. What are the four pillars of Object Oriented programming?
Abstraction, Encapsulation, Inheritance, Polymorphism

4. What are some tools available in JavaScript to help you write object oriented code?
classes, objects, constructor functions, etc.

5. What are some key concepts to be aware of when refactoring your JavaScript?
Be consistant, only use ES6 or ES5.  Seperate by functionaliy, like AJAX calls, etc.

6. What's a callback function and what are some reasons when we use/need callback functions?
A callback function, also known as a higher-order function, is a function that is passed to another function as a parameter, and the callback function is called (or executed) inside the function. These 'first class functions' are unique to JS and are used often, on prettymuch every JQuery method. 

7. What's the scope of variables in Javascript?
JavaScript has two scopes – global and local. Any variable declared outside of a function belongs to the global scope, and is therefore accessible from anywhere in your code. Each function has its own scope, and any variable declared within that function is only accessible from that function and any nested functions. Because local scope in JavaScript is created by functions, it’s also called function scope. When we put a function inside another function, then we create nested scope.

8. What's the difference between `==` and `===` in JavaScript?
If you don't know the difference than always use '==='!  "===" is more strict and usually the one a programmer would use. 

9. Why do front end frameworks exist?
To make life easier.  JS can be a mess and inconsistant and as we move to a mobile first world things like responsiveness and speed are demanded by the end user so very clever people make front end frameworks to make the front end programming process easier.  

#### Review  

10. Why do people say "HTTP is stateless"?
As far as HTTP is concerned, they are all requests are separate requests and must contain enough information on their own to fulfill the request. That is the essence of "statelessness". Requests will not be associated with each other absent some shared info the server knows about, which in most cases is a session ID in a cookie.

11. Describe a RESTful API.
A RESTful API is an application program interface (API) that uses HTTP requests to GET, PUT, POST and DELETE data.

12. What are some main characteristics of a team following an agile workflow?
There are many different agile software development philosophies but the overall goal of each Agile method is to adapt to change and deliver working software as quickly as possible. As an example, the full Agile software development lifecycle includes the concept, inception, construction, release, production, and retirement phases.

13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
advantages: you are not keeping senstive data on your server.  The process is easy to setup and users like having the option.  
disadvantages: you have less control over the authentication process, specficically, the amount of data you are able to keep.  
