# These are some common commands & concepts for use with git, and github. #

## Git vs Github ##
  - **Git:** Version Tracking software that lets you maintain and update various ```branches``` of a project before ```commiting``` to 
         a final version to the master branch.
  - **Github:** A company that serves as a central location for various git ```repositories``` Basically a 'dropBox' for coding.
  
### Git ###
 - **```git clone <yourRepoLink>```** - Used to copy or 'clone' a project for editing
    - ***try not to do your work on the master branch, get in the habit of making a new branch for changes.***
    
 - **```git checkout -b <newBranchName>```** - Used to create a new branch off of your current project.
 - **```git status```** - Shows all changes made since last update
 - **```git add <fileName>```** Add a file to the staging area before pushing
 - **```git commit -m 'some Descriptive Message' ```** - commits all the changes made as 'ok' to update the branch with.
    - ***-m is the message flag, it lets you specify a descriptive comment for what the update / commit was for.***
    
 - **```git push origin <branchName>```** - update <branchName> with the changes you just commited.
 
### Github ###
 - **```Fork```** - Basically just a copy of a repository. NOT the same as a clone.
    - in a clone, you have to have 'contributor' status in order to contribute back to the main project.
    - in a fork, you can make changes and then submit a pull request to have your changes reviewed and passed.
 - **```Pull Request```** - Having your code reviewed before it is sent to the branch / Master to update it.
