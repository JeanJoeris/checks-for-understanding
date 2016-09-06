## Week Three Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What are the 3 main features in an ERD?
  * entities, their relational verbs and their attributes
2. Create an ERD for the following database: Restaurants, Customers, Items, Ingredients, Beverages, Orders, Vendors.
  * did drawing
3. What is the entry at the command line to create a new rails app?
  * rails new <project-name>
4. What do Models generally inherit from in rails?
  * ActiveRecord::Base
5. What do Controllers generally inherit from in a rails project?
  * Application Controller
6. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  * `get '/horses/:id, to: 'horses#show'`
7. What rake task is useful when looking at routes, and what information does it give you?
  * rake route, it tells you the path, the verb, the prefix, and controller/method
8. What is an example of a route helper? When would you use them?
  * `link_to <link_name> <href>`
9. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  * url gives the whole url, while path gives just the path relative to root
10. What are strong params and why are the necessary?
  * they are objects that encompass just the params paroperties we want, they are necessary so we don't grab any unsecure params. 
11. What role does `form_for` play in helping us create our forms?
  * It is for making forms for a specific model object. It uses the model attributes to help simplify the forms
12. How does `form_for` know where to submit the user's input?
  * it uses the prefix paths (e.g. put to "thing#create")
13. Create a form using a `form_for` helper to create a new `Horse`. 
  ```
  <%= form_for(@horse) do |f| %>
    <%= f.label :name %>
    <%= f.text_field :name %>
    <%= f.label :breed %>
    <%= f.text_field: breed %>
    <%= f.submit %>
  <% end %>
  ```
14. Why do we want to validate our models?
  * we want to validate our models so we can have control over what kind of data is ok to save to the db. We can require data we need or ensure uniqueness, or lots of other things
