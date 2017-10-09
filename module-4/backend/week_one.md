## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?
I really like learning about how front end and back end programs are completely seperate programs and connect through APIs.  Maybe that isn't as sexy as learning AJAX or something but to me this changes the way I look at programming and opens up a lot of ideas for my personal project (like a golang backend and a react frontend)

2. What are some tools to help debug JavaScript code?
I find debugging in JS much harder than Ruby.  The error codes are not as helpful!  I use debugger, the console and the error messages in the npm start webpack server compiler to help debug.  This is an area that I feel I could def improve on so I will keep working on it.  

3. What are some tools you need in order to unit test your JavaScript?
In class we used Mocha and Chai.  Mocha is for unit testing and Chai adds a bunch of useful methods like deepEqual that normally wouldn't say two strings or two arrays are equal because they are in different places in memory.

4. What is the syntax for invoking a function?
function multiply() {
statements
};
let functionName = () = {
statements
};
var multiply = new Function(x, y, statements);

5. What's `this` in JavaScript?
This references the object you are inside (if you are not inside an object it will reference global or window).  The one caviot here is if you are in an object of an object it will reference the global scope.  Many consider this a bug but it was created intentionally by the high council of Javascript.  

6. What is Webpack and why is it useful?
Similar to the asset pipeline in Rails, Webpack condenses all of the assets (JS, CSS, SCSS) into one file of readable code (JS instead of JSX or CSS instead of SCSS).  This makes everything faster and easier for the user, the server and the programmer.  This does mean everything needs to be formatted correctly to complie correctly so it can causes additional issues for the programmer.  

7. When/why do you want to use event delegation?
This was the only question I had to look up.  Event delegation allows us to attach a single event listener, to a parent element, that will fire for all descendants matching a selector, whether those descendants exist now or are added in the future.  I.E. this allows us to use parents and children in our events, saving time and hassle and keeping our code DRY.

8. What's `npm` and what do we use it for?
Node package manager, we use it to install packages and help with dependancies.  I heard there are better ones for Node out there but it is a good place to start.  

#### Review  
9. What's the MVC design pattern? Describe each part of MVC.
MVC is a way of organizing a program.  MVC stands for Model View Controller and componets of the program are seperated into the M, V, or C sections of the program depending on their function in relation to the whole.  All work together to make the program work correctly so that the user gets what they want and the programmers have a repeatable blueprint that is easy to code and easy to update.  Models are all about the data and talk to the database.  Views are all about the user and making sure they see the information they are suppose to see.  The Controller is the brain that decides what views and models to access depending on what the user is requesting.  

10. What are a few ways to optimize a Rails application?
Load order of the page, for instance, have a png of a big banner at the top of the homepage load first so the user thinks the page loads instantly while the API calls that take longer are further down the page.  Also, using background workers to offload tasks that aren't as timely like sending a user an order confirmation email, no reason for the user to wait while the email is sent.  Also, just benchmarking your site would probably help identifiy problem areas on which to focus.  

11. What's a background worker? When would we want to use a background worker?
Background works are things that work in the background.  I honestly felt that although this was covered alot in Mod3 that I never fully grasped the difference between background workers, rake tasks, action jobs, etc.  To me they all do the same thing (which is, run things we want to do (ie functions) at a time of our choosing, whether now or later).  We would use these when we want to speed up the user experience, like when we want an email to go to a new user but we don't want the new user to wait on the page loading for the email to send.  Send it to a background worker to be done when it is ready and the user doesn't have to wait. 
