---
layout: post
title:  "Getting started with phabricator"
date:   2017-04-13 05:42:38
categories: techteam
---
This has been shamelessly copied from the post written [https://www.facebook.com/notes/abhilash-inumella/moving-to-code-conversations-from-feature-conversations/10153441383084384/](https://www.facebook.com/notes/abhilash-inumella/moving-to-code-conversations-from-feature-conversations/10153441383084384/) by my friend abhilash-inumella

Writing software is at the heart of a consumer internet company like ours. All of the heavy lifting is done by the code we write. But the irony of the current situation is that we're talking very less about the code. To overcome this problem Facebook, Quora, Dropbox, Uber, Pinterest, KhanAcademy internally use [http://phabricator.org/](http://phabricator.org/). It's a tool to communicate code. It's for reviewing code. It's a tool to get the shit done. It's the only review tool I've seen that doesn't suck.

Action items:
```
some_install_path/ $ git clone https://github.com/phacility/libphutil.git
some_install_path/ $ git clone https://github.com/phacility/arcanist.git
```
Now add `some_install_path/arcanist/bin/` to your PATH environment variable.
When you type "arc", you should see something like this:`Usage Exception: No command provided. Try 'arc help'.`
`source /path/to/arcanist/resources/shell/bash-completion`


Software Engineer Workflow:
```
git pull: pull from remote master
git branch -b 'feature-awesome' : you make a feature branch
git commit : implement the feature
arc diff : send it for review by including a proper test plan
git commit --amend : incorporate changes suggested by the reviewer
arc diff: send it for review again
git commit --amend : incorporate changes suggested by the reviewer
arc diff : send it for review by including a proper test plan
git commit --amend : incorporate changes suggested by the reviewer
arc diff: send it for review again
git commit --amend : incorporate changes suggested by the reviewer
....... ITERATE UNTIL THE REVIEWER IS SATISFIED ......
Once the reviewer is satisfied: make sure you're upto speed with changes others have made
git checkout master;
git pull;
git checkout feature-awesome
git rebase master
git push
```
From now on all the code that goes onto master will be reviewed first on Phabricator. Let me know what you guys think!
