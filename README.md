My first Readme
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

General
What is source code management
What is Git
What is GitHub
What is the difference between Git and GitHub
How to create a repository
What is a README
How to write good READMEs
How to commit
How to write helpful commit messages
How to push code
How to pull updates
How to create a branch
How to merge branches
How to work as collaborators on a project
Which files should and which files should not appear in your repo
Copyright - Plagiarism
You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
You are not allowed to publish any content of this project.
Any form of plagiarism is strictly forbidden and will result in removal from the program.
Requirements
General
A README.md file at the root of the alx-zero_day repo, containing a description of the repository
A README.md file, at the root of the folder of this project (i.e. 0x03-git), describing what this project is about
Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
Your answer files should only contain the command, and nothing else
More Info
Basic usage
At the end of this project you should be able to reproduce and understand these command lines:

$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
Quiz questions
Great! You've completed the quiz successfully! Keep going! (Show quiz)
Tasks
0. Create and setup your Git and GitHub account
mandatory
Score: 100.0% (Checks completed: 100.0%)
Step 0 - Create an account on GitHub [if you do not have one already]
You will need a GitHub account for all your projects at ALX. If you do not already have a github.com account, you can create an account for free here

Step 1 - Create a Personal Access Token on Github
To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow this tutorial to create a token.

Once it’s created, you should have a token that looks like this:



Step 2 - Update your profile on the Intranet
Update your Intranet profile by adding your Github username here

If it’s not done the Checker won’t be able to correct your work



Step 3 - Create your first repository
Using the graphic interface on the github website, create your first repository.

Name: alx-zero_day
Description: I'm now a ALX Student, this is my first repository as a full-stack engineer
Public repo
No README, .gitignore, or license


Step 4 - Open the sandbox
On the intranet, just under the task, click on the button  and run to start the machine.

Once the container is started, click on  to open a shell where you can start work from.

Step 5 - Clone your repository
On the webterm of the sandbox, do the following:

Clone your repository
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-zero_day.git                  
Cloning into 'alx-zero_day'...
warning: You appear to have cloned an empty repository.       
Replace {YOUR_PERSONAL_TOKEN} with your token from step 1

Replace {YOUR_USERNAME} with your username from step 0 and 1

Pro-Tip: On windows, use CTRL + A + V to paste in the web terminal

Step 6 - Create the README.md and push the modifications
Navigate to this new directory. Tips
root@896cf839cf9a:/# cd alx-zero_day/
root@896cf839cf9a:/alx-zero_day#
Create the file README.md with the content My first readme. Tips
root@896cf839cf9a:/alx-zero_day# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/alx-zero_day# cat README.md                                                                                      
My first readme                                                                                                                       
Update your git identity
root@896cf839cf9a:/alx-pre_course# git config --global user.email "you@example.com"
root@896cf839cf9a:/alx-pre_course# git config --global user.name "Your Name"
Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
root@896cf839cf9a:/alx-zero_day# git add .
root@896cf839cf9a:/alx-zero_day# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/alx-zero_day# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/alx-zero_day.git                                                                                       
 * [new branch]      master -> master              
Good job!

You pushed your first file in your first repository of the first task of your first ALX School project.

Set up Git
In this article
Using Git
Setting up Git
Authenticating with GitHub from Git
Next steps
At the heart of GitHub is an open-source version control system (VCS) called Git. Git is responsible for everything GitHub-related that happens locally on your computer.



**USING GIT**

To use Git on the command line, you will need to download, install, and configure Git on your computer. You can also install GitHub CLI to use GitHub from the command line. For more information, see "About GitHub CLI."

If you want to work with Git locally, but do not want to use the command line, you can download and install the GitHub Desktop client. For more information, see "Installing and configuring GitHub Desktop."

**If you do not need to work with files locally, GitHub lets you complete many Git-related actions directly in the browser, including:
**
Creating a repository
Forking a repository
Managing files
Being social
Setting up Git
Download and install the latest version of Git.

Note: If you are using a Chrome OS device, additional setup is required:

Install a terminal emulator such as Termux from the Google Play Store on your Chrome OS device.
From the terminal emulator that you installed, install Git. For example, in Termux, enter apt install git and then type y when prompted.
Set your username in Git.

Set your commit email address in Git.

Authenticating with GitHub from Git
When you connect to a GitHub repository from Git, you will need to authenticate with GitHub using either HTTPS or SSH.

Note: You can authenticate to GitHub using GitHub CLI, for either HTTP or SSH. For more information, see gh auth login.

Connecting over HTTPS (recommended)
If you clone with HTTPS, you can cache your GitHub credentials in Git using a credential helper. For more information, see "About remote repositories" and "Caching your GitHub credentials in Git."

Connecting over SSH
If you clone with SSH, you must generate SSH keys on each computer you use to push or pull from GitHub. For more information, see "About remote repositories" and "Generating a new SSH key and adding it to the ssh-agent."

Next steps
You now have Git and GitHub all set up. You may now choose to create a repository where you can put your projects. Saving your code in a repository allows you to back up your code and share it around the world.

Creating a repository for your project allows you to store code in GitHub. This provides a backup of your work that you can choose to share with other developers. For more information, see “Create a repository.".

Forking a repository will allow you to make changes to another repository without affecting the original. For more information, see "Fork a repo."

Each repository on GitHub is owned by a person or an organization. You can interact with the people, repositories, and organizations by connecting and following them on GitHub. For more information, see "Be social."

GitHub has a great support community where you can ask for help and talk to people from around the world. Join the conversation on GitHub Community.

You can now check your repository on GitHub to see if everything is good.

Repo:

GitHub repository: alx-zero_day
File: README.md
