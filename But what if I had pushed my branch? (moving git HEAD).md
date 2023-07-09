
In this case, I would have had to use `git revert` to revert the commits. Let’s say I want to go back 4 commits from the tip of the branch, aka `HEAD`.

    # Revert the changes specified by the fourth last commit in HEAD and create a new commit with the reverted changes.
    git revert HEAD~3
    git push -u origin BRANCH_NAME

Then when my teammates pull my branch for review and testing, it will have a commit with all the changes removed, and the history of the repo will remain intact.

