### Part 4: Staging, Committing, and Pushing to GitHub {#part-4-staging-committing-and-pushing-to-github}

There are three vital steps to pushing your changes up to GitHub: **staging**, **committing,** and **pushing.** Let’s try it now.

1.  In Git Bash or iTerm2, type `git status`.  This shows you what changes you have made to your code.

2. Type `git add README.md`.

3. To verify that your files were added, type `git status`, which will tell you all about your repo. the last line will show which files have been modified.<br>
![](../assets/image09.png)

4. In Atom, make another change to your _README.md_ file and save the changes.

5. In Git Bash or iTerm2, check your status again by typing `git status`.  You'll see that the _README.md_ file was again modified.

6. This time,  type `git add -A`, to add all files you have modified since the last commit to the staging area.

2.  Commit your changes with a brief commit message by typing `git commit -m "Initial Commit"`.

    {% hint style='info' %}
The -m flag allows you to provide a description of the changes. This is important information for those who will be responsible for maintaining your code later.
    {% endhint %}

    Your changes have been committed and are ready to be pushed up to GitHub.
    
    ![](../assets/image00.png)

3.  Type `git push origin master` to initiate the push.

    {% hint style='info' %}
    “origin” tells Git you are pushing the changes to the original remote location

    “master” indicates which branch within the remote location you'd like to push to.
    {% endhint %}

Voila! You have pushed your first revision to GitHub!
