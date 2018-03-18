1. Type `git status` <i class="fa fa-share fa-rotate-180"></i> to see the status of our change.

1. Now let's stage the file by typing `git add cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>. Check git status and GitKraken. We see the file is staged.

1. Oops! We weren't ready to stage that file yet! Let's reset it by typing `git reset cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>. Check git status and GitKraken to see the file is no longer staged. 

1. Stage and commit your change. You can use anything you like for the commit message.
   {% hint style='tip' %}
We can stage and commit your change by passing in an extra flag to the `git commit` command. Type `git commit -am "cocktail complete"` <i class="fa fa-share fa-rotate-180"></i> to stage your changes and commit your file in one go.
   {% endhint %}

