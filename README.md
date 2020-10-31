# Welcome to Git

Git is a source control software that was developed my Linus Torvalds and the Linux Kernel developers in 2005,
to help manage their large codebase with a very high number of developers. It has since become the most common
source control system.

Git is a graph-based source control system.


## Intro

There are many commands, and complex workflows in Git. However, most of the complexity can be avoided. Next, 
I'll walk you through the most common commands.

### Creating a repo

There are two primary ways to create a repository. The first is locally. If you already have an existing codebase,
or an empty directory, you can create a git repository directly in it. To do this, execute `git init`. This will 
create a git directory, and start tracking. 

The second method of creating a git repository is by cloning an existing remote repository. This will intialise a
git repository, and synchronize the files from the remote repository. To do this, execute `git clone <url>`, 
replacing `<url>` with the url of the remote repository. 

|⚠️|Note: Remote repositories can be cloned using HTTPS or SSH. |
|---|---| 

### Checking status

After cloning a repository, or making changes, you may want to check the status of your repository. You can do so
with the `git status` command. This command will show you the difference in state from your last commits, and from
the remote repository. If you are ever confused about the state of your repo, start with this command. It is always
safe to run. 


### Making and tracking changes

At this point, you're ready to make some changes. You can add a new  file, or make changes to an existing file. When
you save, you'll be ready to start tracking changes. Make and save a change, and then `git status` to see that change.
If you've made a change to an existing file, you'll see that the file has been modified. If you created a new file,
you'll see that the file is untracked.  
It's time to add these changes to our changeset. You can add them by calling `git add <filenames>` by replacing <filenames>
with the names of the files that you would like to add. Alternatively, you can add all files by calling `git add -A`.  
If you call `git status` again, you'll see that these files have now been added to the changeset, and are now tracked by git.

The next step is to commit your change. This step indicates a point in time. The state of these files will be tied to this
commit. To commit your changes, call `git commit -m '<message>'`, replacing `<message>` with your commit message. This
message should be a short description of the changes you made. Don't forget to include the single quotes.

Checking the status again, you can now see that these changes have been added and committed. 

### Pushing changes

At this point, you're ready to push your changes back to the remote repository. If you cloned your repo, the remotes
should already be configured. If you created your repo using `git init`, skip down to the next sections to learn 
how to configure remote repositories. 

Pushing your changes is as simple as calling `git push`. This is a short form of `git push <remote> <branch>`. TODO

### Configuring remote repositories

TODO

`git clone <url>`  
`git add -A`  
`git commit -m "message"`  
`git fetch -va`  
`git checkout -b <name>`  
`git push`  
`git status`  

## Terminology
|Term|definition|
|---|---|
|Repository (Repo)| A collection of source code files generally representing a deployable entity or a common set of files|
|Commit|definition|
|Tracked|definition|
|Tracked|definition|
|Remotes|definition|


⚠️❗
