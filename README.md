# TESTING GIT COMMITS

- COMMIT 1
- COMMIT 2
- COMMIT 3
- `git reset HEAD~` - undos the last commit + unstages the changes
- COMMIT 4
- `git reset HEAD~ --soft` - undos the last commit + keeps the changes staged
- `git revert --no-commit fecff0f312dfc965353498c0564734a07147d1c5 HEAD` - deletes the data upto the given commit hash
- `git checkout fecff0f312dfc965353498c0564734a07147d1c5` - just goes to that commit
- `git reset fecff0f312dfc965353498c0564734a07147d1c5 --hard` - goes to this commit, deletes everything after this in local
  - `git push -f origin main` - overwrites the changes on remote (branch before after this becomes invisible)
  - commit gets removed from github
- `git revert 9944b45e1e3f522ef06ccbc9120ae49e5d4ed66d` -- removes this commit
  - appends a commit in the github history
