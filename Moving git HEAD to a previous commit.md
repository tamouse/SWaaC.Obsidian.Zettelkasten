# Idea

Sometimes, in the course of development work, we decide that we didn’t actually want a commit.

# Description

Moving the HEAD pointer back to previous commits in your _local working tree_ essentially erases the commits that had been added.
It's also possible to do this to a remote.

# Sources

1.  [SO: GIT: move HEAD back to a previous commit](https://stackoverflow.com/questions/14243089/git-move-head-back-to-a-previous-commit)
2.  [Git reset](https://git-scm.com/docs/git-reset)
3.  [Git revert](https://git-scm.com/docs/git-revert)

#article #check


# Compass
![[2023.07.08.ZettelkastenVideosNotesP039atomicMap.jpg]]
## West - similar ideas

## East - opposing ideas
- [[Problems changing remote commit history]]

## North - questions for this idea

## South - outcomes this idea leads to

==Anecdote==

In a situation I recently ran into, I had done a merge from `main`, and then the tech lead said to rebase it instead. Luckily, I hadn’t yet pushed to `origin` so I could back out of the commit I had made.

But how?

[[I had not pushed my branch yet (moving git HEAD)]]
[[But what if I had pushed my branch? (moving git HEAD)]]
