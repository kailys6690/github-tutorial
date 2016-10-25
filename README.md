# GitHub Tutorial

_by Kaily Sanchez_

---
## Git vs. GitHub
What is **Git**?  
Git is a version control that takes "screenshots" of your code. Git is run throught locally and through the commad line. It is important because it helps you keep track of different versions of your work. 

What is **GitHub**?  
GitHub is used to save your code into the "cloud." They visually track the changes you have made and are easy to collabortae on files. 

What is the difference between **Git** and **GitHub**?

* Git runs locally, unlike GitHub which runs in the clouds.
*  Git doesn't require GitHub, but GitHub does require Git.
  

---
## Initial Setup
**Making a new GitHub Account**  
This is required if you want to connect your C9 account (Cloud 9) with your GitHub account.  
Here are the steps you need to take to make your **Github account** & **SSH key**: 

1. You first sign up for a GitHub account by going to [GitHub](https://github.com/).
2. After you have made your account, go to your homepage (by clicking the octocat logo on the top-left corner) and at the top-right corner of the page you will see your profile icon. Click on it.
3. A dropdown menue will appear. Go to your settings.
4. On the left sidebar, find :SSH and GPS keys" and click on it.
5. You will want to create a New SSH Key that will appear on the SSH keys tab on the right corner
6. Give it a title then click the big green button that says "Add SSH key" once you're done.  

Now that you have made your SSH key, you will want to open your C9 account that is on the [C9 website](https://c9.io/)

1. Log into your c9 account
2. On the top-right corner, click the gear icon
3. On the left side bar, click on the "SSH Keys" tab
4. Copy your SSH key that is in the big grey box 
5. Paste your SSH key into GitHub
* starts with ssh-rsa
6. Then add your SSH key
7. Go back to Cloud9 and open up your workspace. Then enter your ssh key into the command line

Once you have entered your ssh key into the command line, you will finally have your Cloud9 and GitHub connected

---
## Repository Setup
How do you set up your own repo(sitory)?  
To make a repository, you need to turn a directory you specify to that repository. We use a command called `git init`.

`git init` is used to initialize git in our directory (that is now a repository) for version control. You can only use this code only **once!**  
Once you have initialized your repository, now you can start adding and commiting edits/changes on the files you have made in that repo. This will be yout first **add** and **commit!*  

But now we have to connect your new repository to your **remote repo** that will live on GitHub. Here are the steps you need to take:

1. Go to the top right corner of your homepage and click the "+" sign.
2. A dropdown menue will appear and you will want to click "New Repository"
3. You will appear in a new page and you will see "Create a new repository." Under "Repostory name", you will want to type in your repository name.  
This **_must_** _always_ match your repository name that you have in **Cloud9!** 
4.






---
## Workflow & Commands
These are *the most* important steps to remember because you will **ALWAYS** be using these commands:

1. `git status`
2. `git add`
3. `git status` *(optional)*
4. `git commit -m ""` 
5. `git push` (only _if_ you have )

The commands above are in workflow order. You *__cannot__* use these commands randomly or you will run into many errors. 

`git status` is used to check any changes/ edits made in the working directory. This command can be used as many times as you want and it very helpful.  
Use `git status` often! It can help you if you run into a probelm when you are using the workflow.  
_hint_: to know if your recent edits have been made, they will be in **_red_**!

`git add` is used to add file(s) to the staging area. This doesnt mean it's been fully saved! It has to be commited so the file is pushed to the staging area, waiting to be fully commited.

`git status` is completely optional to use again, but I totally recommend it because you can never underetimate `git status`!  
This is especially helpful to use after adding file(s) because you may never know if you fully added the file to the staging area. This can also check what file(s) you have added to the staging area.  
_hint_: to know if your files are staged for the commit, they will be in **_green_**!

`git commit -m ""` is the last step of the workflow and the most important. This command takes a 'snapshot' of the file(s) you have added and fully commits them into the . Otherwords, it is saving the changes you have made **permantely**. `-m ""` should be used as a message to describe what is being modified. 

`git push` is used after git commit to send all your recent commits that have been made from our local repo to the remote repo(sitory) (up to the clouds: GitHub) that lives on GitHub. In otherwords, we are sending our commits from Git to GitHub.  
**BUT** in order to use the command `git push`, you need to make sure that you do have a **remote repo** which allows us to push our changes up to the cloud.

---
### Error Handlings