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

# Basic App Flow
  - User logs into their account
  - User creates a shopping list or opens an existing one
  - Usr adds items via app or alexa
  - User prints wirelessly or saves/shares shopping list
  - User deletes list w/option to automatically delete after sharing
  
# Alexa Integration
  - Create a custom skill
  - Lambda function that executes a Python script to add user/list info to a sqlite database
      - This info is to be accessed through the app to display the data in it live
  - Alexa responds if the item was added/removed successfully or not
  
# Communication
  - Ionic Application and Alexa Device connects to the Sqlite database in order to store/receive data.
  - Ionic Application and Alexa Device needs to be able to connect to a WiFi printer or share the list
  
# Releases
  - Version 1.0.0 Goals
      - Account creation/login
      - Landing page shows lists of shopping lists created by the user (which are stored on database)
          - Allows user to add/remove lists
      - Create List page to get name and other basic info, not items
      - Add Items pages
          - Categorize item pages to keep adding/removing simple and quick
