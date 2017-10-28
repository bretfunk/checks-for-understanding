## Week Four - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's your favorite project management tool?
I use Trello day-to-day but really like Tracker for software related tasks.  I feel like I am just scratching the surface of what Tracker can do so I look forward to using it on-the-job.

2. Why do we create staging environments?
To simulate live conditions without the repercusions of live conditions.  For the same reason flight schools use bad weather simulators instead of actually sending flight students to their possible death in adverse weather conditions (this is actually the hardest part of flight school and where most people wash out, my school had a 10% pass rate!).

3. What are the characteristics of a good README (in your opinion)?
Based on my QS assessment I think I am the wrong person to ask but what I look for in a READ ME for a new gem is 1. easy to understand, 2. assume nothing of the reader, spell things out, and have the most useful information at the top.  This is the same for good writing in general but for techincal writing it is extra important.  Something I should have done on QS in retrospect was to follow our installation instructions to see if they were easy to follow and if I missed any steps.  Oops.

4. What's one main improvement you're going to make to your code regarding accessibility issues?
For QS we intentionally used buttons on everything for ease of accessability.  That and contrasting colors for our app.  After using Vim for three months I want to go full keyboard, even in Chrome, so I hope this will really help me understand the importance of accessability because I too won't be using a mouse.  

5. What are some basic security concerns to be aware of when building applications?
The most intersting one to me is clickJacking, or where hidden buttons do hidden actions to unsuspecting users.  For me, I think being aware of the problem and getting some time using some of the gems out there to test vulnerabilities in your code is a good idea.  I talked to a Turing grad over the break for job advice and he told me that their company got hacked and it was his code that added the vulnerability.  It was very sobering to hear.  This is important stuff.  I know when I worked with the Senate Intel Committee on Cybersecurity issues this was something that came up alot.  My Senate office was constantly targeted by foreign governments and as our Sys Admin I renwed my Secret clearance so I could better defend us from attacks.  Even my secret clearance info (along with millions of others) was stolen by hackers a year or two ago.  Much, much worse for the US Gov than Equifax.  This is important stuff and it affects everyone.  

6. Why is continuous integration helpful/important?
Continuous integration (CI) is the practice of merging all developer working copies to a shared mainline several times a day (like github) and testing every build to make sure it works (like with TravisCI).  For me, as programs get bigger and you are reviewing lots of code, the first question you ask is "does this code even work?".  CI products solve this problem by running the code for you to make sure it works.  When I was jobshadowing with Healthify I asked them about this and they used Travis CI (and it wasn't able to run the app while I was shadowing!).  

7. What are some continuous integration tools?
TravisCI, CircleCI, AppVeyor, Percy, Buddy, Semaphore.  (I had to google this and had only heard of Travis CI previously).

#### Review  

8. What are some characteristics of "good" git workflow?
If on a team project not pushing to master and having others review and comment on your code.  Will and I were really good with this on QS, the only issue for us is once things aren't working on Heroku or Github pages then you have to push to master to test your code until it works correctly.  I know for us we have to rebuild the buttons because Github pages wouldn't load our code properly even thought it worked fine on localhost.  Other than that, don't push to master!

I also think using branches, commiting often, having a good commit sytem that works with your project managment app cards,  etc. are all good practices.  

9. What are the four fundamental concepts of object oriented programming?
 Encapsulation -Tthe internal representation of an object is generally hidden from view outside of the object’s definition.  Programs and components are built out of pieces.
 Abstraction - Abstracting out elements.  Pieces have limited knowlege of each other.  
 Inheritance - A way to reuse code of existing objects.  Functionality in layers.   
 Polymorphism - One name, many forms, ie, more than one identity that fits under a general identity.  

10. What's a module in Ruby and what's the difference between a class and a module?
Classes are all about objects, modules are all about methods.  Modules are the equliviant of lockers of methods that you can use across multiple classes, like libraries of functionality.  Often, at least at Turing, we use classes as modules (ie lockers of methods) when we really should be using modules.  When I first wrote this answer I used 'functions' instead of 'methods.'  I think JS is runing my Ruby knowlege.  Ha.  
