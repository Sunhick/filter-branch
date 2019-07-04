# filter-branch

git filter-branch

Remove the sensitive files from the git repository.

```shell
git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch passwords" \
  --prune-empty --tag-name-filter cat -- --all
```

Now force push the modified repo with history to the remote using -

```shell
git push origin --force --all
```
