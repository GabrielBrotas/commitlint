## Commit Pattern
This repository contains the settings needed to create a commit pattern in the commitlint format

**Commit Available Prefix**
[build, chore, ci, docs, feat, fix, perf, refactor, revert, style, test]

Obs.: If you not start your commit with one of the followings prefix it will thrown an error

## Requirements
- npm 8.x

## How to Run
```bash
npx husky install ## setup husky on .git folder 
chmod a+x .husky/commit-msg ## add permision to execute script
```

