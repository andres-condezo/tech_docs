# Heroku

```bash
curl https://cli-assets.heroku.com/install-ubuntu.sh | sh
npm install -g heroku
git push heroku development
heroku login
heroku create rent-a-car-bk
heroku open
heroku run rails console
heroku run rails db:create
heroku git:remote -a rent-a-car-bk
heroku run rails db:drop
heroku pg:reset DATABASE_URL
heroku run rails db:migrate
heroku run rails db:seed
```
