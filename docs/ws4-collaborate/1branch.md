1. We've been making all our changes to 'master' branch. Let's create a branch for our next set of work. In the terminal, type `git checkout -b cocktails-branch` <i class="fa fa-share fa-rotate-180"></i>. It should look like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (master)]
**[delimiter λ ]**[command git checkout -b cocktails-branch]
Switched to a new branch 'cocktails-branch'
   ```
   {% hint style='info' %}
Your terminal might look a little different after creating a branch. The terminals we have you use include the branch name, so you should see 'cocktails-branch' included in your prompt.
   {% endhint %}

1. Type `git status` <i class="fa fa-share fa-rotate-180"></i>. It should look something like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
nothing to commit, working tree clean

   ```

1. In Atom, edit _cocktails.txt_ by adding a new sentence. Perhaps your second favorite cocktail? Save the file.

1. In the terminal, stage your file and commit your change. 
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git commit -am "personalized message here"</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Take a look in GitKraken. It shows 'cocktails-branch' in the top toolbar and added your branch under **LOCAL** branches on the left. We've created a branch but the origin, GitHub, doesn't know about it. We need to push our new branch info.

1. In the terminal type `git push` <i class="fa fa-share fa-rotate-180"></i> like we did before to push our changes. Oh oh! We got an error
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git push]
fatal: The current branch cocktails-branch has no upstream branch.
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin cocktails-branch
   ```
   {% hint style='info' %}
JAD TODO hint here?
   {% endhint %}

1. Type `git push origin cocktails-branch` <i class="fa fa-share fa-rotate-180"></i>.

1. Switch back to 'master' by typing `git checkout master` <i class="fa fa-share fa-rotate-180"></i>.

1. In Atom, notice your change to _cocktails.txt_ is no longer there. That's because our change only exists in the 'cocktails-branch' branch. 

