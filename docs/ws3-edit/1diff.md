1. Create another file by typing `echo My favorite cocktail is > cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='tip' %}
Feel free to keep tabs on this file using `git status` and in GitKraken along the way.
   {% endhint %}

1. Add _cocktails.txt_ to git by using the `git add` command. 
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git add cocktails.txt</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Commit _cocktails.txt_ by typing `git commit -m "important file"` <i class="fa fa-share fa-rotate-180"></i>.

1. Let's make a change to _cocktails.txt_. Open Atom by typing `atom .` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='working' %}
What was up with that Atom command?
When you install Atom it automatically adds itself to your system PATH. The command `atom` opens Atom. Adding `.` tells Atom to open at this file location.
   {% endhint %}

1. Think of your favorite cocktail and add it at the of the sentence in _cocktails.txt_. Save your file. 

1. We made an edit to an existing file. Let's see what `git status` shows. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (master)]
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
   {% hint style='info' %}
JAD TODO Call out difference about modify versus previous git status message
   {% endhint %}

1. We modified a file so let's check out the difference between them. Type `git diff` <i class="fa fa-share fa-rotate-180"></i>.
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (master)]
**[delimiter λ ]**[command git diff]
diff --git a/cocktails.txt b/cocktails.txt
index 29a3e24..4d8a785 100644
--- a/cocktails.txt
+++ b/cocktails.txt
@@ -1 +1 @@
**[error -My favorite cocktail is]
**[warning +My favorite cocktail is code on the beach.]

   ```
   Git diff shows us the difference in the files. The top line in red with the `-` in front of it shows the line removed. The second line with the `+` in front of it shows the line added.

1. Take a look in GitKraken by clicking on the top line and then on _cocktails.txt_ in the **Unstaged Files** list.

