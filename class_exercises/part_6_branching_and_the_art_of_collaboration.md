### Part 6: Branching and the Art of Collaboration {#part-6-branching-and-the-art-of-collaboration}

Now we are going to collaborate on a very simple web application.

1.  In Google Chrome, navigate to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp). 

2. Click on the issues tab at the top.

3. Look through the list of issues for one that does not yet have a comment icon on the right side: ![](/images/comment.png).

4. Click on the issue to open it and at the bottom, add a comment "This issue is assigned to @<your GitHub Username>". Replacing the angle brackets and text "your GitHub Username" with your actual GitHub username, leaving the @ symbol. Make note of the issue number to use in step 7. 

5. Fork the repository.

    {% hint style='tip' %}
    If you need a refresher on how to fork a repository go back to [Part 5: Forking](/class_exercises/part_5_practice_with_forking.md).
    {% endhint %}

6. In Git Bash or iTerm2 you are probably still in the _MyFirstRepo_ directory from step 4. If so, type `cd ..` to navigate back up to your `VersionControl` directory.  If you are anywhere else change directories to the _VersionControl_ directory.

7. Clone the repository and `cd` into it.

7. Use the issue number from step 4, make a new branch. In Git Bash or iTerm2, type `git checkout -b issue-##` to do this.

    {% hint style='tip' %}
    If you are working on issue #4, your branch name would be **issue-04**.
    {% endhint %}

8. To view all branches within the repo, type `git branch` . This should show you at least two branches - master, and the issue-## branch you just created. The branch you are currently working in will be highlighted with an asterisk (*).

    {% hint style='tip' %}
    To switch between branches type `git checkout {{branchname}}` 
    {% endhint %}
    
9.  In Git Bash or iTerm2 type `atom .`. This will open your Atom text editor with the context of the current directory.

10. Make changes to the application as instructed in your issue and make sure to save any files you change. 

11.  After you've saved your files, in Git Bash or iTerm2, type `git status` to view which files you've changed. 

12. If everything looks good, stage and commit your changes. Type `git push origin <branchname>` to push to the branch you made to your remote fork, substituting your own branch name for the angle brackets and "branchname" text. Now you have pushed your changes to the _origin_ (that is, to the cloud), to your specific branch.

9. Create a **pull request** to migrate your changes from the fork and branch you have been working on to the Kansas City Women in Technology repository.

    1. In Google Chrome, navigate to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp) and click on the **New Pull Request** button.
    
    ![](/images/pullrequest.png)

    2. Click the "compare across forks" link at the end of the text "Compare changes across branches, commits, tags, and more below. If you need to, you can also compare across forks."
    
    3. Keep the "base fork" (organization where you are moving your changes **TO**) as KansasCityWomeninTechnology 

     4. Change the "base" (the branch within the organization you selected to move your changes **TO**) as "vc-final".
    
    4. Change the "head fork" (User that you're moving changes **FROM**) to yourGitHubusername/DrinkOrderApp 
    
    5. Change the "compare" to the issue-## branch you created in step 7.
    
    Feel free to add any comments you'd like.  If you keep scrolling down you'll see the commits you added to make the change along with the diff across the file(s) you changed.
    
    5. Click on the Green "Create pull request" button.

    {% hint style='info' %}
    If Git detects no conflicts, it will give you a checkmarked message saying “able to merge.”
    
    If Git detects conflicts, it will display a red message saying "Can't automatically merge."
    {% endhint %}

11.  Typically we would expect someone to have oversight into merging the pull requests into the master branch to become the final version of the code. Once your pull request is accepted by this person, you can view your code in the master branch, along with all of the changes your peers have made.

**Congratulations! You’ve collaborated on a project for the first time!**