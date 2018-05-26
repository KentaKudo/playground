1. Make a commit A.
2. Make a commit B.
3. Check commit has using `git log`, and pick up the one previous to commit A.
4. `git rebase -i <commit hash>`.
5. Modify action of commit B to **squash**.
6. Modify commit message. In most of the cases, it should be just deleting the commit message of B.
7. Force-push rebased commit if it's already in remote with `git push --force`.

