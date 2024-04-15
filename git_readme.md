# Version control and Git

### What is version control?

Version control is the tracking and managing of changes made to something over the length of its creation.
This can be a piece of code, software, graphic design etc.

### What is Git?

Git is a open-source version control system. It can be used to track any set of changes in a set of computer files chosen by the user.

* A favourite amongst programmers or devops personnel, it allows them to work collaboratively to manage source code during software
development.
* The main aims for Git are speed and efficiency, data integrity and support for teams working in non-linear development.

### How does Git work?

Git has three main stages. Modify, stage, commit.
* Modify is where the file is being worked on and the changes have been recognised by git, however 
the user does not currently want it on the database.
* Staged is when the user has decided they want to add the file to the git database but have yet to do so. At this
point they can still make changes and edit. Like boarding a plane but you've yet to take off, staged is the file in waiting.
* Commit is takeoff! The file that was staged has now been added to the database. Note that all these steps are occurring
locally on the machine in use.

# Git command flow

The git command flow has a few steps. You are not able to just push files to the database haphazardly.
* git init - is the first step. This command creates a git repository for the unversioned filed being worked on that the user 
wants to start tracking.
* git status - is the second step. This command shows the state of the current directory/folder and the staging are. Displaying
which files aren't being tracked by git, and the changes that have and haven't been staged.
* git add - is the third step. This command adds the changes made to the current working directory/folder to the staging
area. The git add . command will add all changes made to files in the folder and subfolders into staging. Both commands 
do not make any changes to the repository. There is debate as to the usefulness git add, but it is an important step as 
the prequisite to git commit. Without it git commit would not add anything to the repository.
* git commit - is the final step. This command saves all the changes made to the files safely in the local git repository.
The user has to set a message for the commit for the command to be completed. In essence all the changes that were in the
staged area are captured in what is best thought of as a snapshot of the projects current version. These snapshots of 
the project are known as safe versions.

# Git log and Git diff

Two useful commands are git log and git diff. 
* Using git log allows the user to display the commited snapshots. They are 
able to list the project history, filter it, and check for specific changes.

* Using git diff helps the user to see, compare and understand changes in their commits.
The can see code changes between two commits of their choice, or between the current repository and
an earlier commit.

# What is .gitignore? and why we should use it

A very useful process is .gitignore. It is not a command, but a file the user creates. 
* The file tells Git what files in the directory to ignore when committing files in our working directory to the repository. 
* It should be used as it is essential for maintaining privacy and security. Any files containing passwords, 
sensitive information, specific code or generally files the user does not want git to track and to be seen publically.

# Distributed version control


### What is Github?

Github in essence is a cloud based repository. It is a platform where code can be hosted and allows for collaboration and
version control on projects. It works with git, which is the software, to push locally stored repositories to the shared platform on 
the internet, to be seen and worked on by others.

### Alternatives to Github

Github is not the only cloud(online) hosted repository platform. There are options such as GitLab, BitBucket,
AWS CodeCommit and SourceForge, to name a few. GitHub however, is the most popular.

### How do you add a local repo to a remote repo (GitHub)?

There are a few steps involved, but they are simple
* First is the creation of your local repo (see above).
* Second is inputting commands ```git remote add origin```followed by the url destination. 