Welcome to "chiphub"

This repo is for testing git stuff - perhaps have some fun.

/ Henrik

# Configure your identity (once - should be chip mail address)
```
git config --global user.email "henrik@lassen.dk"
git config --global user.name "Henrik Lassen"   
```

# Create repo (once)
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
# Rename default branch
1) Rename "Deafault Branch" in GitHub: "Settings/General"
```
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```
