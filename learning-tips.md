This article records some small tips.

1. tree: 查看目录结构
```bash
brew install tree
```

2. git pull : 
    **fatal: refusing to merge unrelated histories**
```bash
git pull origin master --allow-unrelated-histories
```

3. git add: 
```bash
git remote add origin your_remote_repository
git push -u origin master
```

4. git changing a remote's URL
```bash
git remote -v: list the existing remotes
git remote set-url [--add] <name> <newurl>
git remote set-url [--delete] <name> <newurl>
git remote set-url [--push] <name> <newurl> [<oldurl>]
```