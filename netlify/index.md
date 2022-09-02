# Netlify

- Install netlify-cli:

```bash
npm install netlify-cli -g
```
- Installation in a CI environment:

```bash
npm install netlify-cli --save-dev
```

- Continuous deployment:

```bash
netlify init
```

- Create toml file:

```bash
vim netlify.toml
```

- Content:

```bash
[build]
  command = "npm run build"
  functions = "netlify/functions"
  publish = " "

  [[redirects]]
   from = "/*"
   to = "/index.html"
   status = 200
```

## Other commands:

```bash
netlify login
netlify init
netlify deploy
netlify open
```
