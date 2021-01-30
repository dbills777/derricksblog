---
templateKey: blog-post
title: Blog Post Advanced Git Blog Post
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

What are some advantages and disadvantages of git rebase? (At least 2 of each)

* When shouldn't you use git rebase? Why?

Create a new repo and demonstrate your knowledge of the following items with screenshots:

* A rebase merge
* An interactive rebase merge
* When you shouldn't rebase with a remote repo.

### git reset, checkout, and revert

Answer the following questions:

* What is git reset?
* * What is the difference between hard, mixed and soft?
* What is git checkout?
* What is git revert?
* In what ways are these commands the same and what ways are they different?
* When would you use reset, checkout, or revert? Why?

Create a new repo and demonstrate your knowledge of the following items with screenshots:

* a git reset
* a get checkout
* * a commit
  * a file
* a get revert

### git submodules

Answer the following questions:

* What are git submodules?
* When would you use a submodule?
* What are the advantages and disadvantages of git submodules?

Please be complete and clear when answering the above questions.