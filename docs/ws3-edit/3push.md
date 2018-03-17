1. We've made quite a few changes. We can see the history in the command line. Type `git log` <i class="fa fa-share fa-rotate-180"></i> to see all the changes you made tonight. It should look like this

   ![](images/git-log.png)

   {% hint style='tip' %}
It shows each commit (with the unique identifier) and the commit message along with the author and date. Notice the top commit also has `(HEAD -> master)`. This says your own copy of the "master" branch is at the top commit. Notice the bottom commit has `(origin/master, origin/HEAD)`. This is the last change that your remote, GitHub, is aware of.
   {% endhint %}

1. We have 4 commits for our work so far, but we don't need to keep both commits for _cocktails.txt_. We can squash our changes. Let's squash the last 2 changes, both of which were to _cocktails.txt_. Type `git reset --soft HEAD~2` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='tip' %}
We told git to reset the last two commits you made. This command also removes the commit message but stages your file.
   {% endhint %}

1. Think of a good commit message for your cocktails change and commit your file with your message. (JAD TODO-- need guidance here?)

1. Let's check `git log` again. Now we see 3 commits instead of 4. 

1. We can also see the git graph in the terminal. Type `git log --graph` <i class="fa fa-share fa-rotate-180"></i> to see lines between each commit.

1. Type `git push` <i class="fa fa-share fa-rotate-180"></i>. Take a look at git status (states up to date with 'origin/master') and check out GitKraken. The graph you saw in the terminal should match up with what you see in GitKraken.

1. In Chrome, navigate to your "MyFirstRepo" page and reload the page. You should see your 2 new files _cocktails.txt_ and _myfile.txt_. You can click on each file to see the contents.
