# kottans-frontend

Front-End Course. Contents
Stage 0. Self-Study
A preparatory stage of the Front-End Course. Following tasks should be completed to join main course.

General
Git Basics

Linux CLI and Networking

VCS (hello gitty), GitHub and Collaboration

Front-End Basics
Intro to HTML & CSS

Responsive Web Design

HTML & CSS Practice

JavaScript Basics

Document Object Model - practice

Advanced Topics
Building a Tiny JS World (pre-OOP) - practice

Object oriented JS - practice

OOP exercise - practice

Offline Web Applications - optional

Memory pair game — real project!

Website Performance Optimization - optional

Friends App - real project!

0 Git intro
Finish the course Version Control with Git
I've already worked with git locally, so this topic is not someting brand new to me. Though, I liked the way the material is performed in this course, it seems well-structured and covers the very first steps for exploring version control system.

Udacity screenshot

Complete the following levels at learngitbranching.js.org:
I've discovered a rebase command: it is used when we want to make it look like two features were developed sequentially in one branch, when in reality they were developed in parallel in different branches.

Main: Introduction Sequence

Practicing git remotes while faking a teamwork was all new to me. I've discovered the difference between rebase and merge(creates new commit), uncovered the inner nature of pull (which is fetch combined with merge ). Also I've learned how to solve conflicts with locked master branch. I will definitely use this knowledge in future!

Remote: Push & Pull -- Git Remotes

Send a pull-request to Kottans/mock-repo proposing a change. This was a really cool experience! Sending a pull request was absolutely new to me and now I feel more confident with git.
1 Linux CLI Http
Linux Survival (4 modules)
I've been using cli in Linux ( Ubuntu, if being precisely ) for the last 7 years already. Though, I've discovered some new commands: Here are the basic Linux print commands:

lpr for sending to printer
lpq for displaying print queue
lprm for removing from print queue
and I was surprised, about the finger, which shows the user's info: name, home catalogue, etc.

LS

LS

LS

LS

[] HTTP: The Protocol Every Web Developer Must Know - Part 1

[] HTTP: The Protocol Every Web Developer Must Know - Part 2

2 Git collaboration
This Udacity course makes a great summary and gives advanced explanations to the practice of pull-request, performed at task 0. I've got a great advice, which is wonderfully obvious:

⚠️ Prefer Working Locally ⚠️ Because GitHub has a web interface, it allows you to add commits manually through its interface. But just because you can do a thing, doesn't mean you should. I've demoed making these changes this way so that we could simulate commits being on the remote repository but not in the local repository. But I recommend that you should always work locally on a project and then push those changes to the remote repository.

In addition I'd like to highlight the importance of git fetch:

One main point when you want to use git fetch rather than git pull is if your remote branch and your local branch both have changes that neither of the other ones has. In this case, you want to fetch the remote changes to get them in your local branch and then perform a merge manually. Then you can push that new merge commit back to the remote.

Forking a remote repository (ref Lesson2) was recently cpompleted by me at task 1, when I was aimed to fork the kottans repo and perform some changes. So, I'm sure, this is what I'll be performing for many times in future.

git shortlog was a command that has surprised me — it's really convenient and makes the collaboration easy-peasy. I'll definittely use it if forking a repo. Flags available:

-s to show just the number of commits (rather than each commit's message) -n to sort them numerically (rather than alphabetically by author name).

When to rebase The git rebase command can help you edit commit messages, reorder commits, combine commits, etc.

Whenever you rebase commits, Git will create a new SHA for each commit! To Git, the SHA is the identifier for a commit, so a different identifier means it's a different commit, regardless if the content has changed at all.

So you should not rebase if you have already pushed the commits you want to rebase. If you then use git rebase to change things around and then force push the commits, then the other developers will now be out of sync with the remote repository. They might just have to scrap all of their work and start over with your newly-rebased, force-pushed commits.

GitHub & Collaboration
Main

Complete the following levels at learngitbranching.js.org:
Main: Ramping Up, Moving Work Around
Main

Remote: To Origin and Bey
