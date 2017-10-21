## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?
Node.js is a JavaScript run-time environment for executing JavaScript code server-side.  Its abiltity to be asyncronous in conjunction with it being javascript (meaning no context switching) makes it very popular.  

2. What is Express? What is Express similar to in the Ruby world?
Express is the jQuery of Node, making Node much easier to use and more understandable to code with.  In class we were told it was like Sinatra and jQuery.  Sinatra because Express is perfect for one page and smaller apps and jQuery in the sense that it makes Node easier to work with by providing a lot of shortcuts for common operations.  

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
Express is great.  If you have already set up the basic express setup (
const express = require('express')
const app = express()

You can then do a basic GET request like:

app.get('/', function(req, res) {
  res.send('Hello World!')
})

4. What do we use Knex for?
Knex is the ORM of Node.  So you can do ORM-type-things like SQL database queries and other database commands (like running migrations) using the Knex DSL.  

5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?
In both our client side app and our server side app we followed the MVC model where we had a basic app file that was the router and would direct to the controller, where we would keep our methods and instructions of what to do for that specific route.  If interaction with the database was required (as it often is) then that would go to the model file that would have all of the methods and instructions for dealing with the database.  In this way, we tried to be as MVC as possible and honestly after learning about MVC I am a believer in having a design pattern like MVC at all times for your own sanity.  

6. How do you execute raw SQL in node?
We would use database.raw('SQL COMMAND HERE')
This command would work because we had setup const database as the require of knex with the correct configuration already set up.  

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
The idea of having front end and back end code seperate is very aligned with OOP and aglie processes.  Also, I feel that it gives a lot of flexiblity with having different front end and back end languages and the ability to swap out those languages with different languages or updates without it affecting the whole program.
The disadvantage is that it could make things alot more complex and if you were doing all communication through APIs you might have to additional protections to keep sensitive data secure.

#### Review  

8. Describe DNS.
Domain Name Servers (DNS) are the Internet's equivalent of a phone book. They maintain a directory of domain names and translate them to Internet Protocol (IP) addresses.  This is necessary because, although domain names are easy for people to remember, computers or machines, access websites based on IP addresses, which are not so easy for humans to remember.

9. What does writing clean code mean to you?
Easy for future Bret to read and understand.  Follows the basics (Sandy Metz's guides), has comments, and is abstracted but not so much that it isn't understandable.  

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?
I think I suck at questions like this and it is something I need to practice so I am glad you asked this question.  I think of classes as nouns so for a hotel probably: rooms, floors, staff areas, entrence, bar, dining room, parking lot.  The functionality would be controlled by where it occurs so the 'welcoming' actions would be in the entrence, the 'cleaning' actions would be in the rooms, etc.  If you have resources on how to best understand this concept please let me know!

