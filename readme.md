# Test repo started on local machine

Plan is to push it to GitHub as a new creature

Steps used are:

* create local repo  
** create directory  
** `git init` there  
** add content outside of Git supervision (common file operations)
** `git add` all needed files (`git add .` for example)
** `git commit` this state

* now, I want to push this new repo to my GitHub account
* not found (yet?) a way to "force push" i.e. create remote repo and push there in one command so
* I have first to create dummy repo at GitHub (same name as local one)
on GitHub:
** create new repo, name=local_repo.name=="repo-st-local"
** write down GitHub response with this new repo URL, like `https://github.com/sivanhoe/repo-st-loc.git` in my case
* add this remote repo to local Git config with following command
`git remote add rem-mirror https://github.com/sivanhoe/repo-st-loc.git`
* and only then push local repo there with command
`git push rem-mirror master`
