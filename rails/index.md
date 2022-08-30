# Rails

- Create Commands:

```bash
# Create new app: 
rails new [app-name] --database=postgresql

# Create new api only app: 
rails new [app-name] --api --database=postgresql
```

- g commands

```bash
# Create Scaffold:
rails g scaffold User name:string bio:text counter:integer

# Create controllers: 
rails g controller user

# Create model
rails g model post name:string user:references

# Create migration files:
rails g migration add_collumn_to_users name:string bio:text counter:integer
```

- db commands

```bash
# Create database
rails db:create

# Drop database
rails db:drop

# Run Migration files: 
rails db:migrate

# Show Migration status: 
rails db:migrate:status

# Rollback migration:
rails db:rollback STEP=1
 
# Run migration files in dev environment: 
rails db:migrate RAILS_ENV=development

# seed database
rails db:seed
```

- Bullet commands

```bash
bundle exec rails g bullet:install
```

- Devise commands

```bash
rails g devise:install
rails g devise User
rails g devise:controllers users -c=registrations
```

- Other commands

```bash
# Install dependencies:
bundle install

# Run rails server in different port:
rails server -p 3001

# Show rails routes:
rails routes -E

# Upload images: 
rails active_storage:install
```

- Rspec commands

```bash
rails g rspec:intall
rails g rspec:system User
```

- Cancancan commands

```bash
# Create ability file:
rails g cancan:ability
```

- Rswagger commands

```bash
# Setup rswagger
rails g rswag:install

# Create tests and yaml file:
rails g rspec:swagger API::V1::UsersController 
```
