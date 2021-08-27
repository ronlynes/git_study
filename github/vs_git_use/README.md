## 初めに
このページでは、VSCode上でのgitの使い方を解説します。

### 拡張機能のインストール

次の拡張機能をインストールしてください。
* Git Graph<br/>
VSCode上でGitログが見れるようになります。
<div align="center">
    <img src="img/git_graph.png" width="600px" style="margin:50px">
</div>

* Git Lens<br/>
commitメッセージがコード上に表示されるようになります。

<div align="center">
    <img src="img/git_lens.png" width="600px" style="margin:50px">
</div>

* gitignore<br/>
言語に応じたgitignoreを自動的に作成してくれます。
<div align="center">
    <img src="img/gitignore.png" width="600px" style="margin:50px">
</div>

## 基本的な操作方法
Gitの操作は上から3番目のアイコンをクリックして表示されるウィンドウで操作する.
<div align="center">
    <img src="img/git_icon.png" width="600px" style="margin:50px">
</div>

### Git Add & Commit
赤枠の更新ボタンを押す。
<div align="center">
    <img src="img/git_add0.png" width="600px" style="margin:50px">
</div>
変更したファイルがあると、このように変更タブの下に表示される。
test.pyの変更を、Git addしたい時は赤枠のプラスボタンを押す。
<div align="center">
    <img src="img/git_add1.png" width="600px" style="margin:50px">
</div>
すると、ステージングされている変更に追加される。<br/>
この変更をcommitしたい時には、[メッセージをここに入力する]にコミットメッセージを書く。<br/>
最後に赤枠のチェックマークを押すとコミット完了。
<div align="center">
    <img src="img/git_commit.png" width="600px" style="margin:50px">
</div>

### Git reset: コミットの取り消し
左下にある、COMMITSを押すと次のように表示される。
<div align="center">
    <img src="img/git_reset1.png" width="600px" style="margin:50px">
</div>
先ほど追加した、コミットを選択し、赤枠の戻るマークをクリックすると、コミットを取り消すことができる。
<div align="center">
    <img src="img/git_reset2.png" width="600px" style="margin:50px">
</div>

### Git Push: リモートに変更をアップロード
左下にある、COMMITSを押すと次のように表示され、Change to push to origin on Githubを選択する。<br/>
赤枠の、アップロードボタンを押す。
<div align="center">
    <img src="img/git_push1.png" width="600px" style="margin:50px">
</div>
すると、次のポップアップが表示され、Pushをクリック。
<div align="center">
    <img src="img/git_push2.png" width="600px" style="margin:50px">
</div>

### Git Pull: リモートの変更をローカルに適用
画面左下にある、赤枠のボタンをクリックする。
<div align="center">
    <img src="img/git_pull.png" width="600px" style="margin:50px">
</div>
すると、次のような警告ポップアップが表示され、OKボタンを押すと、リモートの変更をローカルに適用させることができる。
<div align="center">
    <img src="img/git_pull2.png" width="600px" style="margin:50px">
</div>

### Git branch: ブランチを作成
今いるブランチは赤枠のところに表示されている。
<div align="center">
    <img src="img/git_branch0.png" width="600px" style="margin:50px">
</div>
赤枠をクリックすると、次のポップアップが表示される。
<div align="center">
    <img src="img/git_branch1.png" width="600px" style="margin:50px">
</div>
新しい分岐の作成を選択する。作成する分岐の名前を入力してエンター。
<div align="center">
    <img src="img/git_branch2.png" width="600px" style="margin:50px">
</div>
ブランチを作成でき、赤枠を確認すると、新しく作成したブランチに移動していることがわかる。
<div align="center">
    <img src="img/git_branch3.png" width="600px" style="margin:50px">
</div>

### Git merge: ブランチをmergeする
Macなら Command + Shift + P, Windowsなら Ctrl + Shift + Pを押し、「merge」と検索する。そして、「Git: ブランチをマージ」を選択。
<div align="center">
    <img src="img/git_merge1.png" width="600px" style="margin:50px">
</div>
現在いるブランチにmergeしたいブランチを選択してクリックすると、mergeされる。
<div align="center">
    <img src="img/git_merge2.png" width="600px" style="margin:50px">
</div>

### Git pull request
リポジトリのWebを開く
赤枠のPull requestを選択する。
<div align="center">
    <img src="img/git_pullrequest1.png" width="600px" style="margin:50px">
</div>
New pull requestボタンを押す。
<div align="center">
    <img src="img/git_pullrequest2.png" width="600px" style="margin:50px">
</div>
baseにmerge先(develop), compareにmergeするブランチ(features/xx)を選択する.
<div align="center">
    <img src="img/git_pullrequest3.png" width="600px" style="margin:50px">
</div>
Create pull requestボタンを押す。
<div align="center">
    <img src="img/git_pullrequest4.png" width="600px" style="margin:50px">
</div>
Pull requestのタイトルと、変更内容を記述し、右下のCreate pull requestを押す。
<div align="center">
    <img src="img/git_pullrequest5.png" width="600px" style="margin:50px">
</div>
Merge pull requestボタンの右側にある、プルダウンをクリックし、Squash and mergeを選択する。
<div align="center">
    <img src="img/git_pullrequest6.png" width="600px" style="margin:50px">
</div>
Squash and mergeになっていることを確認したら、Squash and mergeボタンを押す。
<div align="center">
    <img src="img/git_pullrequest7.png" width="600px" style="margin:50px">
</div>
コミットメッセージを押したら、Confirm squash and mergeボタンを押して、mergeする。
<div align="center">
    <img src="img/git_pullrequest8.png" width="600px" style="margin:50px">
</div>
最後に、mergeしたブランチをDelete branchボタンを押して削除すれば、完了。
<div align="center">
    <img src="img/git_pullrequest9.png" width="600px" style="margin:50px">
</div>

## その他(また今度)

### コンフリクト解消方法
### 指定した範囲だけGit add
### Git stash: 変更を一時退避
### Git rebase -i: コミットをまとめる
