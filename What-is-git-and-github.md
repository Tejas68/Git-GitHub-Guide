**1.1 What is Git?**

Git is a Version Control System (VCS).


A Version Control System helps you:


Track changes in files


Go back to previous versions


Work with a team without overwriting each other's work


Manage code history safely


Git was created by Linus Torvalds in 2005 for managing the development of the Linux kernel.


**1.1 What is Git?**

Git is a Version Control System (VCS).

A Version Control System helps you:

Track changes in files

Go back to previous versions

Work with a team without overwriting each other's work

Manage code history safely

Git was created by Linus Torvalds in 2005 for managing the development of the Linux kernel.

**1.3 How Git Works (Core Concept)**

Git works in three main areas:

1. Working Directory

This is your project folder.

2. Staging Area (Index)

This is where you prepare changes before saving.

3. Repository (.git folder)

This stores the full history of your project.

**Simple Flow: Working Directory → Staging Area → Repository**

**Each commit = a saved version of your project.**

**1.4 Installing Git**

**Download & Install Git from** [**https://git-scm.com/**](Git)

Check version after Installing Git:
git --version

First-Time Setup
Git needs your identity:

**git config --global user.name "Your Name"**

git config --global user.email "your@email.com"

Check config:

**git config --list**
**git config user.name**
**git config user.email**


Check Global vs. Local 
Git allows you to have different identities for different projects. 

    Global (System-wide): git config --global user.name
    Local (Current Repo Only): git config --local user.name

For VS Code Users
If you are using Visual Studio Code, you can also check your info via the UI:

    Open the Command Palette (Ctrl+Shift+P or Cmd+Shift+P).
    Type and select "Git: Show User Info"


**Update Your Git Identity**
To change the name and email that appear on future commits, use the git config command.

**To replace the user globally (for all projects)**
git config --global user.name "New Name"
git config --global user.email "new-email@example.com"

**To replace the user only for the current project:**
git config user.name "New Name"
git config user.email "new-email@example.com"

**1.5 use**

Create a folder
mkdir my-project
cd my-project

Initialize Git
git init


**Add Files to Staging**

Add one file:
git add file.txt

Add all files:
git add .

Commit:
git commit -m "Initial commit"

View Commit History:
git log
