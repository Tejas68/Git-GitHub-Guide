**2.1 What is GitHub?**



GitHub is a cloud platform where we store Git repositories online.



It allows you to:



Backup your code

Share code with others

Collaborate with teams

Contribute to open-source projects

Showcase your portfolio

GitHub was founded in 2008 and later acquired by Microsoft in 2018.



**2.2 Difference Between Git and GitHub**



**Git**

A Version Control System

Works locally on your computer

Tracks file changes

No internet needed



**GitHub**

A cloud hosting platform

Works online

Stores \& shares repositories

Internet required





**Simple explanation:**

**Git = Tool**

**GitHub = Platform**

**You can use Git without GitHub.**

**But GitHub always uses Git.**



**2.3 Why Do We Use GitHub?**



**Imagine:**



You are building a project on your laptop.



Suddenly:

Laptop crashes

Files get deleted

System is stolen



**Without GitHub → You lose everything.**

**With GitHub → Your project is safe in the cloud.**



Also:

Companies use GitHub for:

Team collaboration

Code reviews

Tracking issues

Managing releases



**2.4 Key Concept: Local vs Remote Repository**



Local Repository

Your project on your computer.



Remote Repository

Your project stored on GitHub.



Your workflow becomes:

Your Computer → Git → GitHub



**2.5 Creating Your First GitHub Repository**



Step 1:

Go to GitHub and create an account.

Step 2:

Click New Repository

Fill:

Repository name

Description

Public or Private

Click Create Repository

Now you have an empty remote repository.



**2.6 Connecting Local Project to GitHub**



Inside your project folder:

git remote add origin https://github.com/username/repository-name.git



Check remote:

git remote -v



**2.7 Push – Sending Code to GitHub**



Push your code:

git push -u origin main



What this means:

push → Send changes

origin → Remote name

main → Branch name

Now your project is uploaded to GitHub



**2.8 Pull – Getting Code from GitHub**

If someone else makes changes:

git pull origin main

This downloads updates from GitHub to your local project.



**2.9 Clone – Copy Project from GitHub**

Instead of creating manually, you can clone:

git clone https://github.com/username/repository-name.git

This:



Downloads project

Initializes Git

Connects to remote automatically



**2.10 Most Important Commands (Remote Level)**



Check Remote

git remote -v

Push Changes

git push

Pull Changes

git pull

Clone Repository

git clone <repo-url>

**Real-Life Scenario
Imagine you and your friend are building a project.**

**You:**

**Push homepage feature**

**Friend:**

**Pulls project**

**Adds login feature**

**Pushes changes**

**You:**

**Pull new updates**

**Now both of you are working safely without deleting each other's work.**

**That is collaboration power.**





