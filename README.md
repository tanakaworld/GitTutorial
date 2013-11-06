# GitTutorial

## Command
+ `$ git init`  //
+ `$ git add .`  // 
+ `$ git commit -a`  // 
+ `$ git commit -m "comment"`  // 
+ `$ git branch -a`  // ローカル・リモートブランチ表示
+ `$ git checkout <branch_name>`  // ブランチの切り替え
+ `$ git branch <branch_name>`  // 新規ブランチ作成
+ `$ git checkout -b <branch_name>`  // 新規ブランチ作成とブランチ切り替え
+ `$ git tag -a <tag_name> -m "comment"`  // タグの作成
+ `$ git fetch [repository_name]`  // 
+ `$ git merge [repository_name]`  //
+ `$ git merge [repository_name/branch_name]`  //
+ `$ git push [repository_name] [branch_name]`  // 
+ `$ git branch -d hoge`  // ローカルブランチ削除
+ `$ git push :hoge`      // リモートブランチ削除
+ `$ git rm -rf --cached [name]`  // トラック対象から除く（.gitignoreをaddした後に無効にする場合）
+ `$ git push origin [tag_name]` // tag の共有
+ `$ git push origin --tags` // ローカルリポのタグでリモートにないものすべてを転送
+ `$ git stash [save] [-m "comment"]` // 現在のワークツリーを一時的に保存する（uncommited changes だけど、checkout して後に commit したい場合など）
+ `$ git stash list`
+ `$ git stash pop [stash@{0}]` // 任意のスタッシュを復元
