## Phase 4:
## phase 4.1:  Fetch & Pull Updates
- Used `git fetch instructor` to check for updates.
- Compared branches using `git diff main instructor/main`.
- Pulled latest updates from instructor repository to stay synchronized.
- No new updates were found — repository is already up to date.

## Phase 4.2: Stash Usage

 - Used git stash to temporarily save uncommitted changes before switching branches.
 - Ensured a clean working directory to prevent merge conflicts during testing.

 - Retrieved stashed changes later using git stash pop.
 - Verified that all changes were restored successfully.
 -Used stash 1 time as part of Git workflow practice.
 ## phase 4.3: Cherry-pick Practice

 - Ceated a new feature branch feature/new-feature and committed a change (feat: Add new feature).
 - Used git cherry-pick b14ffe9 to copy that specific commit into the main branch.
 - Verified the commit history using git log --oneline --graph --all.
 - Successfully applied the cherry-picked commit without conflicts.
 - Used cherry-pick 1 time to merge an isolated feature into the main branch.
 ## Phase 4.4: Git Rebase Practice

- Created a new branch feature/another-feature and added a new file test.txt with the commit message feat: Add test feature.
- Switched to the main branch and made another update (docs: Update README).
- Rebasing was performed to align feature/another-feature with the latest main updates using git rebase main.
- Resolved the branch history cleanly with a linear commit sequence.
- Successfully pushed the rebased branch to remote using git push origin feature/another-feature --force.
- Used rebase 1 time to synchronize the feature branch with the latest main branch changes
 ## Phase 4.5 – Revert, Reset & Reflog

- In this phase, I practiced advanced Git recovery commands to manage and recover changes efficiently:
- git revert: Used to undo a specific commit safely by creating a new commit that reverses the changes, preserving history integrity.
- git reset: Practiced all three modes —
 --soft: Keeps changes staged, only moves HEAD.
 --mixed: Keeps changes in the working directory but unstaged.
 --hard: Discards all changes and resets the working directory completely.
- git reflog: Utilized to view the complete history of HEAD movements and recover lost commits.
 - git cherry-pick <commit>: Applied to restore a specific lost commit after reset.
 - Documented Action: Used revert, reset, and reflog once each to test commit recovery and rollback operations.

 ## Phase 4.6 – Git Tagging
 - This phase involved tagging important project versions for clear release tracking.
-  git tag: Used to mark specific commits with version identifiers.
-  Created annotated tags to store additional metadata like author, message, and date.
-  Commands used:
    git tag -a v1.0.0 -m "Release 1.0.0: Resolved all conflicts"
    git tag -a v1.1.0 -m "Release 1.1.0: Added all features"
    git push origin --tags
-  Tags help in identifying stable release points and facilitate deployment and rollback management.
-  Documented Action: Created and pushed 2 annotated tags (v1.0.0, v1.1.0) for version control and release documentation.