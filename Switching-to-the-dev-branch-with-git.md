If you like you can create a separate clone of the release_3.0.0dev branch.

To do so:
1. Change to a directory one level up from where you would like to install the new clone.

2. Issue the command:

`git clone -b <branch_name_on_GitHub> https://github.com/srhea/GoldenCheetah.git <Your_name_for_the_branch>`

eg. `git clone -b release_2.1.0 https://github.com/srhea/GoldenCheetah.git GCv2.1`

This will create a new directory called GCv2.1 and clone just the release_2.1.0 branch. Now you just need to setup the build environment (gcconfig.pri, qwtconfig.pri and possibly src.pro) and you should be good to go.

I found this easier than bouncing back and forth between branches under the main repo clone.

## Branch work

To checkout the branch, do this...

`git checkout origin/<branch_name_on_GitHub> -b <your_branch_name>`

eg. `git checkout origin/release_2.1.0 -b v2.1.0_mods`

This creates a branch in your local repo called _v2.1.0_mods_, it tracks github's repo's branch called release_2.1.0. Also, if you have commits on master that you want to rebase (move to) the release_2.1.0 branch, do a _git rebase_

git rebase release_2.1.0

Do not do a "git merge", since that would merge the two branches... bringing all the changes on master to release_2.1.0 (yours + everyone else's...)

Or a less complex way to do it... Use "git cherry-pick <hash>", that will move one commit at a time.

git cherry-pick <hash>