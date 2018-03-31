1. Find a buddy at your table. Using Chrome, navigate to their "MyFirstRepo" page.

1. Find the **<span class="octicon octicon-repo-forked"></span> Fork** button in the upper right corner of the page and click on it.
    ![](images/fork.png)

    {% hint style='danger' %}
If asked, “Where should we fork this repository?” Select your personal profile. This question indicates you're a part of a GitHub organization but we want to use our personal accounts this evening.  If you are not asked that question, carry on.
    {% endhint %}

1. In your terminal, navigate to "CodingAndCocktails/VersionControl" folder in your home directory. If you are already in "MyFirstRepo", you can type `cd ..` <i class="fa fa-share fa-rotate-180"></i>.

1. GitHub will automatically add a "-1" to the name of the repo so that repo names are unique. Once the fork completes, GitHub navigates to your fork. Click on the green clone button to get the link to clone the fork to your machine.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git clone </code> and paste the link <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Navigate into "MyFirstRepo-1" and create a new branch using your username and add "-branch" after it. In our example, user "ladydev" will create "ladydev-branch".
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git checkout -b ladydev-branch</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. In the newly created branch, create a new file named using your name, such as "ladydev.txt". Add the message "Hello fellow ladydev!". Feel free to use the `echo` command, `vim`, or in Atom.

1. In the terminal, add, stage, and commit your file. Add a friendly commit message.
   {% hint style='tip' %}
This file is not tracked by git, so you have add the file first. Then you can stage and commit the changes. Refer to [Add a new file and check status](ws-2create/#add) for further guidance.
   {% endhint %}

1. Push your changes and branch.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git push --set-upstream origin branch-name</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Create a pull request by clicking the **New pull request** button. 

1. This time when comparing branches you're comparing against forks. We want the changes from our branch to migrate to your buddy's master branch so select your newly created branch in the right-most dropdown. 

1. Click the green **Create pull request** button twice. You created a pull request to make a change to your buddy's repo! Hopefully they merge it in soon!

1. Don't forget to accept your buddy's pull request
   1. To merge in your buddy's pull request, navigate to your "MyFirstRepo" in Chrome. Click on **<span class="octicon octicon-git-pull-request"></span> Pull requests** to see the pull request. There should be a number after it indicating the number of open pull requests.

   1. Click on a pull request. Click the green **Merge pull request** button and then click the green **Confirm merge** button.

![](https://i.giphy.com/media/3oz8xFT5JkOhZhCWDC/giphy.webp)
