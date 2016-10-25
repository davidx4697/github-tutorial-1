# GitHub Tutorial

_by Xinyan Chen_

---
## Git vs. GitHub
**1. Explain what each is**  
* Git is a version control that helps take snapshots of the code or different versions of the file.  
* Github helps store code in the cloud which makes it easier to collaborate on files and help visually track changes made to the code.  

**2. Explain the differences between the two**  
* The differences between Git and Github is that Git takes snapshots of the code and doesn't require Github, however, Github stores the codes in the "cloud" and require Git.  

---
## Initial Setup
**1. Explain how to make a GitHub account**  
* Go to [github.com](github.com)  
![](githublink.png)  
* Click **Sign up** to create a account  
![](signup.png)  
* Include your personal informations  
    * Type in your username  
    * Type in your email address  
    * Type in your a password  
![](addpersonalinfo.png)
* Click **Create an account**  
![](createanaccount.png)  
* Select **Free** account type  
![](free.png)  
* Click **Finish sign up**  

**2. Explain SSH key setup**
* Go to [github.com](github.com)  
![](githublink.png)  
* Click profile icon at the top-right  
![](profileicon.png)  
* Click **Setting**  
![](setting.png)  
* Click **SSH and GPG keys** at the left sidebar  
![](SSH&GPG.png)  
* Press **New SSH key**  
![](newSSH.png)  
* Type in _cloud9_ for **Title**  
* Open a new tab to [cloud9](c9.io)  
![](c9.png)  
* Sign in with your gitHub account  
* Click the gear icon at the top-right  
![](gear.png)  
* Go to **SSH keys** and copy and paste your SSH key into GitHub  
![](SSHkey.png)  
    * Key starts with `ssh-rsa`  
![](exSSH.png)  
* Add SSH key  
* Open github-learning IDE in [cloud9](c9.io)  
![](IDE.png)  
* Type in `ssh -T git@github.com`  

---
## Repository Setup
**1. How to create a repository**  
* Go to [cloud9](c9.io)  
![](c9.png)  
* Sign in with GitHub account  
* Open github-learning IDE in [cloud9](c9.io)  
![](IDE.png)  
* Change to workspace by typing in `cd ~/workspace` into the terminal  
* Make a new directory by typing in `mkdir first-repo` into the terminal  
* Change into first-repo by typing in `cd first-repo` into the terminal  
* Inside the first-repo type in `git init` into the terminal  
* Create a README file by typing in `touch README.md` into the terminal  
* Open README file by typing in `c9 README.md` into the terminal  
* Type in any message(s) into README file  
* Save the message(s) by pressing the keys _control_ and _z_  
* Add the message(s) into the repo by typing in `git add README.md` into the terminal  
* Take a screenshot of the message(s) by typing in `git commit -m ""` into the terminal  
    * Note: Type in a good message that helps you understand the change(s) made in README file  
* Open a new tab to [github.com](github.com)  
![](githublink.png)  
* Sign in with GitHub account  
* Press the plus icon  
![](plus.PNG)  
* Click on **New Repository**  
![](newrepo.PNG)  
* Type in _first-repo_ in **Repository name**  
![](repotitle.PNG)  
* Press **Create repository**  
![](createrepo.PNG) 
* Press **SSH** on the top and copy and paste `git remote add origin git@github.com:username/first-repo.git` and `git push -u origin master` one at a time into the terminal in git-learning IDE  
![](repopush.PNG)  
* Refresh the page to see changes  

---
## Workflow & Commands
**1. Workflow of Commands**  
* `git status`  
* `git add file.txt`  
* `git status`  
* `git commit -m "message"`  
* `git push`  

**2. Status**  
* `git status`  
* Helps check which file(s) have been edited since last commit  
**3. Add**  
* `git add file.txt`  
* Add file to the stage being committed  
**4. Commit**  
* `git commit -m "message"`  
* Takes “Snapshot” of files. The message(s) have to be in present-tense and it describes what is being modified.  
**5. Push**  
* `git push`  
* Update file folder  
    * Note: Can only push after commit  