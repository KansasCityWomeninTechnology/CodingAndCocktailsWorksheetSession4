1. In Atom, add a new sentence to _README.md_. Save your file.

1. In the terminal stage, commit, and push your change.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git add README.md</code> <i class="fa fa-share fa-rotate-180"></i>.</br>
Type <code>git commit -m "personalized message here"</code> <i class="fa fa-share fa-rotate-180"></i>.</br>
Type <code>git push</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Check the graph by typing `git log --graph` <i class="fa fa-share fa-rotate-180"></i>. It doesn't look right. Your 2 branches diverged. Now there is a change in 'master' that your 'cocktails-branch' doesn't know about. Your changes for both branches now looks like the picture below but the terminal doesn't reflect this.
   
   ![](images/git-graph-diverge.png)

1. There's another parameter we can add to the `git log` command to see the graph for all branches. Type `git log --graph --all` <i class="fa fa-share fa-rotate-180"></i>. 
   {% hint style='info' %}
Sometimes all we want to see is a high level view of the graph. You can use `git log --graph --all --oneline` <i class="fa fa-share fa-rotate-180"></i> to trim the graph up even more. Read about the different parameters you can use at [Git SCM documentation](https://git-scm.com/docs/git-log). 
   {% endhint %}
   {% hint style='tip' %}
We've been using 2 commands a lot-- `git status` and `git log --graph`. These are great candidates to create as aliases. Refer to [Command Line Basics](https://www.gitbook.com/book/codingandcocktailskc/session-2-command-line-basics/details) for more details on create aliases or ask a mentor for help.

Mac users - oh-my-zsh creates git aliases for you. Feel free to check out the [built in aliases](https://github.com/robbyrussell/oh-my-zsh/wiki/Cheatsheet) or create your own.
   {% endhint %}

1. We want to bring our changes in the 'cocktails-branch' into 'master' by creating a pull request. Before we do so, we should reconcile the differences in branches. Checkout 'cocktails-branch'.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git checkout cocktails-branch</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Make sure you have the latest changes in 'cocktails-branch' by typing `git pull` <i class="fa fa-share fa-rotate-180"></i>.

1. To sync the changes in 'master' branch into 'cocktails-branch', type `git merge master` <i class="fa fa-share fa-rotate-180"></i>. Your terminal should look like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git merge master]
Merge made by the 'recursive' strategy.
 README.md | 1 +
 1 file changed, 1 insertion(+)
   ```
   {% hint style='info' %}
In this case, we didn't really have to merge from master. Git automatically figures out how to merge the branches together. Merge is used when you have a longer running project and need to bring in changes from the rest of the development team. Sometimes when working on larger projects, there are merge conflicts. Check out the [Merge conflicts](/homework/merge-conflicts.md) bonus work as extra practice before next session.
   {% endhint %}

1. Open Atom and take a look at _README.md_. It now contains the sentence you added in the beginning of this section.

1. We created a merge commit in 'cocktails-branch' to bring in code from 'master'. In the terminal, take a look at the git graph. We see the path now includes 'master' branch. Your graph now looks like this

   ![](images/git-merge.png)

