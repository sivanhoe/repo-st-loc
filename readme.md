# Test repo started on local machine

Plan A was to push it to GitHub as a new creature but failed as I could not find (yet?) a way to "force push" i.e. create remote repo and push there in one command.

Plan B was to make minimal necessary steps on GitHub staying essential part on local machine.

Steps used are:

## Create local repo and prepare it to sharing    
* create directory, "repo-st-loc" in my case  
* add content outside of Git supervision, with common file operations  
* `git init` in that directory  
* `git add` all needed files -- `git add .` for example  
* `git commit` this state

## Do necessary actions on GitHub  
Now, I want to push this new repo to my GitHub account. I have first to create dummy repo at GitHub (same name as local one).  
* create new repo, name=local_repo.name=="repo-st-loc"  
* write down GitHub response with this new repo URL, like `https://github.com/sivanhoe/repo-st-loc.git` in my case  

## Return to local machine and add this remote repo to local Git config with following command  
`git remote add rem-mirror https://github.com/sivanhoe/repo-st-loc.git`  

## And only now push local repo to GitHub with command  
`git push rem-mirror master`
