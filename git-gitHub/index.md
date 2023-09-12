# Git and GitHub

## Configutations:

- Set user configuration:

```bash
git config [--global] user.name "Full Name"
git config [--global] user.email "email@address.com"
```
- Templates:
```bash
git config --global commit.template ~/.gitmessagevim ~/.gitmessage
```

## Branches:

- Delete a local branch:
```bash
git branch -d <branch-name>
```

## Other commands:

- Show repository status:
```bash
git status -s
```

- Create GitHub repo:
```bash
curl -u 'USER' https://api.github.com/user/repos -d '{"name":"REPO"}'
```

- Add SSH origin:
```bash
git remote add origin git@github.com:USER/REPO.git
```

- Change SSH origin
```bash
git remote set-url origin git@github.com:USER/REPO.git
```

- Change stage file permissions:
```bash
git ls-files --stage
```
```bash
git update-index --chmod=+x 'name-of-shell-script'
```

- Move last 3 commits to master
```bash
git branch -f master HEAD~3
```
