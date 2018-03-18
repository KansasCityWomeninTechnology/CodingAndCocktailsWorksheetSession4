1. Now we can commit our new file to git. Type `git commit -m "important file"` <i class="fa fa-share fa-rotate-180"></i>. You should see something like this in your terminal
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git commit -m "my first commit"]
[master bc3f239] my first commit
1 file changed, 1 insertion(+)
create mode 100644 cocktails.txt
   ```
  {% hint style='info' %}
We committed a snapshot of the files to the repository history. We see each of these commits in the git graph. The '-m' flag allows you to provide a description of the changes. This is important information for those who may collaborate on the code later.
   {% endhint %}
   {% hint style='tip' %}
If you accidentally hit `Enter` after you typed `git commit`, have no fear.

Your default text editor (default is vi) will open, where you can add your commit message.
   {% endhint %}

1. Your terminal changed back to how it looked before we added the _cocktails.txt_ file. Take a look at your git status and in GitKraken. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git status]
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
(use "git push" to publish your local commits)
nothing to commit, working tree clean
   ```