# Heroku

## First steps

- Install:

```bash
curl https://cli-assets.heroku.com/install-ubuntu.sh | sh
npm install -g heroku
```
- Login:

```bash
heroku login
```

- Create:

```bash
heroku create <heroku-app-name>
```

- Push:

```bash
git push heroku <your-branch> 
```

- Build and push:

```bash
git push heroku <heroku-app-name> <your-branch>:main
```

- Open deployed app:

```bash
heroku open
```

- Add remote origin:

```bash
heroku git:remote -a <heroku-app-name>
```

## Heroku and Rails

- Open rails console:

```bash
heroku run rails console
```

- Create database:

```bash
heroku run rails db:create
```

## DataBase commands

- Reset database:

```bash
heroku pg:reset DATABASE_URL
```
