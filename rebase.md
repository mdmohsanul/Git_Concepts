# Rebase
- Git rebase is a powerful Git feature used to change the base of the branch. It effectively allows you to move a branch to a new starting point, usually a different commit, by "replaying" the commits from the original base onto the new base.
- This can be useful for keeping a cleaner, linear project history

- So basically when we merge then unnecessary a commit happens so to avoid that commit we change the base of the branch.

- git rebase

* Rebase conflicts
- git add <resolved_files>
- git rebase --continue

# Difference between git rebase and merge

- git merge integrate changes by creating merge commit and preserves the original history
Use merge when 
- when you collaborating with team a want to preserve the commit history

- git rebase integrate changes by rewriting the commit history it means it change the base of the branch.
Use rebase 
- when working on my own feature and before raising the PR
- or you want clear, clean commit log