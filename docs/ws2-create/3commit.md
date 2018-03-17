1. We can add the file to git by typing `git add cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>. Check your status and GitKraken.

1. Let's check out the status again. This time the terminal lists _cocktails.txt_ as a change to be committed.
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git status]
On branch master
Your branch is up to date with 'origin/master'.
Changes to be committed:
(use "git reset HEAD <file>..." to unstage)
cocktails.txt 
   ```
   You should see _cocktails.txt_ move from **Unstaged Files** to **Staged Files** in GitKraken.

   {% hint style='tip' %}
Something here about what staging is
   {% endhint %}

1. Now we can commit our new file to git. Type `git commit -m "important file"` <i class="fa fa-share fa-rotate-180"></i>. You should see something like this in your terminal
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git commit -m "my first commit"]
[master bc3f239] my first commit
1 file changed, 1 insertion(+)
create mode 100644 cocktails.txt
   ```
      {% hint style='tip' %}
Something here about what committing is. And that their terminal changed back to normal.

The -m flag allows you to provide a description of the changes. This is important information for those who may collaborate on the code later.

Also
If you accidentally hit enter after you type `git commit`, have no fear.
Your default text editor [or falls back to `vi` editor] will open, where you can add your commit message
Remember from last month: To get out of the editor, `ESC` key & then type `:wq` & then `ENTER` key
This is great for when you have a lot of changes & want a large commit message, but you'll find most of the time you stick with shorthand.

   {% endhint %}

1. Take a look at your git status and GitKraken (should no longer see _cocktails.txt_ in staged files and see a new commit in the tree view)
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git status]
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
(use "git push" to publish your local commits)
nothing to commit, working tree clean
   ```