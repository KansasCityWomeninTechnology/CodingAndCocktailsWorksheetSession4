### Part 6: Branching and the Art of Collaboration {#part-6-branching-and-the-art-of-collaboration}

Now we are going to collaborate on a very simple web application.

1.  In Google Chrome, navigate to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp). 

2. Click on the issues tab at the top.

3. Get your issue number

4. Fork the repository

5. In Git Bash or iTerm2 change directory to your CodingAndCocktails directory.

5. Clone the repository and cd into it 

4.  Make a new branch. In your command line (Git Bash or iTerm2) type `git checkout -b newbranchname` where “newbranchname” is the branch name for the issue we will assign to you in class. We suggest using issue-## as your branch name so if you were assigned issue #4 your branch name would be **issue-04**.

5.  To list all branches within the repo, use `git branch` . This should show you at least two branches - master, and the one you just created. The branch you are working in will be highlighted with an asterisk (*).

    To switch between branches type `git checkout {{branchname}}`
    
7.  In Git Bash or iTerm2 type `atom .`

8. Make changes to the application as instructed in your issue and make sure to save any files you change. 

8.  After you've saved your files, in Git Bash or iTerm2, type `git status` to view your changes. 

9. If everything looks good, stage and commit your changes. Type `git push origin [branchname]` to push to the branch you made, substituting your own branch name. Now you have pushed your changes to the _origin_ (that is, to the cloud), to your specific branch.

9.  Next, you have to migrate your changes from the branch you have been working on to the _master_ branch. To do this we create a **pull request.** Go to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp) and click on the green **New Pull Request** button.

10.  You will be prompted to select the “base”, which is where you are moving your changes TO, and the “compare”, which is where you are moving them FROM. If Git detects no conflicts, it will give you a checkmarked message saying “able to merge.” Below that will be your _commit_ message. Scrolling down further you will be able to see the commit history that is being included in this request, and the actual changed code. At the bottom for your message box, click on **Create pull request**.

11.  Typically we would expect someone to have oversight into merging the pull requests into the master branch to become the final version of the code. Once your pull request is accepted by this person, you can view your code in the master branch, along with all of the changes your peers have made.

**Congratulations! You’ve collaborated on a project for the first time!**