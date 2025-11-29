# You committed something by mistake — how will you remove it from history safely?

1. If the wrong commit is not pushed to github
- git reset --soft HEAD~1  -> removed the commit but keeps the code staged
- git reset --mixed HEAD~1 -> delete the commit + unstage the files
- git reset --hard HEAD~1 -> delete the commit + delete file changes too:

2. If the commit is pushed to github
- git revert <commit_hash>

# Your branch is behind main — how do you update it?
Before pushing your feature branch, update it with:
git pull origin main (merge)
OR
git pull --rebase origin main (safe rebase)

# You resolved a conflict incorrectly — how do you undo it?
| Situation                            | Solution                                   |
| ------------------------------------ | ------------------------------------------ |
| Merge/rebase still ongoing           | `git merge --abort` / `git rebase --abort` |
| Wrongly fixed file but not committed | `git restore <file>`                       |
| Committed wrong fix (not pushed)     | `git reset HEAD~1`                         |
| Committed & pushed wrong fix         | `git revert <hash>`                        |

