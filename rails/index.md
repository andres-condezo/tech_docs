# Rails

## Create Commands:

- Create new app: 
```bash
rails new [app-name] --database=postgresql
```

- Create new api only app: 
```bash
rails new [app-name] --api --database=postgresql
```

## g commands

- Create Scaffold:
```bash
rails g scaffold User name:string bio:text counter:integer
```
- Create controllers: 
```bash
rails g controller user
```

- Create model
```bash
rails g model post name:string user:references
```

- Create migration files:
```bash
rails g migration add_collumn_to_users name:string bio:text counter:integer
```

## db commands

- Create database
```bash
rails db:create
```

- Drop database
```bash
rails db:drop
```

- Run Migration files: 
```bash
rails db:migrate
```

- Show Migration status: 
```bash
rails db:migrate:status
```

- Rollback migration:
```bash
rails db:rollback STEP=1
```

- Run migration files in dev environment: 
```bash
rails db:migrate RAILS_ENV=development
```

- seed database
```bash
rails db:seed
```

## Bullet commands

```bash
bundle exec rails g bullet:install
```

## Devise commands

```bash
rails g devise:install
rails g devise User
rails g devise:controllers users -c=registrations
```

## Other commands

- Install dependencies:
```bash
bundle install
```

- Run rails server in different port:
```bash
rails server -p 3001
```

- Show rails routes:
```bash
rails routes -E
```

- Upload images: 

```bash
rails active_storage:install
```

## Rspec commands

```bash
rails g rspec:intall
rails g rspec:system User
```

## Cancancan commands

- Create ability file:

```bash
rails g cancan:ability
```

## Rswagger commands

- Setup rswagger
```bash
rails g rswag:install
```

- Create tests and yaml file:
```bash
rails g rspec:swagger API::V1::UsersController 
```
