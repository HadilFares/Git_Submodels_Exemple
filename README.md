# Git_Submodels_Exemple
Git Submodels :
The concept of submodules is brilliant. It essentially allows you to attach an external repository inside another repository at a specific path. In order to illustrate the value of submodules, it will probably be helpful for me to explain how I am using them.

# Add a repository as a submodule
git submodule add <repo>

# Add Submodule in our main repository
git status
git commit -am "Add  submodule in my main repository"
git push 

Note: a Submodule Git repository is checked out on a specific commit ; when new commits happen the checked out commit does not change 



# Update a Submodule
-Get the latest submodule repository updates

git submodules git submodule update --remote


# Clone a Project with Submodules and their contents
git clone --recursive <project-repo>

# But if we do just clone :
git clone <project-repo>
Note: folders submodels will be empty so to get all folders you must do this :

git submodels update --init --recursive 



References : https://www.youtube.com/watch?v=qsTthZi23VE&t=1283s
