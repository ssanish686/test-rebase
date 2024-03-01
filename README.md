1. Checkout the master or main branch from which rebasing is required.  
   `git checkout <master or main branch>`
3. Pull the latest changes.  
   `git pull`
5. Now checkout to the feature branch which needs rebasing.  
   `git checkout <feature branch>`
7. Pull the latest changes.  
   `git pull`
9. Run the rebase command in this feature branch.  
   `git rebase <master or main branch>`
10. Resolve all conflicts manually.  
11. Then add or remove all the manually changed files.  
   `git add/rm <conflicted_files>`
12. After adding the changes enter below command.  
   `git rebase --continue`
 It will open a window with commit messages, press :wq to save that.  
 If everythng goes good you will see below message.  
`Successfully rebased and updated refs/heads/<feature branch name>.` 
13. Finally push the changes to remote forcefully.  
   `git push --force`
