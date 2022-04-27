[Return to main page](https://KrisDunning.github.io/reading-notes/)

# Git Intro Summary

*****

Git is a version control system (VCS). Version control tracks modifications and can merge changes from different users or revert changes if the results are undesireable. Local VCS lives on local storage and may be susceptible to drive loss. Distributed Version Control (DVCS) combats this by allowing mirrored repositories to exist. Git is just one example of a DVCS.

Git stores the data as a snapshot or a commit. Data can be one of 3 states. Modified, staged or committed.

- Modified- data has changed but not committed to the database
- Staged- Flagged a files changed version to be committed in the next snapshot
- Committed- Data is securely stored in the local database

Git is normally used via the terminal but there are some graphical user interfaces abailable for many OS's. 

The standard operation cycle for git is to clone a repository. Make changes desired to files. ADD files to que for committing. The commit files to local repository. Then push files to remote server if utilizing such. 

Usefull terminal commands are :

- git help command- opens the git manual
- git status- reports status of files in repository
- git add [filename]- adds files to be committed
- git commit [filename]- stores files in the repository (git commit -m "useful message")
- git push origin main- push files from local to remote storage

*****
