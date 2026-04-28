
```
git clone https://github.com/srikant/python-db-day2.git demo
cd demo
```
```
cd demo
git remote add origin https://github.com/srikant/python-db-day2.git
```
```
git fetch origin
```
```
git pull origin main        # or 'master' – check with git branch -a
```
```
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/github/gitignore/main/Python.gitignore" -OutFile ".gitignore"
```

```
cd demo
git init
git remote add origin https://github.com/srikant/python-db-day2.git
git add .
git commit -m "Initial commit"
git branch -M main          # rename branch to 'main' (if needed)
git pull origin main --allow-unrelated-histories   # if remote already has files you want to merge
git push -u origin main

```