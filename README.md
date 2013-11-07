# GitTutorial

## Command
+ `$ git init`
+ `$ git add .`
+ `$ git commit -a`
+ `$ git commit -m "comment"`  // コメント付きコミット
+ `$ git branch -a`  // ローカル・リモートブランチ一覧表示
+ `$ git branch <branch_name>`  // 新規ブランチ作成
+ `$ git branch -d hoge`  // ローカルブランチ削除
+ `$ git push :hoge`      // リモートブランチ削除
+ `$ git rm -rf --cached [name]`  // トラック対象から除く（.gitignoreをaddした後に無効にする場合）
+ `$ git checkout <branch_name>`  // ブランチの切り替え
+ `$ git checkout -b <branch_name>`  // 新規ブランチ作成とブランチ切り替え
+ `$ git checkout -b <local_branch_name> <remote_branch_name>`  // master以外のリモートブランチ取得
+ `$ git tag -a <tag_name> -m "comment"`  // タグの作成
+ `$ git fetch [repository_name]`  // 
+ `$ git merge [repository_name]`  //
+ `$ git merge [repository_name/branch_name]`  //
+ `$ git pull [repository_name/branch_name]`  // fetch, merge を同時にやる
+ `$ git push [repository_name] [branch_name]`
+ `$ git push origin [tag_name]` // tag の push
+ `$ git push origin --tags` // ローカルリポのタグでリモートにないものすべてを転送
+ `$ git stash [save] [-m "comment"]` // 現在のワークツリーを一時的に保存する（uncommited changes だけど、checkout して後に commit したい場合など）
+ `$ git stash list`
+ `$ git stash pop [stash@{0}]` // 任意のスタッシュを復元

## [Git-Flow](http://danielkummer.github.io/git-flow-cheatsheet/index.ja_JP.html "GitFlow")

## Tips

### .gitignore
+ [VisualStudioで.csprojがコンフリクトしないように](http://stackoverflow.com/questions/13479294/why-are-my-csproj-files-getting-messed-up-after-a-git-rebase)

### Alias

以下のコマンドでエイリアスが作成できる

`git config --global alias.<short-cut-command> "<normal-command>"`

| Normal | ShortCut | Command Detail |
|:-----------|------------:|:------------:|
| branch -a     | br-a |    全ブランチ表示    |
| commit -a | cm-a | コミット（Vimでコメントを書く）|
| status | st | Status |
| log --graph --all --color --pretty='%x09%h %cn%x09%s %Cred%d%Creset'| log-all | SourceTree |
