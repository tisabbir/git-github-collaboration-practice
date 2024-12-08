## Basic Git

**1. git init**

- This command initializes a new Git repository in the current directory. It creates a hidden folder called ".git" that stores all the version control information for your project.
- Essentially, it tells Git that this directory is now under version control and you can start tracking changes to your files.

**2. git add README.md**

- This command adds the file named "README.md" to the staging area. The staging area is a temporary holding area where you specify which files you want to include in the next commit.
- By adding the file, you're telling Git that you want to track changes made to this specific file in the future.

**3. git commit -m "first commit"**

- This command creates a snapshot of the current state of your project, including all the files that have been added to the staging area. The `m` option allows you to provide a commit message that describes the changes you're making.
- In this case, the message "first commit" indicates that this is the initial commit in your repository.
- This snapshot is stored in Git's history, allowing you to revert to previous versions or track the evolution of your project.

**4. git branch -M main**

- This command renames the current branch to "main". By default, Git creates a branch named "master" when you initialize a repository. However, many developers are now adopting the convention of using "main" as the default branch name.
- The `M` option tells Git to force the rename, even if there are uncommitted changes in the current branch. It's generally recommended to avoid using the `M` option unless you're certain about the changes.

**5. git remote add origin [invalid URL removed]**

- This command adds a remote repository named "origin" that points to the GitHub repository URL you provided. This establishes a connection between your local repository and the remote repository on GitHub.
- Now, you can use Git commands to push your commits to the remote repository and share your project with others.

**6. git push -u origin main**

- This command pushes your local "main" branch to the remote repository named "origin" (which you defined in the previous step). The `u` option sets "origin" as the default upstream branch, meaning future push commands won't require you to specify the remote and branch name again (unless you change the upstream configuration).
- By pushing your local commits to the remote repository, you're making your changes visible to others who have access to the GitHub repository.