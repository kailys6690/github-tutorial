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
![homepage&icon](https://raw.githubusercontent.com/kailys6690/github-tutorial/master/octocat.jpg)
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
To make our first repository, we start by going to the root of our workspace.
**Make sure you are not in `~ $ `! you need to be into `~/workspace $`!**  
Now you make your first directory by using the command `mkdir directoryname`. Once you have made your directory, use the command `cd directoryname` to go into the directory you have made. This step is completely **important** because we are going to use the command `git init` for that specific directory you have made. If you don't `cd` into that directory and instead you use `git init` right away, you will make your workspace as a repository and we do **not** want that. 

Once you have initialized your repository (you will know if you see `(master) $ ` in your command line) , you can start adding and commiting edits/changes on the files you have made in that repo. This will be your first **add** and **commit!** But how can we push our new changes into the cloud? We need to connect your new repository to your **remote repo** that lives in the clouds.  

In order to connect your new repository to your **remote repo** that will live on GitHub. Here are the steps you need to take:

1. Go to the top right corner of your homepage and click the "+" sign.
2. A dropdown menue will appear and you will want to click "New Repository"
3. You will appear in a new page and you will see "Create a new repository." Under "Repostory name", you will want to type in your repository name.  
This **_must_** _always_ match your repository name that you have in **Cloud9!** 
4. Then click the big button that says "Create New Repository"
5. A new page will load with the name of your repositry name. This is your repository page. Now in the "Quick setup" section, you will see two buttons that say "HTTPS" next to "SSH". Make sure you click on the "SSH" button. (this is because we made an SSH key in the beginning)
6. Now in the "…or push an existing repository from the command line" section, copy and paste (one at a time) into the command line in you Cloud 9 account. It will look something like this:  
![ExamplePicture](https://raw.githubusercontent.com/kailys6690/github-tutorial/master/example_of_ssh.png)  

Copy and paste these two codes (not these examples above, the ones you have) into your cloud9 account.    
After you have pasted both of commands into the command line, you have now officially connected your cloud9 account with github!  
You can now use the command `git push` without having to use the whole comand `git push -u origin master`.


---
## Workflow & Commands
These are *the most* important steps to remember because you will **ALWAYS** be using these commands:

1. `git status`
2. `git add`
3. `git status` *(optional)*
4. `git commit -m "put what changes you have made in this commit"` 
5. `git push` (only _if_ you have a remote repo)

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
