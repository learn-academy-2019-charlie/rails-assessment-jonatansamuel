# Rails Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

### 1. What are some advantages of using Ruby on Rails?

It's more user friendly. Very easy to read and can be fullstack.



### 2. How does Ruby on Rails use the Model View Controller (MVC) framework?
the models are for handling data and business logic, controllers for handling the user interface and application, and views for handling graphical user interface objects and presentations. 

-the browser on the client side sends a request for a page to the conroller on the server.
-the controller retrieves the data it needs from the model in order to respond to that request.
-the controller gives the retrieved data to the view.
-the view is rendered and sent back o the client for the broswer to display.


### 3. Using the information given, complete the steps for creating a new view in a rails app by filling in the blanks:

  1. Create a route: 
  
  code: 
  ```
  get '/about' => 'statics#about' 
  ```
  file: config/routes
  
  2. Create the Controller
  
  code: 
  ```
  class StaticsController < ApplicationController
  
  def about 
    render about.html.erb
  end
  ```
  
  file: statics_controller.rb
  
  3. Create the View
  
  code: 
  
  ```
  <div>This is the About page!</div>
  ```
  
  file: about.html.erb
  
  
### 4. Look at these sets of Rails routes, they are an example of which principle/term that we touched on briefly in class? Find the term, and explain why it is important.

```
/users/       method="GET"     # :controller => 'users', :action => 'index'
/users/1      method="GET"     # :controller => 'users', :action => 'show'
/users/new    method="GET"     # :controller => 'users', :action => 'new'
/users/       method="POST"    # :controller => 'users', :action => 'create'
/users/1/edit method="GET"     # :controller => 'users', :action => 'edit'
/users/1      method="PUT"     # :controller => 'users', :action => 'update'
/users/1      method="DELETE"  # :controller => 'users', :action => 'destroy'
```

This is a load of CRUD operations: Create Read Update Delete

### 5. What is the public folder used for in Rails?

public folders are accessible files for the public. They don't contain private or sensitive information and can be viewed for free. 

### 6. Write a rails route for a controller called "main" and a page called "game" that takes in a parameter called "guess"

class MainController < ApplicationController
  def answers
  render 

Rails.application.routes.draw do
get 


rails generate controller main


-get "/game/:guess" => "main#game"

### 7. What are cookies for? How do they work? What is the difference between a session and a cookie?

Cookies are normally set to give the appliacation a way of recognizing users when they visit again or later

you can use methods such as:

cookies.permanent[:username] = "example"

- to store cookies for longer than the current browser session. 



### 8. In an html form, what does the "action" attribute tell you about the form?  How do you designate the HTTP verb for the form?
The action attribute is used to inform the browser what page to call once the submit button is pressed.



### 9. Why would you use an instance variable in a rails controller?


it allows for your controllers to be available in your views.

### 10. Name two rails generator commands and what files they create:

rails generate controller
rails generate model


### 11. Rails has a great community and lots of free tutorials to help you learn. Here is a list of some tutorials to choose from, choose one, do it, and then report back here at least one thing you learned. You can also use a different resource if you find one that you like better. 

- https://www.tutorialspoint.com/ruby-on-rails/index.htm
- http://railsforzombies.org
- http://guides.rubyonrails.org/getting_started.html
- 

I found a udemy tutorial on rails and it has been super helpful.
