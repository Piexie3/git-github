## What is Git & Github
- Git - is a free and open-source distributed version control system used for source code management. It is designed to handle small to very large projects with speed and efficiency. Git tracks changes in any set of computer files, enabling multiple developers to work together on non-linear development.
- Github - is a for-profit company that offers a cloud-based Git repository hosting service. Essentially, it makes it a lot easier for individuals and teams to use Git for version control and collaboration.
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
2. Create Github acconunt [here](https://github.com/)
3. Connecting your Github account with Git
- make sure Git is installed 
- Then open your terminal 
 * To set your username:
     ```git config --global user.name "yourUsername"```
    * To confirm your username:
    ```git config --global user.name```
    * To set your email:
     ```git config --global user.email "youremail@gmail.com"```
    * To confirm your email:
     ```git config --global user.email```
4. Creating New repository
* navigate to your project's root directory in your terminal and run:
     ```git init```
5. Add Files to the Repository:
* Adding all your changed files to Git repository using the following command:
     ```git add . ```