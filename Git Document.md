*This file is for a help in git*

# Making a dir a git repo:
-> git init
{it will turn the current dir into git repo by adding a .git folder}

# Cloning the repo-
-> git clone [cloning link given on the repo:

# Checking the Status of current work Tree:
-> git status

# Adding a file to the current git repo:
-> git add [filename]

# Adding all file in current dir to git repo:
-> git add .

# Discaed local changes made in a file
->git restore [filename]

# Discard local changes in current dir
-> git restore .

# Commiting changes on current git repo with message:
-> git commit -m "[your massage]"

# Pushing the changes made on repo to origin at cloud:
-> git push

# Pulling changes from the origin at cloud to local
-> git pull

# Making another Branch of current repo
-> git 	branch [branch name]
{doing this will not shift you to another branch}

# Moving to another branch (checking out another branch)
-> git checkout [branch name]

# Merging the branch to origin
-> git merge [branch name]
{make sure to run this commmand after moving to master}

# Deleting a branch
-> git branch -d [branch name]
