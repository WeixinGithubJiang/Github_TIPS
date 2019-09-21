# Github_TIPS
Github tips for me

## 1. push file from local to the server

> Check if there is anything changed since last checkpoint
```bash
git status
```

> Select all changes/or part of the changes
```bash
git add *
git add file
```
> Check if selected changes are as expected
```bash
git status
```


> Confirm all changes and add some commits
```bash
git commit -m "message"
```

> Upload to the server
```bash
git push origin master
```

> Clone an existing environment
```bash
conda create --name clone_env_name --clone existing_env_name
```

## 2. download codes from the server
> if start from scratch, clone every bits
```bash
git clone address
``` 

> if some updates happened in the server, download the updates
```bash
git pull
``` 
`

## 3. Add tags for each commit
> check existing tags
```bash
git tag
```

> add tag directly after commit
```bash
git tag tag_name
```

> check commit history
```bash
git log --pretty=oneline --abbrev-commit
```


> add tag to one specific commit
```bash
git tag tag_name commit_id
or
git tag -a tag_name -m "message" commit_id
```

> check what changes have happened for one tag
```bash
git show tag_name
```

> remove tag locally
```bash
git tag -d tag_name
```

> upload tag to the server
```bash
git push origin tag_name (one tag)
git push origin --tag (all tags)
```

> remove tag in the server
```bash
git tag -d tag_name (delete local tag)
git push origin :refs/tags/tag_name (sync to the server)
```

> switch to different tag
```bash
git checkout tag_name
```
