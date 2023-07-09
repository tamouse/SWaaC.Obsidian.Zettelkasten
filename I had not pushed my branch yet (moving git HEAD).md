Following the advice given in this [StackOverflow](https://stackoverflow.com/questions/14243089/git-move-head-back-to-a-previous-commit) question, the form of the operation looks like this:

    git reset COMMIT_SHA
    git reset --soft HEAD@{1}
    git commit -m "Reverted to COMMIT_SHA"
    git status
    # Check on the uncommitted files, see if you want to salvage any of this work
    git reset --hard

`COMMIT_SHA` is the short or long SHA of the commit I want to roll back to, e.g. "56c637bd8" or "56c637bd8a369373dcfdc62cbdca810658a7fd4e"

In the scenario I was in, I omitted the last `git reset --hard` command, so the changes that I was working on prior to the commit were left in their modified state. If I had wanted to just get rid of any changes and start fresh, then I would definitely run the last reset command.