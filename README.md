# VITMAS_Task0_21BIT0320
Description of basic git commands

**Basic Git Commands’ List**

**git config**-----
To set up the author name, email address, username, file format, and more – use the following command
git config --global user.email youremail@example.com
The ‘-global’ flag represents your email will be used for all local repositories. In case you need to use different emails for several repos then use the following:
git config --local user.email youremail@example.com

**git init**-----
This command will create a new local repository. Moreover, the repository created will be in the current directory.
git init
Alternatively, if you require a repository in a new directory, you have to specify the name like so:
git init [project name]

**git clone**-----
This is used to copy a repository if it is lying on the remote server.
git clone username@host:/path/to/repository
Similarly, to copy a local repository, use the command:
git clone /path/to/repository

**git add**-----
Add files to the staging area using the following git command which will index the temp.txt file:
git add <temp.txt>

**git commit**-----
This command will create a snapshot of the changes made and save it to the git directory. However, the committed changes won’t reflect in the remote repo as well.
git commit –m “Message to go with the commit here”

**git status**-----
Shows the overall status of changed files in a list with the files that are yet to be staged or committed.
 
**git push**-----
This command is used to send local commits to the master branch of the remote repository. in case you need to push your code to another branch and not the master, then simply replace <master> in the following git command:
git push origin <master>
  
**git remote**-----
To view all remote repos (short of repositories), run the following command and it will list the connections with the URLs.
git remote –v
To connect the local repository to a remote server or to delete a connection to a specified remote repository – use the following commands, respectively.
git remote add origin <host-or-remoteURL>
git remote rm <name-of-the-repository>

**git checkout**-----
This use of command creates branches and enable you to easily navigate between them.
command git checkout -b <branch-name>
Once the brand is created using the above command, you are automatically switched to it. Now, to switch between branches, you need to run the following
git checkout <branch-name>

**git branch**-----
A simple ‘git branch’ command will list all the branches present in the repository. Like so:
git branch
If you want to delete a branch, then use
git branch –d <branch-name>

**git merge**-----
This is used to merge a branch into an active branch.
git merge <branch-name>

**git pull**-----
This merges all the changes present in the remote repository on to your local working directory.

**git reset**-----
The index and the last working directory reset to the last git commit’s state, using this command.
git reset --hard HEAD

**git gc**-----
Using this command you can clean unnecessary files and optimize your local repo.
git gc

**git diff**-----
To view conflicts against the base file, run the following command.
git diff --base <file-name>
Similarly, to list down all the conflicts present, run:


**git reset -hard**-----
The following git command discards all history and reverts back to the specified commit.
git reset –hard [commit]

**git show**-----
To view any git object, run this small command
git show

**git fetch**-----
Fetch all objects from the remote repo that are not yet available in the local directory.
git fetch origin

**git instaweb**-----
Browse your local repository in the git-web interface with this simple command
git instaweb –httpd=webrick

**git prune**-----
This deletes objects that have no incoming pointers. Simply run

**git archive**-----
Self-explanatory? This allows creating a zip or a tar file that contains the constituents of a single repository tree. For example:
git archive --format=tar master

**git rebase**-----
When you need to apply certain changes from one branch to another, you use:
git rebase master
