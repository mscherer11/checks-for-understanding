## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
  - GET
  - POST
  - DELETE
  - PUT
  
2. What is Sinatra?
  - A ruby gem that lets ruby interact with a server
4. What is MVC?
  - Model
  - View
  - Controller
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  - It makes it easier to debug
  - It is easier for other developers to follow code
6. What types of variables are accessible in our view templates without explicitly passing them?
  - instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
  ```ruby
  get '/horses' do
    @count = 1
    erb :index, locals {name: "Mr. Ed"}
  end
  ```
9. What's the purpose of ERB?
 - A way to write an HTML template and pass ruby code
10. Why do I need a development AND test database?
  - So you can create test data for specific scenarios, and so you can develop in a sandbox
11. What's responsive design?
  - When the page can adjust to the size of the browser/device
12. What is CRUD and why is it important?
  - Create, Read, Update, Delete
  - It is the foundation for interacting with a web app
13. What does HTTP stand for? 
  - HyperText Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  - <%= thing %> -- returns data to show on the page
  - <% thing %> -- doesn't return data
15. What's an ORM?
  - Object Relational Mapping
16. What's the most commonly used ORM?
  - Active Record
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
  - Read/GET - one
  - Read/GET - all
  - Create/GET - load form
  - Create/POST - save form
  - Update/GET - see form
  - Update/PUT - save form
  - Delete/DELETE
18. What's a migration? 
  - A file that builds a portion (or entire) table in a database
19. When you create a migration, does it automatically modify your database?
  - No - you need to give the command to modify a table
20. How does a model relate to a database?
  - It is the ruby class that contains logic and interacts with the data
