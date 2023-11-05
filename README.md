## What is Git & Github
- `Git` - is a free and open-source distributed version control system used for source code management. It is designed to handle small to very large projects with speed and efficiency. Git tracks changes in any set of computer files, enabling multiple developers to work together on non-linear development.
- `Github` - is a for-profit company that offers a cloud-based Git repository hosting service. Essentially, it makes it a lot easier for individuals and teams to use Git for version control and collaboration.
## Difference between Git and Github
No. | Git | Github
| :--- | ---: | :---:
1  | Git is a command-line tool | GitHub is a graphical user interface
2 | Git is a software. | GitHub is a service.
3 | Git is installed locally on the system | GitHub is hosted on the web
4 |Git is maintained by linux. | GitHub is maintained by Microsoft.
5| Git is focused on version control and code sharing. | GitHub is focused on centralized source code hosting.
6| Git has no user management feature. | GitHub has a built-in user management feature.
7|Git has minimal external tool configuration.|GitHub has an active marketplace for tool integration.
8|	Git provides a Desktop interface named Git Gui.| GitHub provides a Desktop interface named GitHub Desktop.
9| Git competes with CVS, Azure DevOps Server, Subversion, Mercurial, etc. | GitHub competes with GitLab, Bit Bucket, AWS Code Commit, etc.

## How to start using Git and GitHub
1. [Download here](https://git-scm.com/download) depending on your Operating System
    * Open your terminal and run the command to confirm if Git was successfully installed.
    ```
    git version
    ```
2. Create Github acconunt [here](https://github.com/)
3. Connecting your Github account with Git
- Open your terminal 
 * To set your username:
     ```
     git config --global user.name "yourUsername"
     ```
    * To confirm your username:
    ```
    git config --global user.name
    ```
    * To set your email:
     ```
     git config --global user.email "youremail@gmail.com"
     ```
    * To confirm your email:
     ```
     git config --global user.email
     ```
4. Creating New repository
* navigate to your project's root directory in your terminal and run:
     ```
     git init
     ```

5. Connect the Remote Repository:
* you can connect your repository with local repository through
     ```
    git remote add origin your_remote_repository_url
    ```
    Example
    ```
    git remote add origin https://github.com/piexie3/git-github
    ```
    
6. Add Files to the Repository:
* Adding all your changed files to Git repository using the following command:
    ```
    git add .
    ```

7. To double-check that your changes have been added:
*  It will show you a list of the files that have been staged
    ```
    git status
    ```

8. Commit the changes to save them to your Git repository:
    * `-m` means message
    ```
    git commit -m "Your commit message"
    ```
9. To show information about specific commit use
    ```
    git show commit_id
    ```
10. To display Commit history, run:
* Note - to exit from command press `q`

    ```
    git log
    ```
11. Push Changes to the Remote Repository
* If you have a remote repository, you can push your local changes to it:
    * The `-u` flag creates a tracking reference for the branch, and `origin main` puts the code in the `main` branch.
    * This command is used to push your local changes to the "master" branch 
    ```
    git push -u origin master
    ```
 * if you want to push to different branch
    
    ```
    git push -u origin your_branch_name
    ```
 * Fetching Updates
    ```
    git fetch
    ```
 * You can also use 
    ```
    git push
    ```

 12. Pull Changes from the Remote Repository:
 * Used to sync with changes made by others in a remote repository:
    * This fetches changes from the remote "master" branch and merges them into your local branch.
        ```
         git pull origin master
        ```
        

 13. To add README to your project, you can run
        ```
        git add Readme.md 
        ```
### Branching
 1. Creating New Branch
    ```
    git branch name_of_your_branch
    ```
 2. Checking list of your branches
    ```
    git branch
    ```
    ```
    git checkout
    ```
 2. Swithching from one branch to another
    ```
    git checkout branch_name
    ```
    * available in Git versions 2.23 and later
    ```
    git switch branch_name
    ```
    * If the branch you are switching to doesn't exist yet, you can create it at the same time by adding the `-b` and `-c` in switch
    ```
    git checkout -b new_branch_name
    ```
    ```
    git switch -c new_branch_name
    ```
 3. Deleting a branch
 * make sure you are not in the branch you want to delete
    ```
    git branch -d branch_name   
    ```
4. Renaming a branch:

    ```
    git branch -m new_branch_name
    ```
5. Merge Branches
* To Merge the specified branch into the current branch.use
    ```
    git merge branch_name
    ```
6. Setting Upstream Branch
    * Sets the upstream branch for the current branch to track a remote branch.
    ```
    git branch --set-upstream-to=origin/branch_name
    ```

### If you like the the content give a :star: and follow