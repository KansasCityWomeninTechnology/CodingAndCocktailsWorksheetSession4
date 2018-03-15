1. In GitHub, create a new repository by clicking the <span class="octicon octicon-plus"></span> button in the upper right corner. Select **New repository**.
   
   ![](images/new-repo.png)

1. Name your repository "MyFirstRepo". Add a short description and check the **Initialize this repository with a README** checkbox. Click **Create repository**.

   ![](images/create-repo.png)

    {% hint style='tip' %}
You can ignore the **Add .gitignore** and **Add a license** dropdowns for the time being.  You won't need them for what we are doing this evening.
    {% endhint %}

1. You now have a repo! Notice you're automatically on 'master' branch. Click the green **Clone or download** button and copy the link by clicking on the <span class="octicon octicon-clippy"></span> button.

1. Open your terminal and navigate to "CodingAndCocktails/Session4" folder in your home directory. If you are already in "DrinkOrderApp", you can type `cd ../Session4` <i class="fa fa-share fa-rotate-180"></i>.

   {% hint style='info' %}
The <i class="fa fa-share fa-rotate-180"></i> icon tells you when to press `Enter`.
   {% endhint %}

1. Type `git clone` and paste the link to your repository that you copied in the previous step. Press `Enter`. Your terminal will look like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4]
**[delimiter λ ]**[command git clone https://github.com/kcwit/MyFirstRepo.git]
Cloning into 'MyFirstRepo'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
   ```

1. Type `ls` <i class="fa fa-share fa-rotate-180"></i>. You should see a new folder named "MyFirstRepo". 

1. Navigate into the directory by typing `cd MyFirstRepo` <i class="fa fa-share fa-rotate-180"></i>. Notice your terminal now contains the name of the branch 'master'.

   {% hint style='tip' %}
Don't forget to use Tab completion to make typing in the terminal easier!
   {% endhint %}

1. Type `ls -al` <i class="fa fa-share fa-rotate-180"></i>. You should see the following files
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (master)]
**[delimiter λ ]**[command ls -al]
./
../
.git/
README.md
   ```

1. Type `cat README.md` <i class="fa fa-share fa-rotate-180"></i>. You should see the contents of the read me text, which is the same text displayed in GitHub repo page.
   {% hint style='info' %}
Git has special files. One of them is the ".git" folder. It contains all the information on reconstructing the version history for your repo.   
   {% endhint %}

1. Type `git status` <i class="fa fa-share fa-rotate-180"></i>. You will see something like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/Session4/MyFirstRepo (master)]
**[delimiter λ ]**[command git status]
On branch master
Your branch is up to date with 'origin/master'.
nothing to commit, working tree clean
   ```
   {% hint style='info' %}
We haven't done anything to the repo so our working tree is clean. We can always run `git status` to double check our work.     
   {% endhint %}

1. Let's open the repo in GitKraken. Select **File** <i class="fa fa-long-arrow-right"></i> **Open**. Select **Open a Repository** and select your "MyFirstRepo" folder in your home directory.

1. When you create a repository with a read me file, GitHub automatically commits the file for you. You have 1 commit in your repository! Feel free to inspect your commit, the file, and your branch.

1. Before starting any work in a git repository, it's good practice to make sure you have the latest changes. Type `git pull` <i class="fa fa-share fa-rotate-180"></i>. Your terminal should state it's up to date.

