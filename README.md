# GitHub code checkin
The objective of the repository is to create a git repo, making commits, creating branches and reviewing code changes.

# Steps
- Generate [ssh keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) and configuring that key in github.
- Optionally, we can use username and password to get access to our repo instead of ssh keys.
- Initialize our local repository with git, add sample file and commit changes.
- Create a repository in github and use git remote add option to connect your local repo with github remote repository in order to push the code.
```
cd <repo_name>
git init
git add greetings.py
git commit -m "Initial Commit"
git remote add origin <github_repo_url>
git push origin main
```
- Create a feature branch and make modifications in greetings.py file
- Commit those changes in feature branch and push the code.
- Raise a pull request to merge feature branch into main branch, review the changes and merge it.
```
git branch feature/<branch_name>
git checkout feature/<branch_name>
git add greetings.py
git commit -m "From Feature branch"
git push origin feature/<branch_name>
```
