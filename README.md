**CONCEPTS OF GIT VERSION CONTROL SYSTEM AND IMPORTANT COMMANDS:**

**WHAT IS GIT:** "Git is a distributed version control system that enables developers to collaboratively manage and track changes to source code. 
It allows developers to efficiently collect, maintain, and manage different versions of code in a decentralized manner. Through Git, teams can work 
together seamlessly, tracking changes, merging contributions, and maintaining a centralized repository of their project's history."

**TYPES OF VERSION CONTROL SYSTEMS:** There are two main types of version control systems: centralized version control systems and distributed version control systems.

**Centralized Version Control System (CVCS):** In a centralized version control system, developers commit and update code to a central repository, such as a remote server, folder, or storage location. This approach offers certain advantages and disadvantages:

**Advantages**:

**Code Accessibility:** All developers can easily access and track the code since it is stored in a central repository.

**Disadvantages**:

 **Internet Dependency:** An active internet connection is required for developers to access the code from the central repository. Without internet access, developers cannot retrieve or update the code.

 **Lack of High Availability:** Since the code is solely stored in a central repository, any issues or downtime with the central repository can prevent developers from accessing the code, leading to disruptions in the development process.

 Overall, while centralized version control systems offer ease of access and collaboration among developers, they are susceptible to internet dependency and potential disruptions due to central repository issues.
 

**Distributed version control system**:

A distributed version control system (DVCS) empowers developers to seamlessly commit, update, push, and pull code between local repositories and central repositories like GitHub. The advantages of using a DVCS are manifold.

**No Dependency on Internet Connection:** With code committed to a local repository, developers can access it readily even in scenarios of limited internet connectivity.

**High Availability:** DVCS ensures High Availability (HAV) by storing code in both local and central repositories. Developers can access code from the local repository if unable to connect to the central repository, ensuring uninterrupted workflow.

**Versioning Capabilities:** DVCS automatically creates distinct versions of code upon each commit. Deleting a version does not affect other versions, providing a robust versioning mechanism for project history and rollback.

**GitHub Integration:** Through push/pull operations, developers synchronize code with central repository like Git-hub. This facilitates collaboration, enabling other developers to track changes and contribute to the project effectively.



**Different Git stages:**
Git has four main stages in its version control workflow:

**Working Directory:** This is where you modify, add, or delete files in your project. These changes are not yet tracked by Git.

**Staging Area (Index):** After making changes in the working directory, you can add them to the staging area using the git add command. Files in this stage are marked as ready to be committed.

**Local Repository:** Once files are staged, you commit them to the local repository using git commit. This creates a snapshot of the project at that moment in time. Commits in the local repository are only visible on your local machine.

**Remote Repository:** This is the centralized repository hosted on a remote server, like GitHub or GitLab. You can push your local commits to the remote repository using git push, and pull changes from the remote repository to your local repository using git pull. This stage enables collaboration with others and serves as a backup of your project.

**Git installation process and important commands:** Git is an open souce software that allows to install on any machines like -Windows, Linux and Mac operating system.

**I am going to discuss the installion process on linux machine of AWS EC2.** 
After lauching the EC2 machine, need to run the sudo su = super user command that allows to get all the permission to perform the entire process.

**Step 1**:

**updating the machine** = **yum update -y** - allows to install any new packages without having any issues.

**installing git** = **yum install git -y** - allows to install git on the linux machine.

**git -- versions** = shows the current version of git is installed on the system.

**Which git** = shows the location where git is installed. 

**git config --global user.name "Maruf"** = allows to track the code has been wriiten by specfic developer -Maruf

**git config --global user.email "xxx"**

**Step 2**:

First of all, create a directory by follwing command = **mkdir Devops**

Get inside of the deirectory = **cd Devops/** and varify the current location using = **Pwd** command

Run = **git init** command allows to convert the directory into a local repository where we commit the code

Create a file inside of the directory by follwing command = **vi git file.txt** allows to create a file and also can put the content/code at a same time.

**git status** = shows the untrack/track/file is available in the working directory or after commiting the code the working directory is clean

**git add .** = After writting the code we can frowrd it from working directoty to staging area means -code is ready for commit.

**git commit-m "1st commit"** = Allows to commit the code into a local repo by default master branch.

**git log** = shows the history of the codes have been already commited like- user info, date, commit id etc

**git --oneline** = shows all the commit id one by one.

**git show <commit-id>** = shows the code.

**Step 3**:

Forward the code from local repo to central repo - Github.

Go to the setting under developer setting and generating access token to acces the central repo from local repository.

**git remote add origin <git-url>** = allows to establish a connection between local repo and central repo

**git push origin master** = push the code from local repo to central repo

**git pull origin master** = pull the code from central repo to local repo

user name = "github account"

password = "Access token"

**Other important commands**:

**Git Branch**

Git branch is a very important concept. When we commit any code into a local repository that creates master branch by default but we also can create new branch as well that allows to help developer to make any changes or updating the code without impacting the main code from master branch. In the future, if we satisfy the new changes then merge the new branch with master other wise we also can delete the new branch it's not going to affect the code of master branch. when we create a new branch from master then all the codes are automatically copied to the new branch but any updating code from the new branch is not going to be reflected to the master or other branch until we merge it.

**git branch** = shows the list of the branches are available in the system

**git branch branch1** = allows to create a new branch is = branch1

**git checkout branch1** = allows to checkout from master to get enter into a new branch = branch1

**git branch -d branch1** = delete the branch1

**git merge branch1** = allows to merge the new branch with master













