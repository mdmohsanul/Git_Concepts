# Daily git Workflow

- git clone <url>
- cd <repo_name>
- npm install - to install the project dependencies

- git checkout -b <branch_name>
- git pull origin main

- git add .
- git commit -m "Implemented login UI"

- git push origin feature/login

- after pushing create a PR 

# Difference between git fetch and pull

git fetch only downloads changes from the remote without modifying your working branch.
- git fetch 
- git merge origin main -> must manually merge if you want the changes:

git pull downloads and directly merges those changes into your current branch.
- git pull = git fetch + git merge
- git pull origin main