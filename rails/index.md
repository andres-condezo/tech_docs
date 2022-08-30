# Rails

- Commands:

```bash
rails new app-name --api --database=postgresql

bundle install
 
bundle exec rails g bullet:install
 
rails generate devise:install
rails generate devise User
rails generate devise:controllers users -c=registrations
 
rails g cancan:ability
 
rails g controller user
 
rails db:migrate RAILS_ENV=development
 
rails server -p 3001
 
rails routes -E
 
rails active_storage:install
 
rails g scaffold Book title:string description:text isbn:string pages_count:integer
 
rails g model post AuthorId:Integer Title:string Text:string CommentsCounter:integer LikesCounter:integer user:references
 
rails generate migration add_collumn_to_users name:string photo:string bio:text posts_counter:integer
 
rails db:rollback STEP=1
 
 
rails generate rspec:intall
rails g rspec:system Post

rails g rswag:install
rails g rspec:swagger API::V1::CarsController 
```
