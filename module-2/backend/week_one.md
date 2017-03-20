## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
  GET - Read/Fetch information
  POST- Create information
  PUT- Update information
  PATCH- Modify information
  DELETE- Delete information
  
2. What is Sinatra?
  Sinatra is a back-end framework web development framework that is compatiable with Ruby. 

4. What is MVC?
  MVC stands for Model-View-Controller. It is an architectural patttern used for creating software.  
  
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  Create a standard across Ruby/Rails so its easier for other peole to understand our code.(readability)

6. What types of variables are accessible in our view templates without explicitly passing them?
  Instance variables
 
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    name = 'Mr.Ed'
    erb :index, locals: {name: name} 
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
9. What's the purpose of ERB?
  ERB is used to mix html with Ruby. It allows developers to create the structrure of the page and also run ruby code inside of it.
10. Why do I need a development AND test database?
  
11. What's responsive design?
  Responsive design allows flexibility when users are viewing the app on different sized screens.

12. What is CRUD and why is it important?
  CRUD stands for Create, Read, Update and Delete. It is important because it's a key functionality of all websites.
13. What does HTTP stand for? 
  Hypertext Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  <=% Ruby code... %> : This displays the evaulated ruby code on the page
  <% Ruby code... %> : This doesn't display the evaluated ruby code on the page.
15. What's an ORM?
  ORM stands for object relational mapper. This is a way to organzie database tables. It draws relationships between databases with foreign keys and join tables.
16. What's the most commonly used ORM in ruby (Sinatra & Rails)?
  Active Record.
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
  get '/restaurants' = see all restaurants
  get 'restaurants/:id' = see single restaurant
  get 'restaurants/new' = get form for creating new restaurant
  post 'restaurants' = click submit to create new restaurant and redirect to index page
  get 'restaurants/:id/edit'= get form for editing a restaurant
  put 'restaurants/:id' = click submit to edit current restaurant and redirect to show page
  delete 'restaurants/:id' = click delete and remove current restaurant
18. What's a migration? 
  A migration creates/updates/deletes a table/column in your database. It creates the table with the specific structrue you specified in you migration file.
  
19. When you create a migration, does it automatically modify your database?
  After creating the migration we need to run rake db:migrate to input the migration into the database.

20. How does a model relate to a database?
  The model directly interacts with the database through Active Record. 
  
21. What's the difference between agile workflow and waterfall method?
   Agile workflow is a continuous work cycle where you complete small complete iterations and continue to build upon them. Waterfall method plans all project specs upfront and then completes them all after. Waterfall isn't a good workflow b/c the project spec/expectations always change during the project lifecycle.
  
22. What is the difference between `#new` and `#create`?
  #create instansitates and new object and puts it into the database. #new instantiates the new object but doesnt save it in the database.
