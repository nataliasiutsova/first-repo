# GIT FETCH vs GIT PULL

When downloading content from a remote repo, **git pull** and **git fetch** commands are available to accomplish the task.

## GIT FETCH

![img git_fetch](https://github.com/nataliasiutsova/first-repo/blob/master/git_fetch.png)

The **git fetch** command downloads commits, files, and refs from a remote repository into your local repo. Git isolates fetched content from existing local content; it has absolutely no effect on your local development work. This makes fetching a safe way to review commits before integrating them with your local repository. Fetched content has to be explicitly checked out using the **git checkout** command. If you approve the changes a remote repository, you can merge it into a local repository using **git merge** command.

## Git fetch commands and options

1. `git fetch <remote>`

   Fetch all of the branches from the remote repository.

2. `git fetch <remote> <branch>`

   Same as the above command, but only fetch the specified branch.

3. `git fetch --all`

   A power move which fetches all registered remote repo and their branches.

## GIT PULL

![img git_pull](https://github.com/nataliasiutsova/first-repo/blob/master/git_pull.png)

The **git pull** command is the more aggressive alternative; it will download the remote content for the active local branch and immediately execute **git merge** to create a merge commit for the new remote content.

## Git pull commands and options

1. `git pull <remote>`

   Fetch the specified remote’s copy of the current branch and immediately merge it into the local copy.

2. `git pull --no commit <remote>`

   Similar to the default invocation, fetches the remote content but does not create a new merge commit.

3. `git pull --rebase <remote>`

   Same as the previous pull Instead of using **git merge** to integrate the remote branch with the local one, use **git rebase**.

## GIT COMMIT --AMEND

This option adds another level of functionality to the commit command. Passing this option will modify the last commit. Instead of creating a new commit, staged changes will be added to the previous commit.

## GIT BRANCH
