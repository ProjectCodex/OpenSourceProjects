# Welcome to [Project Codex's][1] Open Source FAQ!
[1]: https://github.com/ProjectCodex

### Navigation
  - [So what is Open Source?](#so-what-is-open-source)
  - [What is Git?](#what-is-git)
  - [Where do I download Git?](#where-do-i-download-git)
  - [I Need a Git Walkthrough](#i-need-a-git-walkthrough)
  - [I just need a quick Git Reference](#i-just-need-a-quick-git-reference)
  - [How do I use git on my own projects?](#how-do-i-use-git-on-my-own-projects)
  - [How does Git work with Open Source Projects?](#how-does-git-work-with-open-source-projects)
    - [That was confusing. Can you walk me through that again?](#that-was-confusing-can-you-walk-me-through-that-again)
  - [Where can I practice contributing to Open Source?](#where-can-i-practice-contributing-to-open-source)
---
## So what is Open Source?

From [opensource.com](https://opensource.com/resources/what-open-source):
>The term "open source" refers to something people can modify and share because its design is publicly accessible.
>...Open source software is software with source code that anyone can inspect, modify, and enhance.

Open source projects are a way for people to collaborate on projects without being in the same office, on the same team, or even on the same network. Using version control systems like Git/GitHub, people are able to work on code bases independently and submit their changes for review to be merged in.  

---
## What is Git?

Here's a great intro by The Coding Train: 

[![The Coding Train Explains Git](https://img.youtube.com/vi/BCQHnlnPusY/0.jpg)](https://youtu.be/BCQHnlnPusY)  

---
## Where do I download Git?

Download git/git bash [here](https://git-scm.com/downloads)  
Git Bash is the Linux command line shell that you can use for git. It's awesome, trust us.

---
## I Need a Git Walkthrough

Here's a video by Traversy Media that walks you through some git adding, pushing, pulling, etc.:

[![Traversy Media Walkthrough](https://img.youtube.com/vi/SWYqp7iY_Tc/0.jpg)](https://youtu.be/SWYqp7iY_Tc)

---
## I just need a quick Git Reference

Here's a [Git Cheat Sheet](http://jonas.nitro.dk/git/quick-reference.html)
This covers probably more git commands than you'll need.

And Here's a [Simple Git Guide](http://rogerdudler.github.io/git-guide/)
This guide explains a lot of the commands you'll use 

---
## How do I use git on my own projects?

Definitely check out the resources above for a more in-depth explanation, but once you make a repository and clone it down into a folder, 
just add your files there and work on them, then send the changes up to github with the commands below.

Here's the basic commands you'll use with git:
* `git add .` - add files to track
* `git commit -m "<some message>"` - commit the changes to the files
* `git pull` - pull changes down from the cloud
* `git push` - send your changes up

Those four commands are all you need to work on your own project with git/github. But what about collaborating?

---
## How does Git work with Open Source Projects?

Since you don't own the repo or code in an open source project, how do you contribute? Basically you make a github and local copy of the project, make and test your changes, and then submit them for review.

1. Find a project and `Fork` it.  
At the very top right of this page you'll see a Fork button.  
If you click that, you'll make a copy of the project on your github profile.  
  
1. `Clone` it down.  
You need to clone the project to your local machine.  
Click the "clone or download" button on your repo's homepage and copy the link in the menu.  
Then open git bash in the directory/folder on your machine you want to work in and `git clone <paste the link here>`  
  
1. Set your upstream `remote` to the Main Project's repo.  
Go back to github and repeat the previous step using the original project's repo homepage.  
Don't clone it down again, just copy that link under "clone or download"  
Now on your machine in git bash enter `git remote add upstream <paste the link here>`  
This adds a way for you to pull changes from the source project down to your local machine.  
**This is important because you must assume the source project is constantly changing!**  
  
1. Make whatever changes you want to make then `add` and `commit` them.  
**Don't** `push`.   
`git add .` then `git commit -m "<description of your changes>"`  
**Don't Push yet!**

1. `Pull` down from the original project.  
Type `git pull upstream master`  
This will let you handle any conflicts to the original repo locally on your machine.  
If there's no conflicts, great. Skip to the next step.  
If there are, you'll have to fix those conflicts and then save, `git add .` and `git commit` again.  

1. Now you can `push`.  
Now you need to push your changes to your _forked_ repo.  
You can't send your changes directly to the original project/upstream.  

1. Now submit a pull request!  
Click the "pull request" button on your repo page.  
This lets the original repo owners know that you have made some changes for them to review.  
If they like them, they'll be merged in.  
If not, they may ask you to make some changes, which you can then implement and resubmit.  
  
---
### That was confusing. Can you walk me through that again?

Sure! Here's a video from The Odin Project (a free online web bootcamp) about how the open source process works:

[![The Odin Project Explains Open Source](https://img.youtube.com/vi/mENDYhfxH-o/0.jpg)](https://youtu.be/mENDYhfxH-o)

---

## Where can I practice contributing to Open Source?

You can start by contributing to Project Codex's Open Source Repos! Either fork this repo and help add to this readme or the main readme, or maybe just fix a typo, or sign your name to the credits [here](https://github.com/ProjectCodex/OpenSourceProjects#credits).

There's also some different sites that aggregate beginner-friendly open source projects:
* [First Contributions](https://github.com/Roshanjossey/first-contributions)
* [Up For Grabs](https://up-for-grabs.net/#/)
* [First Timers Only](https://www.firsttimersonly.com/)
* [Your First PR](http://yourfirstpr.github.io/)
* [Awesome For Beginners](https://github.com/MunGell/awesome-for-beginners)
* [freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp/labels/first%20timers%20welcome)

Project Codex is focused on getting its members comfortable with Open Source. Come out to our [meetup](https://www.meetup.com/project-code-experience/) and ask us lots of questions!
