# filter-branch

git filter-branch


```shell
git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch passwords" \
  --prune-empty --tag-name-filter cat -- --all
```
