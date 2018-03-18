# Homework {#homework}

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}


## Configure an upstream remote
In the final section you forked your buddy's "MyFirstRepo" repository. Let's configure your fork to pull down her latest changes.

1. Open your terminal and change directories until you're in the directory for your forked repository. From your home folder, type `cd CodingAndCocktails/VersionControl/MyFirstRepo-1`.

1. Configure your upstream remote (where you forked from).

   1. Type `git remote -v` <i class="fa fa-share fa-rotate-180"></i> to view the currently configured remotes.
   ![](/images/originRemote.png)
        
   1. Navigate to your buddy's "MyFirstRepo" page in GitHub and copy the link for cloning her repository. Refer to [Clone a repository](/ws1-inspect#clone) if needed. 

   1. Specify your upstream remote by typing `git remote add upstream `, paste your buddy's link, and <i class="fa fa-share fa-rotate-180"></i>.
        
   1. Double check you have a new remote configured by typing `git remote -v` again.  This time you should see both origin remotes and upstream remotes. The image shows an example using a different repository so it won't look exactly the same.
      ![](/images/upstreamRemote.png)

   1. Fetch any new commits to the upstream repository. Type `git fetch upstream`.
        
   1. Merge changes from 'upstream/master' into your local branch.  Type `git merge upstream/master` to sync with the upstream repository without losing any local changes that you may have made.  You should now be up to date with any changes that have been committed and merged into the upstream repository since you forked the repository.

      {% hint style='info' %}
This sync only updated your local copy of the repository. To update your fork on GitHub, you must push your changes to your origin remote.
     {% endhint %}

## Additional Resources

1. https://try.github.io/levels/1/challenges/1
1. https://www.codecademy.com/learn/learn-git

1. Just for fun & more practice - Learning Git branching via a game! [http://pcottle.github.io/learnGitBranching/](http://pcottle.github.io/learnGitBranching/)

1. The Atlassian Git Tutorial: [https://www.atlassian.com/git/](https://www.atlassian.com/git/)

1. Git from the Bottom Up: [https://jwiegley.github.io/git-from-the-bottom-up/](https://jwiegley.github.io/git-from-the-bottom-up/)

1. Pro Git Book: [git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)