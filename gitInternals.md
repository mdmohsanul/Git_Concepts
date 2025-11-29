# Whenever we commit the git internally create 3 objects

- Commit Object
- Tree Object
- Blob Object

# Commit Object

- Tree Object
- Parent Tree Object
- Commiter
- Author
- Commit Message

# Tree Object

- File name
- File Mode
- File Hash
- Parent Tree object


# git show -s --preety=row <commit-hash> -  gives commit object
to get commit hash use git log --oneline

# git ls-tree <tree-id> 
to get tree id from commit object

# git show <blob-id>
to get blob id from tree object