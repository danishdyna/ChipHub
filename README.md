# Chiphub: GIT Cheatsheat

GIT Cheatsheat for testing git stuff - and perhaps have some fun.
/ Henrik

## Repository - Change local clone
### Repo Clone Repo (Local repo)
```
git status
git clone https://github.com/danishdyna/chiphub.git
```
### Edit Repo (Use "VS Code", "Notepad", "vi")
```
notepad README.md
```
### Add & Commit files (Local repo)
```
git add -A
git commit -m "Fix formatting"
```
### Push files (Server Repo)
```
git pull
git push
```
## Branches - Change local branch
### Branch - Change branch (Local Repo)
```
git status
git branch -a
git checkout BRANCH-NEW
<Alter branch "BRANCH-NEW">
git pull
git commit -m "Changes to BRQANCH-NEW"
git push
```
### Branch - Rename HEAD (To "Main")
1) Repo "main" GitHub: "Settings/General/Default Branch/Rename"
2) Repo "main" Local:
```
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```
## Repository - New
### Repo - Create New "Main" (Server Repo)
```
git remote add origin https://github.com/danishdyna/PushRepo.git
git branch -M main
git push -u origin main
```
### Repo - Create new "Main" with files (Server Repo)
```
echo "# MyRepo" >> README.md
git init
git add README.md
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/danishdyna/MyRepo.git
git push -u origin main
```
## Authentication
### GIT - Identity Authentication (Forcing ID)
```
git config --global user.email "henrik.lassen@regionh.dk"
git config --global user.name "Henrik Lassen"   
```
