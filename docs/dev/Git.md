tags: #git

# Git

links: [[dev/000 Index|Index]]

---

## Branch

Get local branches that are merged into main and thus can be deleted

```
git branch --no-contains main --merged main
```

Delete those branches

```
git branch --no-contains main --merged main | xargs git branch -d
```

Delete remote branch

```
git push origin --delete BRANCH
```

---
links: [[dev/000 Index|Index]]