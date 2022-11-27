# Reading 3: Revisions and the Cloud

> [@non-technical-friend](mailto:non-technical-friend@seattle.gov) wrote:  
>
> What is version control?

Version control is a system to track changes in file or project over time, in an organized way that allows the creator(s) to review previous iterations and revert to them if necessary.

> How many kinds of version control systems are there?

There are 3 kinds of version control: local, for a single creator on a single computer; centralized, for top-down collaboration by multiple creators through a single portal; and distributed, which allows creators to collaborate while bypassing the central portal.

> What kind of VCS is git?

Git is a *distributed* version control system.

> How does git relate to GitHub?

Git is a terminal-based version control system, originally created for Linux, that is installed on the creator's client machine. GitHub is a website/hosting service run by Microsoft that, among other things, provides a place to keep your git repositories.

> At first you were creating projects in GitHub, why did you stop?

A couple of reasons:

- the editing tools on the client side are better (more powerful/more user-friendly) than editing in the browser on GitHub
- working locally and pushing changes only one direction prevents inconsistencies in edits

> How do I add the GitHub repository I already have into git?

If you already have a repository, you can add it into git using `git clone url.git`. We already have a repository on GitHub, so to find its address:

1. navigate to GitHub
2. click the green `< > Code` button
3. look for the repository URL in the `HTTPS` tab

Git copies all of the files in the repository into a directory on your local hard disk, so you can edit them locally and then upload the changes to the repository later.

> After I work on my files locally, how do I send them to my GitHub repository?

There are 3 stages to the process of incorporating ("pushing") changes you make to your files into the copies of the files in the repository. But before you start pushing changes you should check what git says changed compared to what you think you changed.

You do this using `git status` which will output a list of all the files in the local copy of your project that have been modified, any new files, and any files selected for deletion.

Once you check with `git status` you are ready for the 3 step A-C-P process
- **Add**
- **Commit**
- **Push**

1. Add your files from the working directory (local) to the index/staging area using `git add`
   - there are 3 ways to add files
     - individually `git add file.txt`
     - multiple files in batches `git add file1.txt file2.txt`
       - separate files with a single space
     - all files at once `git add --all`
   - after adding your files, check they are in the staging area using `git status`
2. Once files are in the staging area, approve the changes using `git commit`
   - when you commit changes, it's important to add an explanation of **why** you made the changes
   - the why needs to be readable and understandable in your change log
   - don't write *what* the changes are because it might not make any sense to someone else reading your change log
   - 2 ways to add a commit message
     - `git commit -m "change messsage"`
     - in VSCode, if you run `git commit` without the message flag `-m`, it creates a tab where you can write a commit message. Say something, save message, and close it, and then `git commit` will be able to finish
     - a blank commit message will cause `git commit` to abort, including if you save a blank message in VSCode
3. After committing your changes with a message, you have to push them from your local computer to the repository (ie GitHub) using `git push`
   - in our case we are pushing from `main` to `origin` so we have to use the syntax `git push origin main`
   - by default git names the local copy of the repository `master` but ours was renamed to `main` when we created it
   - `origin` is the copy of the repository on the remote server (for us GitHub)
   - we know that we are using `main` because when we are inside the git repository in the terminal, the active directory looks like `git:(main)`

[Go back home](/reading-notes/)
