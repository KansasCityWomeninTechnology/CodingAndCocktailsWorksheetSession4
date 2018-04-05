1. Let's make a change to _cocktails.txt_. Open Atom by typing `atom .` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='working' %}
What was up with that Atom command?
When you install Atom it automatically adds itself to your system PATH. The command `atom` opens Atom. Adding `.` tells Atom to open at this file location.
   {% endhint %}
   {% hint style='danger' %}
##### Attention Chromebook users

You will use the built in text editor.
   {% endhint %}

1. Think of your favorite cocktail and add it at the of the sentence in _cocktails.txt_ in Atom. Save your file. 

1. We made an edit to an existing file. Let's see what `git status` in the terminal shows. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git status]
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
**[error    modified: cocktails.txt]
no changes added to commit (use "git add" and/or "git commit -a")

   ```

1. We modified a file so let's check out the difference between them. Type `git diff` <i class="fa fa-share fa-rotate-180"></i>.
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (master)]
**[delimiter λ ]**[command git diff]
diff --git a/cocktails.txt b/cocktails.txt
index 29a3e24..4d8a785 100644
--- a/cocktails.txt
+++ b/cocktails.txt
@@ -1 +1 @@
**[error -My favorite cocktail is]
**[warning +My favorite cocktail is Code on the Beach.]

   ```
   Git diff shows us the difference in the files. The top line in red with the `-` in front of it shows the line removed. The second line with the `+` in front of it shows the line added.

   {% hint style='info' %}
We only see differences when a file is unstaged.
   {% endhint %}
   {% hint style='tip' %}
Depending on the amount of changes, your terminal may display the output using 'less'. To exit out of 'less' type `q`. Refer to [Command Line Basics](https://codingandcocktailskc.gitbooks.io/session-2-command-line-basics/content/) for more details on 'less'. 
   {% endhint %}

1. In GitKraken, select the top row in the git tree named "//WIP" and then click on _cocktails.txt_ in the **Unstaged Files** list. Take a look at the diff and compare to what you saw in the terminal.

