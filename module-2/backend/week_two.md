## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  - It is a file that contains instructions on how to build the schema
2. What is a migration?
  - It is a process that runs a series of files to create the table structure
3. How does a table relate to a model?
  - 1:1 -> each table should have a model
4. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  - class methods that define the relationships between tables
  - Example: Tags belong_to Tasks
5. What do they allow you to do?
  - They allow you to create relationships
6. What's the difference between agile workflow and waterfall method?
  - Waterfall workflow is done in chunks at a time, agile is done in strips
7. What is the difference between `#new` and `#create`?
  - new creates and instance of the thing, create saves it to the database
8. At a basic level, what does cURL allow you to do?
  - sends http requests
9. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  - teachers have many students
  - teacher --> student (teacher_id)
10. Define foreign key, primary key, and schema.
  - foreign key - an indexed field that relates to another tables primary key
  - primary key - the unique identifying field
  - schema - table structure
11. Describe the relationship between a foreign key on one table and a primary key on another table.
  - a foreign key is another table's primary key
12. What are the parts of an HTTP response?
  - message, http verb, path
13. `Rack::Test` allows us to test our controllers in isolation. What are some of the methods it gives us to simulate the request/response cycle?
  - last_response.ok?
  - last_response.message
14. Describe some techniques to make our Sinatra views more DRY. Give an example of when you would use these techniques.
  - Use a helper to contain logic that can be reused across views.
  - Also pull logic out of the controller to another class


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
3. What's the difference between agile workflow and waterfall method?
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
