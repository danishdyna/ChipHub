Welcome to "chiphub"

This repo is for testing git stuff - perhaps have some fun.

/ Henrik

# Configure your identity (once - should be chip mail address)
```
git config --global user.email "henrik.lassen@regionh.dk"
git config --global user.name "Henrik Lassen"   
```

# Repo Clone (once)
```
git status
git clone https://github.com/danishdyna/chiphub.git
```
# Edit
```
vim README.md
```
# Add/Commit files (all)
```
git add -A
git commit -m "Fix formatting"
```
# Push files
```
git pull
git push
```
# Branch - Rename (Default)
1) Repo "main" GitHub: "Settings/General/Default Branch/Rename"
2) Repo "main" Local:
```
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```
# Repo - Create new (Command Line)
```
echo "# MyRepo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/danishdyna/MyRepo.git
git push -u origin main
```
# Repo - Push new (Command Line)
```
git remote add origin https://github.com/danishdyna/PushRepo.git
git branch -M main
git push -u origin main
```
