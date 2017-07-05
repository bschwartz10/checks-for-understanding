## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. What's the most useful thing you learned from completing the intermission week work?
   * Basic Javascript syntax and functionality

2. What are some tools to help debug JavaScript code?
   * PryJS
   * Chrome Console
   * Debugger

3. What are some tools you need in order to unit test your JavaScript?
   * Mocha and Chai

4. What is the syntax for invoking a function?
   * someFunction()

5. What's the difference between `==` and `===` in JavaScript?
   * The === operator does not do a type conversion and the types must be the same to be considered equal
   * The == operator will compare for equality after doing the necessary type conversion

6. What's the difference between asynchronous and synchronous JavaScript?
   * asynchronous code will not wait for a line to complete before moving on to the next line whereas synchronous code will wait until the line of code is completed before moving on

7. How do we setup a route when creating an API with Node and Express?
   * app.get('/api/secrets', function(request, response) {
   some code here.....
   }

8. What do we use Knex for?
   * Knew is a partial ORM thats helps us work with the database. It includes features like migrations and seeding. We can also interact with the database through Knex but using .raw to insert SQL.

9. What's `npm` and what do we use it for?
   * NPM stands for Node Package Manager and it allows us to install dependencies into our code just as Ruby Gems do in Rails.

#### Review  
10. What's the MVC design pattern? Describe each part of MVC?
   * MVC stands for Model, View and Controller respectively. The model houses all of our ruby objects. If we adhere to SRP principles our model should be the only part of our application that interacts with the database. Views are our ERB templates that users interact with. Each view corresponds with a RESTful action in the controller. The controller decides which routes go to which action and render the view accordingly. Each controller action defines instance variables that become available to us in the corresponding view.

11. What is AJAX? What are some benefits of using AJAX?
   * AJAX stands for Asynchronous JavaScript and XML. AJAX is a client-side script that interacts with the database and updates the page without requiring a refresh. Thus, is provides a much smoother UX because the page doesn't reload every time data is being read/written from the database.

12. What's a background worker? When would we want to use a background worker?
   * A background worker facilitates tasks in the background while the application is still running. Active job is an example of a background worker in the rails environment. We would want to use background workers when a task takes a long time to perform but we still want users to access other parts of the application.
