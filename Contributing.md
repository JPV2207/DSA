# How to Contribute?

### Here's how to create a Pull Request
1. Fork this repository.
2. Clone your new repository to your system.
3. Create a new branch (i.e. add/your-name).
4. Commit changes and push the new branch.
6. Open and submit a PR.

If this is your first PR and need direction, read more below.

### Contributor's Guide

* Feedback, bug reports, and pull requests are welcome. Feel free to ask for [help](https://github.com/allenthomas01/DSA/issues).
* You can learn how to do a PR from this _free_ series [How to Contribute to an Open Source Project on GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github)

#### Steps:

1. Setting up your system by installing [Git](https://git-scm.com/) or your favorite Git client.

2. Forking the repository

* Go to the top level page of this [repository](https://github.com/allenthomas01/DSA).
* Click the "Fork" Button in the upper right hand corner of the interface ([More Details](https://help.github.com/articles/fork-a-repo/)).
* After the repository has been forked, you will be taken to your copy of the repo at https://github.com/yourUsername/DSA.

3. Cloning Your Fork

* Open a Terminal / Command Line in your project's directory.
* Clone your fork of DSA repository.

$ git clone https://github.com/yourUsername/DSA.git

(in the above command replace yourUsername with your GitHub username)

Now you have a local copy of the DSA repository.

4. Maintaining Your Fork

Now that you have a copy of your fork, there is work you will need to do to keep it current.

Rebase from upstream prior to every time you create a branch for a PR:

* Make sure you are on the master branch.


$ git status
On branch master
Your branch is up to date with 'origin/master'.


* Do a pull with rebase against master

shell
$ git pull --rebase upstream master


This will pull down all of the changes to the official master branch, without making an additional commits in your local repository.

* Merge remote changes to your local master fork:


$ git merge upstream/master

5. Create a Branch

Before you start working, you will need to create a separate branch specific to the issue / feature you're working on. You will push your work to this branch.

* Naming Your Branch

You could name the branch something relevant i.e, eg: add/your-name

* Adding Your Branch

To create a branch on your local machine (and switch to this branch):

shell
$ git checkout -b [add/your-name]


and to push to GitHub:

shell
$ git push origin [add/your-name]


If you need more help with branching, refer [this](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches). It is important to always edit only on the branch.

6. Creating a Pull Request

Editing via your Local Fork is the recommended method. Read about [How to Setup and Maintain a Local Instance](#maintaining-your-fork).

1).  Perform the maintenance step of rebasing master.

2).  Ensure you are on the master branch using git status:

        $ git status
        On branch master
        Your branch is up-to-date with 'origin/master'.

        nothing to commit, working directory clean

3).  If you are not on master, checkout git checkout master

4).  Create a branch off with git command: git checkout -b add/your-name

5).  Edit your file(s) locally with the editor of your choice.

6).  Check your git status to see unstaged files.

7).  Add your edited files: git add path/to/filename.ext You can also do: git add . to add all unstaged files. Review your git status first.
