---
title: 'Class 1: Course Introduction | Git Overview | IDE'
separator: '\-\-\-\-\-'
verticalSeparator: '\+\+\+\+\+'
theme: 'moon'
revealOptions:
    transition: 'fade'
---

### ITSE-1402 Intermediate Python
<span style="font-family:Helvetica Neue; font-weight:bold; color:#e49436">Class 1: Course Introduction | Git Overview | IDE</span>
<br /><br />
##### [https://itse-1402.github.io/class1-slides](https://itse-1402.github.io/class1-slides)
##### Short Link: [https://bit.ly/1402-class1](https://bit.ly/1402-class1)

-----

## Introductions

+++++

### Instructor

![Image](./assets/philip.jpg)

Philip Ulrich

[philip.ulrich@austincc.edu](mailto:philip.ulrich@austincc.edu)

[https://www.telegram.me/PhilipUlrich](https://www.telegram.me/PhilipUlrich)

Note:
Education:
- BS, Information Technology; Minor in Computer Science

Occupation: 
- Cloud Engineer @ Rackspace

Experience: 
- Programming as a hobbyist for over 9 years using a mixture of Bash, Java, PHP, Powershell, Python, Swift, VB Basic, and a little bit of Javascript.
- Currently a developer on multiple internal tooling projects at Rackspace.

+++++

### Student Introductions
<br />
Ideas:
- Name
- Occupation
- Experience with Programming
- Did you attend Introduction to Python?
- What do you hope to learn from this class?
- What do you hope to do with it afterwards?

Note:
Any and all of these are optional. At the very least, just tell us your name. 

-----

## Attendance

-----

## Syllabus

+++++

[https://itse-1402.github.io/syllabus/](https://itse-1402.github.io/syllabus/)

Short Link: [https://bit.ly/1402-syllabus](https://bit.ly/1402-syllabus)

-----

## Course Resources

+++++

### Course Resources
- GitHub
- Cloud9 IDE

+++++

#### GitHub
<br />
Website: [https://github.com](https://github.com)
<br /><br />
Login: You can either use your existing GitHub username or a new one. If you are using a new one, please go through the account sign up process as you normally would.

+++++

#### GitHub
<br />
Purpose:
- Code repository for the class. Class files will be cloned from here into your workspaces in Cloud9. 
- You will treat assignments/projects as if they were projects you are maintaining on GitHub. All assignments and projects will be submitted via GitHub.

NOTE: Any material assigned/turned in is private by default. Any repos you make also can be private as well. Personal GitHub accounts are okay for use in this course. 

+++++

#### Cloud9 IDE
<br />
<small>Website: https://aws.amazon.com/cloud9/</small>
<br /><br />
Purpose:
<small>

- Primary working environment for the class. We will create a workspace for each class session.
- Class files will be cloned from GitHub to a C9 workspace. From here, you will work your assignments and push changes to your GH repo. Assignments will be graded based on repository contents.

</small>
Login: 
<small>

This login will be provided to you on the first day.

</small>

+++++

#### Creating Cloud9 Environment
<small>

- Log into AWS Console
- Ensure you are in the proper region in the top right corner (typically N. Virginia - us-east-1)
- Click "Services" on the top left and type "Cloud9" and click on link
- Click "Shared with you" and open your workspace
- Click "AWS Cloud9" at the top left and click "Preferences"
- Go to "Python Support" and change "Python Version" to Python 3
- [optional] Go to "Themes" and change it to a less hideous color scheme
- [optional] Go to "Experimental" and enable auto save on focus change. 

</small>

+++++

##### Importing Your First Repo
<small>

- In the terminal at the bottom, run the following command to generate a ssh key: `ssh-keygen` and press enter 3 times
- Then run the following command to get your public signature: `cat ~/.ssh/id_rsa.pub`
- Copy this and past it into your keys on GitHub (Settings -> SSH and GPG keys -> New SSH key)
- Grab the assignment from the following link: [https://bit.ly/1402-example](https://bit.ly/1402-example)
- With your workspace open, clone the repository into your workspace directory with the terminal at the bottom
    - Hint: `git clone git@github.com:ITSE-1402/example-repo-myusername`
- Open the folder "example-repo-myusername" on the left side and open the "README.md" file.
- Click "Preview" in the menu bar then "Live Preview File (README.md)"
- Follow the instructions. 

</small>

-----

## Git

+++++

#### Git
- What is version control? 
- What is Git?
- What is GitHub?
- Using Git day-to-day
- Collaborating online with Github

-----

## What is version control?

+++++

![Image](./assets/version_control.jpg)
<br />
<small>via [Geek and Poke](https://geek-and-poke.com/)</small>

+++++

- It’s a time machine for files
- Checkpoints through a project
- Also known as revision control

+++++

#### Used For:
- Types of Files
  - Text-Based Files (scripts, configs, etc.)
  - Binary Files (with exceptions)
  - Images (with exceptions)
- Files Shared With Others
  - Keeps Track of Who Did What
  - Allows Reverting to Previous Versions
- Code Deployment (Or Any Deployment)
  - Ensures the Correct Version is Deployed

+++++

![Image](./assets/version_control2.jpg)
<br />
<small>via [Tower](https://www.git-tower.com/learn/git/ebook/en/command-line/basics/what-is-version-control)</small>

-----

## What is Git?

+++++

Definition from the Internet: 

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

+++++

#### Installing Git

- Git is available for all the major OSes
  - Linux, Windows, OS X
- https://git-scm.com/downloads

* git will already be installed in our workspaces

+++++

#### What is a Repository?

- A repository is the place that stores all the data for your version controlled directory.
  - More or less, it is the database for all the versions, metadata, file contents, etc.
- A repository can live on a local machine, cloud server, or really any computer. 
- Repositories can be cloned and shared

-----

## What is GitHub?

+++++

#### Definition from the Internet: 

GitHub is a web-based Git or version control repository and Internet hosting service. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features.

+++++

- GitHub is a web-based Git repository hosting service
  - Centralized repository

- Social coding features
  - Pull request
  - Documentation (markdown)
  - Wikis
  - Issue tracking
  - Small websites
  - History browsing
  - Code reviews

-----

## Using Git Day-to-Day (Part 1)

+++++

#### Git Commands:

- git init: Create repository
  - Ex: git init .

- git add: add file(s) to commit
  - Ex: git add text-file.txt image.png

- git commit: commit changes that were added
  - Ex: git commit -m “a comment about things”

- git push: push changes to remote (github, gitlab, etc)
  - Ex: git push

+++++

#### Git Commands (cont.):

- git fetch: grab latest changes from origin/master
  - Ex: git fetch<br />(You likely won’t be using this from the get-go)

- git pull: essentially does a git fetch and git merge
  - Ex: git pull<br />More likely to be used. Updates local branch.

- git status: tells current status of the repo
  - Ex: git status

+++++

#### Git Commands (cont.):

- git rm: removes file(s) from the repo
  - Ex: git rm text-file.txt image.png

- git reset: removes a file added (git add) before commit
  - Ex: git reset other-file.txt

- git checkout -- changed-file.txt
  - Reverts all edits to a specific file

+++++

![Image](./assets/git_transport.png)
<br />
<small>via [Oliver Steele Blog](https://blog.osteele.com/2008/05/my-git-workflow/)</small>

-----

## Lab 1

[https://bit.ly/1402-git](https://bit.ly/1402-git)

Note:
Create this repo and clone it into your workspace. All 3 labs are in this repo. We will just be completing Lab 1 for now. To view lab, open file in C9 and click "Preview" -> "Preview File 'lab1.md'". 

-----

## Using Git Day-to-Day (Part 2)

+++++

Versioning isn’t always smooth sailing...
<br />
![Image](./assets/merge_conflict.png)
<br />
It also isn’t always linear.

Note:
We'll now be hittng some more intermediate concepts that you may end up seeing/encountering when working in git.

+++++

#### Intermediate Git Concepts

- Branching
- Conflicts
- Merging

+++++

#### Branches

A git branch is a separate line of development from the master branch and other branches. 

Branches are typically used for different features or versions of the content being developed. 

+++++

![image](./assets/git_workflow.png)
<br />
<small>via [Leanpub](https://leanpub.com/git-flow/read)</small>

Note:
The master branch is special and is regarded as the current state of the repository.

It is considered the core branch that changes are merged into.

Branches are not strictly required to be merged into the master.

While the master branch is considered special and the current state of the repo, git sees it as any other branch. 

+++++

#### Conflicts

- A merge conflict happens when you to merge conflicting changes between branches.
  - Example: in your README file
    - master: Hello, cat!
    - alice/master: Hello, dog!
  - Git can't tell which one it should go with, so it tells you to pick
- Git trys to resolve as many conflicts as possible without interaction, but with the above example there is no clear solution.

+++++

#### Git Commands:

- git branch: Create branch
  - Ex: git branch my_branch

- git checkout: switch to a branch
  - Ex: git checkout my_branch

- git checkout -b: shortcut to create and switch
  - Ex: git checkout -b my_branch

+++++

#### Merging

Merging branches is when you take the changes from one branch and put them in another. 

Example:
- git checkout master
- git merge my_branch

-----

## Lab 2

-----

## Lab 3

-----

## Cheat Sheet

-----

All extra credit should be submitted to the following repo:

[https://bit.ly/1402-ec](https://bit.ly/1402-ec)