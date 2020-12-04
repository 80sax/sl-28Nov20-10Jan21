## ###########################
## SCM / VCS using Git
## ###########################

## Git and Linux ---> Linus Torvalds

## Agenda

    Introduction
    Installation and Configuration
    Basic Git operations and commands
    GitHub
    
    Branching and Merging
    Undoing changes in Git
    Ignoring files in Git

## Keywords

    Master/Main/Trunk
    BugFixes / Feature
    Bundle releases --> SP1 / SP2/ SP3

**Apache 2.0 and MIT Licenses**

Linux --> RedHat, Ubuntu, Suse, Mint, Arch
Git --> BitBucket, GitLab, GitHub



## Source Code Management / Version Control System (SCM/VCS)

    - Git
    - SVN
    - CVS
    - Mercurial
    - TFS
    - Accurev
    - Perforce

## Why Version Control Systems?

    - Versioning and Rollback
    - Collaboration
    - Local and remote copies of the Source Code (Backup) --> Only applicable for Distributed VCS
    - Distributed / Parallel Development /  Branching    
    - Investigation and Accounting

## Why Git?
    - Distributed
    - Fast
    - Excellent at handling large number of branches
    - Very less administrative Overhead
     

## Types of VCS
    - Centralized - SVN, CVS, Accurev
        - Connected to the server
        - Mulitple Devs can't contribute simultaneously
        - Slow

    - Distributed

## Installation

    Office Webpage
    https://git-scm.com/

    MacOS / Windows
    https://git-scm.com/downloads

    Linux
    Ubuntu: sudo apt-get install -y git
    CentOS: sudo yum install -y git

    Git Documentation
    https://git-scm.com/book/en/v2


## Git Commands

    git config --global user.name <yourname>
    git config --global user.email <youremail>
    git config --list
    git init
    git status
    git add . (staging or tracking)
    git commit
    git commit -m "Commit message"
    git commit -a -m "Commit message" (to avoid using "git add" separately)
    git log
    git log --oneline
    git push
    git pull


Class Exercise:
    1. Create an account on Gitub
    2. Create repository on github
    3. add some sample file
    4. Clone the repository to your local laptop
    5. Add some files locally 
    6. Use git Push to push the changes to GitHub




git add .
git commit -m "..."

git commit -am ".."



References:

    - https://git-scm.com/
    - https://nvie.com/posts/a-successful-git-branching-model/
    - https://git-scm.com/book/en/v2


