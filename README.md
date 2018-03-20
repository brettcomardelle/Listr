# Listr
Ionic application integrated w/Alexa to auto-generate shopping lists

# Notes
Before working on a feature/issue, look to see what branches are currently being worked on to ensure you aren't building the same thing.
Also, only work on 1 feature/issue at a time to avoid confusion and mis-handling of commits.

At times that we are working on a big feature, such as Alexa integration, make your branches mean something short. For example, a cbranch
to make a new command. This way, massive changes in code are not being done at the same time on two different versions. This cannot be done
perfectly, however, but that is what merge conflicts are for :)

# How to Work on a Feature/Bug
  1)  Choose a feature/issue
  2)  Ensure your local master branch is up-to-date
  3)  Create a branch for your feature/issue with a name that defines it
  4)  Code
  5)  Push your branch to the repository (origin)
  6)  Create a pull request to merge it with the master branch
  
# Example branching/commiting
  1)  git checkout master
        - Switch to the master branch
  2)  git pull
        - Fetches the latest code in master and merges it with your local master branch
  3)  git branch BathroomMenu
        - Creates a new branch called BathroomMenu
  4)  git checkout BathroomMenu
        - Switch to the BathroomMenu branch
  5)  Code
        - Implement you feature/fix
  6)  git push origin BathroomMenu
        - Deliver your code to the BathroomMenu branch on the repository
  7)  Go to Github and make a pull request to the master branch
        - Code review will be done and once confirmed it works will be accepted to be master
