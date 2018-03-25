# Women++

## Introduction to Mobile Development
### April 2018

---

### What You Need:

* A machine with [Android Studio](https://developer.android.com/studio/index.html) installed
* [Git](https://git-scm.com/downloads) installed
* Android SDK for 6.0 (Marshmallow and above)
* *Some* knowledge of Java and git
* A bit of XML
* An Android phone (useful, but not essential)

--- 

### Disclaimer(s)

1. I have no idea what I am talking about. Stop me at any time with questions.
2. This is far from an `All you can eat` introduction; I will include links for more detail on some topics, though.

---

### Today's Outline*

1. Git
2. Brief Android Introduction
	* Versions
	* Notable changes
	* Activities and Intents
	* APIs
3. Using git with these exercises
4. Structure of an app
5. Practical time

*Subject to change!

---

## Git. What?

A version control system that allows you to store versions of your code and back them up.

You may have already heard of/used Git....bear with me.

If you haven't, Git is a vital part of modern software development and a crucial skill.

We will be using it throughout this workshop.

---

## Git. How?

Git works by storing a local copy of your work (called a `repository`) on your machine and you make a `commit` when you want to save your work. 

You can have a remote repository (like `Github.com`) and `push` these local changes to the remote repo as a backup.

---

## Git Basics. Example

* `mkdir git_test && cd git_test` - Create a folder 
* `git init` - Initialise a repository on your machine
* `git add <files>` - Add files for your first commit
* `git commit -m '<commit message>'` - Commit these changes to your local repository.

--- 

## Git Basics. Pushing to the remote.

* Sign up for an account / sign in at [Github](github.com)
* Click `New Repo`and give it a name
* In your terminal, enter: `git remote add origin <git_url>`
* Now, you can do `git push origin master`
	* This will push your code to Github, go check it out! 	


---

## Git Basics. Cloning.

Cloning a `repository` is downloading a remote repository to your machine.

`git clone <GIT URL>`

NOTE: If you clone a repository and make changes to it. You can commit, but these changes will be made on the remote repository!


---

## Git Basics. Forking.

If you want to make changes to the repository, then you can `fork` instead of `clone`. 

1. Go to a repository on Github.
2. Click the `Fork` button in the top right.
3. This will make a copy of the `repo` in your Github profile.
4. `Clone` the repo to your local machine.
5. Now you can make changes to the code.

---

## Exercise 1


1. Open a terminal and `cd` to a directory of your choice
2. Go to https://github.com/encima/git-test-repo
3. Click `fork` and copy the URL from the page
4. In the terminal, run: `git clone <URL>`
5. Create a file, call it `intro.txt` and add some text
6. Add the file to a commit `git add intro.txt`
7. `git commit -m <YOUR MESSAGE>`
8. `git push origin master`

---

## Git Basics. Branching.

OK, we have covered the basics of Git, but we need to know one more thing about Git: **Branches**

The `master` branch is the default branch when you create or clone a repository.

---

## Git Basics. Branching


Each step in the exercises we do will be on a different branch. A branch is a different copy of the local repository (i.e. different functionality, separate files, different environments).

We use branches in development projects to make sure the `master` branch can be used in production and we can add features safely to a different branch.

---

## Git Basics. Managing Branches

* `git checkout -b <BRANCH_NAME>` - If the branch does not yet exist
* `git checkout <BRANCH_NAME>` - If the branch already exists
* `git branch --all` - View all branches
* `git branch -d <BRANCH_NAME>` - Delete a branch
* `git merge <BRANCH_NAME>` - Merge the branch you name into the current branch you are one.

---

## Exercise 2

1. `cd` to the git-test-repo
2. `git checkout ex2`
3. View the README file and follow the steps

---

# Git

That covers what we need to know for this workshop, but there is **much** more to Git and it is a super powerful tool.

*DISCLAIMER:*
We have only covered the basics of each of these topics and there is more to know for every command we have learnt. We do not expect you to be experts and definitely ask if you have any problems!

---

# Let's Begin!

![andy](https://media.giphy.com/media/Xmz6AD5s92Re8/giphy.gif)

---

# Android. What?

* Developed by Google
* Released with version  1.5 (Cupcake)
* Currently on Oreo
* Now supports Phones, TVs, Watches, Tablets, Fridges

---

## Then and Now
<img src="https://upload.wikimedia.org/wikipedia/commons/2/26/Android_Cupcake_home_screen.jpg" width="200"/>
<img src= "https://icdn5.digitaltrends.com/image/screenshot_20170821-182305-1-720x720.jpg" width="200" />

---

## Versions

* All food based (not all versions means a new number)
* Cupcake (1.5)
* Donut (1.6)
* Eclair (2.0)
* Froyo (2.2)
* Gingerbread (2.3)
* Honeycomb (3.0)

---

## Notable changes

* Security
* Installation of apps
* Google Services
* Sharing of data
* App Design
* Android Studio

---

## Activities

Every screen in Android is an intent. This is mostly true.
For the purpose of this exercise, we will look at `Activities` first and then how these have changed over the years.

An `Activity` is made up of:
1. A `Java` file
2. An `XML` layout file

---

## Layout

---

## Learning Goals

The aim of these hours is to learn primarily through doing. Some downsides of this are:
* We may not go deep enough into the theory (it is important you call out when something should be explained)
* Draining (tell me when you want breaks)
* Overwhelming (this is the first time this has been done so do not expect to finish, just have fun with it)

---

## Workshop Structure

1. Checkout the git repo
`git clone https://github.com/encima/WomenPlusPlus-Android-Workshop`
2. Checkout the `step_one` branch (if you are not on it)
3. Open the presentation for each branch (link in each README):
[Gitpitch](https://gitpitch.com/encima/womenplusplus-android-workshop/step_one)
4. Open Android Studio and open the project (install any packages it asks for)
5. Click the `TODO` button at the bottom left of Android Studio
6. Click on each `TODO` and complete the task
7. When all is done, checkout the next branch
`git checkout step_two`
8. Can't do it? Ask a mentor or move on to the next branch to see the answers
9. Love Android for more than just the cute mascot
10. Profit?

