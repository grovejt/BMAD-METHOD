### Upstream Repo:
  - https://github.com/bmadcode/BMAD-METHOD
  - git remote -v  
      ```
      origin  https://github.com/grovejt/BMAD-METHOD.git (fetch)
      origin  https://github.com/grovejt/BMAD-METHOD.git (push)
      upstream        https://github.com/bmadcode/BMAD-METHOD.git (fetch)
      upstream        https://github.com/bmadcode/BMAD-METHOD.git (push)
      ```

### Forked Repo: 
    - forked on July 23, 2025
    - last updated on July 23, 2025
    - https://github.com/grovejt/BMAD-METHOD
    - git pull https://github.com/grovejt/BMAD-METHOD.git

    - branches:
        - main
        - feature/enhance-architect-to-create-sequence-diagrams



### Syncing Upstream to Fork:
```shell
git checkout main
git fetch upstream

# To see what commits are in the upstream that you don't have:
git log HEAD..upstream/main --oneline
git log HEAD..upstream/main --pretty=format:"%h - %an, %ar : %s"

# See detailed differences between your main and upstream/main
git diff upstream/main
#See just the file names that have changed
git diff --name-only upstream/main
# See a summary of changes with stats
git diff --stat upstream/main

# Preview the merge (what would happen if you merged)
git merge-tree $(git merge-base main upstream/main) main upstream/main

# See a visual representation of the branch differences
git log --graph --oneline --decorate main upstream/main

# Pull the changes from upstream/main into your local main branch
git pull upstream main
git push origin main
```
# Syncing main to feature/enhance-architect-to-create-sequence-diagrams
```shell
git checkout feature/enhance-architect-to-create-sequence-diagrams
git merge main
git push origin feature/enhance-architect-to-create-sequence-diagrams
```






