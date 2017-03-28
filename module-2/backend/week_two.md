## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR.

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
>Active Record is a ruby tool that allows us to interact with a SQL library by using ruby. It acts as a liason between our models and our database. It allows us to query the database using ruby/active record methods.
2. Assume you have the following model:

```ruby
class Team << ActiveRecord::Base
end
```

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?
>We can call active record methods on team. Some example methods are .all, .find, .where, .find_by, .count. We have access to these methods b/c this class inherits from ActiveRecord.

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team?
>Team.find(4).name   Owner.find(Team.find(4).owner_id)

4. Assume that you added a line to your `Team` class as follows:

```ruby
class Team << ActiveRecord::Base
  belongs_to :owner
end
```

Now how would you find the owner of the team with an id of 4?
>Team.find(4).owner

5. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
> Teachers have_many students. Students have_many teachers.

6. Define foreign key, primary key, and schema.
> Foreign key identifies the primary key of an object in another table. Primary key is a unque value assigned to each instance of an object. Schema is a diagram of all the relationships in a program. 
7. Describe the relationship between a foreign key on one table and a primary key on another table.
> A foreign key on one table points to a primary key on another. They are referencing the same instance.
8. What are the parts of an HTTP response?
>The response is split up between the head and body. the head has the status code, content-length and other misc. info. The body has the raw html for the web page.

### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
3. What two columns does `t.timestamps null: false` create in our database?
4. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
5. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
6. Give an example of when you might want to store information besides ids on a join table.
7. Describe and diagram the relationship between patients and doctors.
8. Describe and diagram the relationship between museums and original_paintings.
9. What could you see in your code that would make you think you might want to create a partial?
