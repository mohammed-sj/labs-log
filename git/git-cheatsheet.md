# **Git Cheatsheet**

## **1. Starting & Setting Up a Repo**   

`git init` | create a new repository
`echo ".env" >> .gitignore` | add file patterns to ignore
`pre-commit install` | enable pre-commit hooks in the repo

---

## **2. Staging, Committing & Saving Work**   

`git add <FILE>` | stage a file
`git commit -m "message"` | create a commit
`git commit --amend` | edit the last commit
`git revert HEAD` | undo the most recent commit safely

---

## **3. Status & History**   

`git status` | see staged/unstaged changes
`git diff` | show unstaged changes
`git diff --staged` | compare staged changes to last commit
`git log --oneline --graph` | compact history view
`git log --graph --oneline --all` | visualize full repo history
`git show <COMMIT>` | show what happened in a commit
`git blame <FILE>` | show who changed each line
`git reflog` | show all HEAD movements (recovery tool)

---

## **4. Branching**   

`git branch` | list/create branches
`git checkout -b <branch>` | create and switch
`git switch -c <BRANCH>` | create and switch (newer command)

---

## **5. Merging, Rebasing & Clean History**   

`git merge <BRANCH>` | bring another branch into current
`git rebase <BRANCH>` | reapply commits on top of another
`git rebase -i HEAD~3` | interactive rebase (squash/reorder last 3 commits)
`git cherry-pick <COMMIT>` | copy a commit from another branch

---

## **6. Undoing, Fixing & Restoring**   

`git restore <file>` | undo unstaged changes
`git reset --soft|mixed|hard` | move HEAD / unstage / delete changes
`git revert <COMMIT>` | safely create an “undo” commit
`git cherry-pick <commit_id>` | re-apply a specific commit (repeated for clarity)

---

## **7. Stashing**   

`git stash` | store unstaged changes
`git stash push -m "<msg>"` | stash with a message
`git stash pop` | apply + remove stash
`git stash apply` | apply stash but keep it

---

## **8. Working With Remotes (GitHub)**   

`git pull` | fetch + merge from remote
`git push origin <BRANCH>` | push branch to GitHub


