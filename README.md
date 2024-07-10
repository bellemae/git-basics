# Git Basics - Tutorial

Git is a distributed version control system.  

**What does that mean?**  
Version control is simply a way to manage and track changes to source code. 


## Git Installation (Assumed) 

This guide assumes you have Git installed and won't go through the details of how to do that. If you don't yet have it installed, both github and atlassian offer thorough guides:
- https://www.atlassian.com/git/tutorials/install-git
- https://github.com/git-guides/install-git 

Both of the above are also great resources to keep on hand for all aspects of using Git.

## Getting started

### Getting a copy of the code - Cloning
First we need to get a local copy of the code in the repository you're wanting to work in. Ensure you are in the folder where you want this work saved.  
Now, we clone the repo with:  

    $ git clone https://github.com/bellemae/git-basics.git

:exclamation: Did you get any unexpected warnings or errors at this step? Raise these with the facilitators and we can work through them before moving on.

### Looking at what just happened
You should now see a directory called `git-basics`. This is your local copy of the repository. Navigate into your working directory and take a look:

    $ cd git-basics
    $ ls -a
You should see the files in this repo, plus a `.git` subdirectory. There are two that we will take note of for now:
* `.git` is a directory where the repo's status and history is managed. Feel free to poke around in there and see what's there :) 
* `.gitignore` is a file you can (and should) add to your repos which tells git what you DON'T want it to track. This usually contains file patterns to exclude temp files and build specific files/folders amongst other things you may not want/need to share with your collaborators. 



## Making Changes

Let's first try creating some new files. Navigate to the `testing` folder, and create yourself a new text file `yourchoice.txt`

    $ cd testing
    $ touch myfile.txt


- Staging a change
    - create a file
    - seeing the new file
    - adding the file (staging the change)
    - committing the change
