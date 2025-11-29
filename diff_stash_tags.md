# diff

git diff is an informative command that shows the differences between two commits. It is used ot compare the changes made in one commit with the changes made in another commit. Git consider the changed versions of the same file as two different files. Then it gives to these two files and shows the differences between them.

How to read the diff

- a -> file A and b -> file B
- ----indicates the file A
- ----indicated the file B
- +++ indicates the file B
- @@ indicates the line number

## Commands
- git diff
- git diff --staged
- git diff <branch_name_one>..<branch_name_two>
- git diff <commit_hash_one>..<commit_hash_two>

# Stash

Stash is a way to save your changes in a temporary location. It is useful when you want to make changes to a file but don't want to perform commit.
You can switch to another branches and again come to the branch where you kept the chnages in stash and apply the changes
## Commands
- git stash
- git stash save "work progress on X feature" --> for giving name to stash
- git stash list -> gives all the stash file
- git stash apply -> apply stash
- git stash apply stash@{0} -> to apply particular stash
- git stash pop -> apply and drop
- git stash drop -> to drop any stach
- git stash clear

# Tags

- Tags are just like sticky notes for a commit
- git tag <tag_name>
- git tag -a <tag_name> -m "Relase 1.0"
- git tag
- git tag <tag_name> <commit_hash>