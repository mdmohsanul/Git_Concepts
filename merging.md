# What is git cherry-pick?

git cherry-pick takes a specific commit from one branch and applies it to another branch.

Use cases:
You want one specific fix, not the whole branch.
Hotfix from develop → main.
You accidentally committed on the wrong branch.

Example
git cherry-pick <commit-hash>

# What is git revert vs git reset?
git revert
Creates a new commit that undoes a previous commit.
Safe for shared branches.
Does not rewrite history.

git reset
Moves the branch pointer to an earlier commit.
Can discard commits (depending on mode).
Rewrites history → unsafe on shared branches.