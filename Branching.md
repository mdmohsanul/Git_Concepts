# What is branch
- Branch let us to work on a feature, bug fix, or some experiment without affecting the main branch
- Each branch manage its own commit history
- Branches make parallel development

# Commands to create branch 

- git branch -> gives all the branch for that particular repo
- git branch dark-mode -> it will create a branch
- git switch dark-mode ->  it will switch to dark-mode branch
- git log -> this will show the commit history for the current branch
- git switch -c dark-mode -> create and switch to new branch  ✅ recommended (modern way)
- git checkout -b orange-mode -> create and switch to new branch ❎ old way

# -c flag means create new branch
 
| Task               | Command                                  |
| ------------------ | ---------------------------------------- |
| Create branch      | `git branch new-branch`                  |
| Create + switch    | `git checkout -b new-branch`             |
| Switch branches    | `git checkout branch-name`               |
| Create from remote | `git checkout -b new-branch origin/main` |

# commit before switching
# Go to .git folder and checkout to the HEAD file, HEAD will refer to the current branch

# Rename a branch
- git branch -m <old_branch_name> <new_branch_name>

# Delete a branch
- git branch -d <branch_name>

# What is merge conflicts--------------------------------------

A merge conflict occurs when Git cannot automatically merge two branches because of conflicting changes in the same file or line.

- Merge conflicts occur when Git cannot automatically decide that which changes to keep because two branches modified the same part of the same file in different ways.

* Main Situations Where Merge Conflicts Occur

1. Both branches edit the same lines
This is the most common one.

2. One branch deletes a file that the other edits
Git doesn’t know:
Should the file exist?
Should it be deleted?

3. Both branches rename a file differently
e.g.,
One branch renames index.js → main.js
Another renames index.js → app.js
Conflict.

4. Both branches modify the same block of code
Even if it’s a few characters — same region = conflict.

5. Rebase conflicts
Rebasing applies commits one-by-one on top of another branch → each commit can conflict. 

# How do you resolve a merge conflict?

git merge feature
# conflict happens
git status   # shows conflicting files
open files
fix conflict markers
git add .
git commit

✅ 1. Accept Current Change
Keeps your branch’s code (the code in your feature branch)
Ignores the changes coming from main

✅ 2. Accept Incoming Change
Keeps main branch’s code
Replaces your changes with whatever came from the latest main

✅ 3. Accept Both Changes
Keeps both versions in the file, one after the other (you may adjust manually)

✅ 4. Compare Changes
Opens a side-by-side diff so you can visually compare your version vs main’s version


Fast-forward merge simply moves the branch pointer because no divergent commits exist.
Recursive merge is used when both branches have diverged; Git performs a 3-way merge and creates a merge commit.