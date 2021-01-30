---
templateKey: blog-post
title: Advanced Git Blog Post
date: 2021-01-30T18:10:32.834Z
description: _____________________________
featuredpost: false
featuredimage: /img/gitlogo.png
tags:
  - Blog#2
---
* ![code](/img/gitlogo.png "code")

  This assignment combines a blog post with an assignment and will require you to take screen shots to demonstrate your knowledge. The git features covered in this assignment can be hard to check. For the screenshots to count, you need to include something specific to you. This can be the name of your repo and/or files, or another window that you have shown to be unique to you.

  ### git rebase

  Answer the following questions:

  * What is git rebase?

  Git rebase is the action of changing where a given branch originated from. If you start with 2 initial commits on the MAIN branch, and create a new branch FEATURE1, you currently have 3 bases in your repository. FEATURE1 is "Based" on the second MAIN branch commit. 

  ![main](/img/2commitsmain.png "main")

  ![feature](/img/feature-3commts.png "feature")

Now switching back to the MAIN branch and creating 3 more commits on MAIN, leaves the FEATURE1 branch connected to the second MAIN commit as its base. Meaning FEATURE1 contains only the changes from main up to the second commit, its head is now at 5 commits. 

Switching back to FEATURE1 and creating 3 more commits on it, exactly like on the main branch leaves, two branches with separate commits that are unaware of each other. 

Rebasing the FEATURE1 branch on the current MAIN branch will change the location of the initial branch to the current HEAD of MAIN allowing us to keep a clean history of all the changes made to MAIN while FEATURE1 was Branched off of it, creating a straight line continuous history for this example project.

git merge feature while on the MAIN branch will create a fast forward, of main bringing it up to speed with the FEATURE1 branch. And at this point all the commits made one FEATURE will be included in the main branch history. 

* A rebase merge

![merge](/img/gitmergefeature.png "merge")

![history](/img/mainhistory1.png "history")

What are some advantages and disadvantages of git rebase? (At least 2 of each)

* When shouldn't you use git rebase? Why?

Create a new repo and demonstrate your knowledge of the following items with screenshots:

* An interactive rebase merge

  ![int](/img/interactivemerge.png "int")
* When you shouldn't rebase with a remote repo.

  If you wish to keep the branch commits based on a specific reference commit, you would not want to use rebase. Doing so would change the anchor point of your branch and could cause confusion if the history to that point is heavily relied upon.

### git reset, checkout, and revert

Answer the following questions:

* What is git reset?

  GIT RESET is a command used to move the currently selected head to a different commit. It does pose a danger of abandoning commits that may be lost forever and should be used with caution. It resets the head in a way that commits made after the selected commit are left behind for later cleanup by the garbage collector.
* * What is the difference between hard, mixed and soft?

    HARD- Resets all three areas of the repo, Working Directory, Staging Area & Commit History. 

    MIXED- Resets the Staging Area & Commit History. Used as the default in git.

    SOFT- Resets only the Commit history. Great option if you commit by mistake and need to undo the commit.
* What is git checkout?

  CHECKOUT is used to move the HEAD of your project to a new branch or even a specific commit. 
* What is git revert?

  GIT REVERT  Moves your repo forward while at the same time undoing a previous commits commit. Is used to undo changes made under a specific commit. 
* In what ways are these commands the same and what ways are they different?

  They all work with specific commits in mind, Moving, resetting and rolling back of a specific commit made to a repo. 
* When would you use reset, checkout, or revert? Why?

  reset case: Great option if you commit by mistake and need to undo the commit.

  checkout case: Great option if you need to take a peek at a specific repo state, like a feature branch.

  revert case: If you make a change and commit that change and later decide the change is not needed you can revert that commit and ignore the changes that were made in it. This method retains the commits that were made after the reverted commit.

  CHECKOUT-

  If you wanted to see the state at a given time (commit) checkout is useful.

  If you want to create a branch at a specific commit checkout can do that.

  If you need to switch branches checkout can do that. 

Create a new repo and demonstrate your knowledge of the following items with screenshots:

* a git reset: 

  ```
  git reset --soft HEAD~1
  ```
* ![reset](/img/gitreset.png "reset")
* a get checkout
* * a commit

    ![checkout commit](/img/checkout.png "checkoutcommit")
  * a file
* a git revert

### git submodules

Answer the following questions:

* What are git submodules?
* When would you use a submodule?
* What are the advantages and disadvantages of git submodules?

Please be complete and clear when answering the above questions.