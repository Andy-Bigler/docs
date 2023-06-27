tags: #git
links: [[dev/000 Index|Index]]

---
# Git

## Branch

Get local branches that are merged into main and thus can be deleted

```
git branch --no-contains main --merged main
```

Delete those branches

```
git branch --no-contains main --merged main | xargs git branch -d
```

---
links: [[dev/000 Index|Index]]