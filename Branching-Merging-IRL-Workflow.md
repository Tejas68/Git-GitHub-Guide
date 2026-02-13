**3.1 What is a Branch?**



A branch is a separate line of development.

By default, when you create a repository, Git creates one main branch called:



**main**



Think of branches like this:

main  → stable version of project

feature-login → working on login

feature-ui → working on design



**Branches allow you to:**

**Work on features safely**

**Fix bugs without breaking main code**

**Experiment without risk**



**3.2 Why Do We Need Branches?**



Imagine you're building an E-commerce website.

Your main project is live and working.



Now you want to:

Add payment gateway

Redesign UI

Fix a bug



**If you work directly on main:**

 **You might break the project.**

**If you create a branch:**

 **You work safely.**

 **Main project remains stable.**

 **You merge only when ready.**

**That is professional workflow.**



**3.3 Most Used Branch Commands**

Check Current Branch

git branch

Current branch will have \* symbol.



Create New Branch

git branch feature-login



Switch Branch

git checkout feature-login

OR (modern way):

git switch feature-login



Create and Switch Together

git checkout -b feature-login

OR

git switch -c feature-login



**3.4 Merging Branches**



After completing work in feature branch:



Step 1 – Go back to main

git switch main

Step 2 – Merge

git merge feature-login

Now your feature is added to main branch.



**3.5 Understanding Merge Conflicts**



**Sometimes two branches edit the same line of code.**

**Git cannot decide which change to keep.**



**This is called a Merge Conflict.**

**Example:**

**Main branch:**

**color = blue**

**Feature branch:**

**color = red**

**Git will show conflict.**

**You must:**

**Open file**

**Choose correct version**

**Save**

**Add**

**Commit**

**After fixing conflict:**

**git add .**

**git commit -m "Resolved merge conflict"**

**Conflict solved.**



**3.6 Real-World Professional Workflow**



Most companies follow this workflow:

main → production

develop → testing

feature branches → new features



Example:

feature-login

feature-payment

bugfix-navbar

You create feature branch → complete work → merge into develop → test → merge into main.

**3.7 Working with Branches on GitHub**



After creating branch locally:



Push it:

git push -u origin feature-login

Now branch appears on GitHub.

You can:

Create Pull Request (PR)

Request code review

Merge after approval





**3.8 What is a Pull Request (PR)?**



Pull Request means:

“I want to merge my branch into main. Please review.”

PR allows:

Team discussion

Code review

Suggestions

Approval before merging

It is one of the most important collaboration tools on GitHub.



**3.9 Real-Life Example (Project Simulation)**



**Let’s say you are building:**

**Portfolio Website**

**Day 1:**

**Create main branch → Homepage**

**Day 2:**

**Create feature-about → Add about page**

**Day 3:**

**Create feature-contact → Add contact form**

**Each feature is separate.**

**After testing:**

**Merge all into main.**



**Safe.**

**Clean.**

**Professional.**

