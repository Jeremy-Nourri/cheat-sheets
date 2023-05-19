## **Cheat sheet Git**
---


| ***Configure Git***                     | ***Git commands***                                       |
|---------------------------------------|------------------------------------------------------|
| set your git username for every repository on your computer | `` git config --global user.name "Your user name" `` |
| set your email for every repository on your computer | `` git config --global user.email "Your email" ``    |
| Verify your git username              | `` git config --global user.name ``                  |
| Verify your git email                 | `` git config --global user.email ``                 |
| Verify your git settings              | `` git config --list ``                              |


| ***Create or Clone a Repository***                | ***Git commands***                                        |
|---------------------------------------|------------------------------------------------------|
| Create a new local repository         | `` git init ``                                       |
| Clone a repository                    | `` git clone ssh://utilisateur@exemple.fr/nouveau-depot.git ``                  |                          |



| ***Remote***                     | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Add a new remote repository           | `` git remote add <remote-name> <remote-url> ``      |
| List all remote repositories          | `` git remote -v ``                                  |
| Show information about a remote repository | `` git remote show <remote-name> ``                |
| Rename a remote repository            | `` git remote rename <old-name> <new-name> ``        |
| Remove a remote repository            | `` git remote rm <remote-name> ``                    |
| Add upstream repository               | `` git remote add upstream <remote-url> ``           |



| ***Add & Commit***                     | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Add one or more files to staging (index) | `` git add <filename> ``                             |
| Add all files to staging (index)      | `` git add * ``                                      |
| Commit changes to head (but not yet to the remote repository) | `` git commit -m "Commit message" `` |
| Commit any files you've added with git add, and also commit any files you've changed since then | `` git commit -a `` |
| Commit any files you've added with git add, and also commit any files you've changed since then | `` git commit -am "Commit message" `` |
| Show all commits, starting with newest | `` git log ``                                       |
| Show changes over time for a specific file | `` git log -p <filename> ``                          |
| Show who changed what and when in file name | `` git blame <filename> `` |



| ***Pushing Changes***                  | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Push all branches to your remote repository | `` git push origin --all ``                          |
| Push master branch to your remote repository | `` git push origin master ``                         |



| ***Branches***                         | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| List all local branches in repository | `` git branch ``                                     |
| List all remote branches in repository | `` git branch -r ``                                  |
| Create a new branch                   | `` git branch <branchname> ``                        |
| Switch to a branch                    | `` git checkout <branchname> ``                      |
| Create a new branch and switch to it  | `` git checkout -b <branchname> ``                   |
| Delete a branch                       | `` git branch -d <branchname> ``                     |
| Delete a remote branch                | `` git push origin --delete <branchname> ``          |
| Delete a remote branch                | `` git push origin :<branchname> ``                  |



| ***Update & Merge***                   | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Update your local repository to the newest commit | `` git pull ``                                    |
| Merge branchname into your current branch | `` git merge <branchname> ``                        |
| View all the merge conflicts | `` git diff --check ``                              |



| ***Stash***                            | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Stash changes in a dirty working directory | `` git stash ``                                    |
| List all stashed changesets           | `` git stash list ``                                |



| ***Tags***                             | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Create a tag                         | `` git tag <tagname> ``                              |
| Create a tag with a description      | `` git tag -a <tagname> -m "Tag message" ``          |
| Push a tag to remote repository      | `` git push origin <tagname> ``                      |
| Push all tags to remote repository   | `` git push origin --tags ``                         |
| Checkout a tag                       | `` git checkout <tagname> ``                         |
| Delete a tag                         | `` git tag -d <tagname> ``                           |
| Delete a tag from remote repository  | `` git push <remote-name> --delete <tagname> ``           |


