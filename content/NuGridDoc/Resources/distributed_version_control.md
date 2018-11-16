# Distributed Version Control

This page describes resources that users need to use the NuGrid
distributed version control facilities. It starts with information on git that is 
used for active developement. For archival access to the NuGrid svn server see bottom of this document.

## Git

### Quickstart guide

#### Access with your browser 

`https://github.com/NuGrid/SAMPLE_REPOSITORY`

#### Command line access:

* Install git on your computer. For example, if you are using linux: `sudo apt-get install git`
*  For one time on each machine you need to configure git and tell it who you are and how you want to identify when talking to [Github](http://gitub.com/nugrid):
    - `git config --global user.name "GITHUB_USERNAME"`
    - `git config --global user.email "GITHUB_EMAIL"`
* the most convenient way to authenticate with [Github](http://gitub.com/nugrid) is to add your public ssh key to your github profile
* In a convenient location on your computer clone a NuGrid repo, e.g.: `git clone git@github.com:NuGrid/NuPPN.git`


* If you want to make changes create a branch first: `git branch name_of_branch`, then switch to that branch `git checkout name_of_branch`, or in one step `git checkout -b branch_name`
* make your changes to the branch and `git add` and `git commit`, then `git push`; finally on the GitHub page do a git pull request and assign an assignee, and alert other through `@mentions`. 
* look into the difference between `git fetch` (which is doing a plain sync of the remote with the local or origin) and `git pull` which is a combination of `fetch` followed by `merge`
* If you want to pull an existing branch from GitGub: `git checkout name_of_existing_branch`, then `git pull origin name_of_existin_branch` 

### Resources to adopt github 
 * [svn 2 git transition guide](https://www.atlassian.com/git/tutorials/svn-to-git-prepping-your-team-migration)
 * [Short online git tutorial](https://try.github.io/levels/1/challenges/1)
 * [First time git setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
 * [Git essentials and links to further resources](https://github.com/fherwig/physmath248_pilot/blob/master/git_intro.ipynb) 

### Useful commands

* provide a summary of branches, their relation and evolution: `git log --all --oneline --decorate --graph`
* you have made some changes to your repo and you would like to undo all of them and go back to the last commit, including recovering files that you may have deleted: `git reset --hard`

### Using Git Submodules
The purpose of git submodules is to create a version controlled link
between the repository and git repositories that it depends on. When a
repository is linked as a submodule the relative path to the submodule
in the repository and the URL of the submodules remote is stored in the
version controlled file ".gitmodule" if a specific branch to be tracked
is specified it will also be stored in the ".gitmodule" file. When the
submodule is linked and updated the result is a git repository nested
with in your main git repository. NOTE: since the submodules are nested
git repositories if your current working directory is in submodule any
git command will act on the submodule and not the main git repository.

#### Adding a Submodule
To add a new submodule to the current repository use the command,

```
git submodule add <URL>
```

This will create the file ".gitmodule" in the root directory of the
repository if the file does not exist already and it will create a
directory containing a clone of the master branch from the repo at the
URL. The path to where the submodule should be created can be
specified using the command

```
git submodule add <URL> <PATH>
```

By default the submodule pulls commits from the master branch of the
submodule's remote. A branch other than master can be tracked by using
the flag "-b <branch>", the command to link a submodule tracking a
branch other than master is then,

```
git submodule add -b <branch> <URL> <PATH>
```

Once the submodule has been added the submodule repository will be
cloned into the specified path. NOTE: the submodule links to a specific
commit on a branch not the branch itself; spesifying the branch tells
git which branch to pull from when updating to the newest commit on the
submodule's remote. So when someone clones the repository the their
submodule will point to the same commit even if that commit is behind
the branch's HEAD. This guarantees that a given commit of the main
repository will always point to the same commit of the submodule unless
it has been manually updated after being checked out.

#### Cloning a the Project
When cloning a repository by default the contents of the submodule are
not fetched since they are tracked by a different repository. The simplest
way to clone a repository with submodules is to tell the clone command
to recursively clone the repository using the flag "--recursive". The
command is,

```
git clone --recursive <URL>
```

If the repository is not cloned recursively the submodules can be
checked out using the commands,

```
git submodule init
git submodule update
```

or

```
git submodule update --init
```

In either case git processes two steps. First the submodules are
initialized, the information about the submodule’s URL, PATH and BRANCH is
updated in the main repositories ".git" files. Then the HEAD commit
from the specified branch is checked out into the submodule's PATH.

Whether you clone recursively or update the submodules manually, in
either case git will checkout the latest commit in the specified branch
not the branch itself. So when updated the contents of the submodule
will be updated but in the detached HEAD state.

#### Updating submodules
Commands that update the main repository by default will not update the
contents of the submodules. To update all of the submodules to the
commit specified by the main repository use the command,

```
git submodule update
```

But if you would like to update the submodules to the latest commit on
the submodule's remote in the branch that it is tracking, then use the
command

```
git submodule update --remote
```

If this change is committed then that commit of the main repository will
point to the updated commit of the submodule. Alternatively if you
navigate to the submodule's directory you can checkout any commit which
can then be applied to the main repository in the same manner.

#### Branching with submodules
If you switch to a branch that contains the same submodules pointing to
the same commits of the submodules, then using submodules will have no
side effects. However if you switch to a branch with different submodules
from the current branch there are two side effects. First, any
submodules that are not in the new branch will be left as untracked
files after checking out the new branch. Second, any submodules that
where not in the old branch will not be checked out after the branch is
checked out, so you will need to call the command `git submodule update`
so the submodule is checked out. If you switch to a branch with the same
submodules but which point to different commits then you will need to
call the command `git submodule update` to get the correct version.

#### Example of Submodules
There is an example use of git Submodules in the repository
[https://github.com/NuGrid/Sandbox](https://github.com/NuGrid/Sandbox)
under the [lsiemens_banch](https://github.com/NuGrid/Sandbox/tree/lsiemens_branch) branch.


### Useful tools

#### Graphical tools
* github desktop

##### Linux

* `gitg`
  locally allows to graphicaly see history, branches, etc.

## svn

NuGrid maintains a svn server at Keele. It is for members only. As we
transition to [NuGrid GitHub organization](http://github.com/nugrid) content will be deleted from the svn. Use of svn for active projects is at this point not supported and strongly discouraged (i.e. don't do it).

### Resources for svn
* The [svn book](http://svnbook.red-bean.com)

* NuGrid Plone [Getting started with
  Subversion](http://www.nugridstars.org/work-packages/io-technologies/getting-started-with-subversion/?searchterm=svn)
