## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. What is Webpack and why is it useful?
  *  Webpack is a node package that helps with the process of shipping code to production. Code that is optimized for a developer is not the most efficient for the browser. For this reason, Webpack helps with the transition from development code to production code. Webpack looks at our starter file and runs all the dependencies throughout our project. It will take care of preprocessers (i.e. SCSS) and minify our code into a single file for the browser to read.


2. When do you want to use event delegation?
  *  We want to use event delegation to avoid adding event listeners to multiple children. This can cause problems such as memory leak. Instead we want to put an event listener on a single parent.


3. What's one difference between ES5 and ES6?
  *  OOP syntax differs between ES5 and ES6. For example, instead of creating instance methods by doing class.protoype.methodName, we can just do methodName (). Also to create an member variable in ES5 we use the syntax of: this.name = name. In ES6 we use the constructor keyword followed by {} and define our variables within.


4. What's the deal with semi-colons in JavaScript?
  *  Semi-colons are used in Javascript to end a statement. They used to be required in older version of the language but not anymore. In ES6 they are looking to phase out semi-colon use. You have to end statements that start with () or {} with a semicolon.


5. How are you using the MVC design pattern in your Quantified Self project?
  *  I did my best to create a MVC framework within my QS project. I created my own model, controller and router files. I am using express router to correctly route a request to the correct controller action. From there the controller talks with the model and fires off a function to interact with the database. Once the database query is complete the model relays the information back to the controller and renders the correct json response.

6. How do you execute raw SQL in node?
  * You can excute raw sql in node by using knex's .raw method.

7. What's a callback function and what are some reasons when we use/need callback functions?
  * A callback function is a function passed into another function as a parameter and is executed when the parent function is called. An example of a callback function is $(#'some-button').on(click, function(){
    do stuff here....
    })
  When this function is triggered by a user pressing the button the code inside the callback function will be fired off. It's necessary in this instance b/c we want another function to be fired off after the button is pressed.

8. What is CORS?
  * CORS allows two web applications to speak with each other and give permissions to allow access.


9. What are some steps to avoid CORS?
  * Put configuration in the backend to allow CORS
#### Review  

10. Why do people say "HTTP is stateless"?
  * HTTP is stateless b/c it completely disconnects from your computer after the request/response cycle is complete. If you were to make the same request right after a previous one is completed the server wouldn't recognize you from your previous request. That is why cookies and sessions were created to persist data across the cycle.

11. What is a RESTful API?
  * A RESTful API follows HTTP standard conventions that has GET, POST, PUT and DELETE functionality.

12. What are some main characteristics of a team following an agile workflow?
  * Work in sprints. These sprints are usually 1-2 weeks and work to complete the project in spirals meaning each iteration delivers a full product and each sprint it becomes more complex. Agile workflows usually include a daily standup which consists of status updates for each member of the team.


13. What are some advantages/disadvantages to using OAuth to authenticate a user?

* Advantages are UX/UI friendliness. If you have OAuth I think your site looks more professional and it's easier for the user to log in with their FB account than create a new account for you website. A disadvantage is if your user doesn't have an account on the OAuth provider you chose. In this case you would need to create an alternative method for them to sign up/log in.
