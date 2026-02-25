# **Undoing Mistakes, Advanced Commands \& Power Features**





**4.1 Checking History Properly**



Before undoing anything, always check history:

git log



Short version:

git log --oneline



This shows:

a3f5d2 Added login feature

b8e1c9 Fixed navbar

d2a4e1 Initial commit

Each commit has a unique ID (hash).

**4.2 Undoing Changes (Before Commit)**



Case 1 – Modified file but not staged

Discard changes:

git restore filename

Case 2 – Added to staging but not committed

Unstage file:

git restore --staged filename



**4.3 Undoing Commits**



Now we move to serious undo operations.

git reset (Dangerous but Powerful)



Soft Reset (Keep Changes)

**git reset --soft HEAD~1**

Removes last commit but keeps changes staged.



Mixed Reset (Default)

**git reset HEAD~1**

Removes commit and unstages changes.



Hard Reset (Very Dangerous)

**git reset --hard HEAD~1**

Removes commit and deletes changes permanently.

**Never use --hard on shared branches.

4.4 git revert (Safe Way to Undo)**



If you already pushed commit to GitHub, use:

**git revert commitID**





This creates a new commit that reverses changes.

&nbsp;Safe for team projects

&nbsp;Keeps history clean

Professional teams prefer revert instead of reset on shared repositories hosted on GitHub.



**4.5 git stash (Temporary Storage)**



Sometimes you are working on something but need to switch branches.



Instead of committing incomplete work:

**git stash**

Now changes are saved temporarily.

To bring them back:

**git stash pop**

View stash list:

**git stash list**

This is extremely useful in daily development.



**4.6 git rebase (Advanced Concept**)



Rebase changes commit history.



Instead of merging like this:

**main ← merge commit ← feature**

**Rebase makes history cleaner:**

**main → feature commits on top**



Use:

**git rebase main**



Why use rebase?

Clean linear history

&nbsp;Better project visualization

&nbsp;Used in professional workflows

But:

&nbsp;Never rebase public/shared branches.



**4.7 Viewing Differences**



Check what changed:

**git diff**

Compare commits:

**git diff commit1 commit2**

This helps in debugging.


**4.8 Cleaning Up Branches**



Delete local branch:

**git branch -d branch-name**

Force delete:

**git branch -D branch-name**

Delete remote branch:

**git push origin --delete branch-name**





**Real-Life Scenarios**

**Scenario 1:**

**You committed wrong message**

**→ Use git commit --amend**



**Scenario 2:**

**You committed sensitive data (API key)**

**→ Use reset locally**

**→ Remove file**

**→ Recommit**

**→ Push carefully**



**Scenario 3:**

**You pushed broken code**

**→ Use git revert**

**→ Push fix safely**



**Professional Best Practices**

 **Commit small changes**

 **Use meaningful commit messages**

 **Never push broken code**

 **Always pull before pushing**

 **Don’t use --hard carelessly**

 **Use feature branches**

 **Review before merging**

