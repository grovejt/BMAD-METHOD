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
git pull upstream main
git push origin main
```








