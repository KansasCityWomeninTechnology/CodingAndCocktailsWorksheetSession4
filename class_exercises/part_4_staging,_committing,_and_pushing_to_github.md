### Part 4: Staging, Committing, and Pushing to GitHub {#part-4-staging-committing-and-pushing-to-github}

There are three vital steps to pushing your changes up to GitHub: **staging**, **committing,** and **pushing.** The first step is to tell Git which files you want to add to the repository. This is called **staging** your changes. Then, you prepare to push them using the `commit` command. Finally, the committed changes are pushed up to the cloud and Git assigns a unique alpha-numeric log entry, known as a **commit hash**, to track that change. Let’s try it now.

1.  In Git Bash or iTerm2, type `git status`.  This shows you what changes you have made to your code.

2. Type `git add README.md`.

3. To verify that your files were added, type `git status`, which will tell you all about your repo. the last line will show which files have been modified.<br>
![](../assets/image09.png)

4. In Atom, make another change to your _README.md_ file and save the changes.

5. In Git Bash or iTerm2, check your status again by typing `git status`.  You'll see that the _README.md_ file was again modified.

6. This time,  type `git add -A`, to add all files you have modified since the last commit to the staging area.

2.  Commit your changes with a brief commit message by typing `git commit -m "Initial Commit"`.

    The -m flag is necessary and should accurately and concisely describe the content of the changes. This is important information for those who will be responsible for maintaining your code later. Your changes have been committed and are ready to be pushed up to GitHub.
![](../assets/image00.png)

3.  Type `git push origin master` to initiate the push.

    {% hint style='info' %}
    “origin” tells Git you are pushing the changes to the original remote location

    “master” indicates which branch within the remote location you'd like to push to.
    {% endhint %}

Voila! You have pushed your first revision to GitHub!
