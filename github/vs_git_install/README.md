## Windows編
1. Gitインストール方法<br/>
    [こちらを参照](https://blog.djuggernaut.com/git-install/)
2. SSHでGitに接続する設定br/>
    https://qiita.com/coffee_g9/items/e1b9ab28cfa54f854308
3. 次のコマンドを実行して、gakken-itチーム内のリポジトリをclone出来たらgitの設定は完了です。<br/>
   `git clone git@github.com:gakken-it/git_study.git`<br />
4. VSCode インストール方法<br/>
    [こちらを参照](https://miya-system-works.com/blog/detail/105)
   
## Mac編
1. Gitインストール方法
  標準で付属していると思いますので、次のコマンドでインストールされていることを確認してください。<br/>
  `git --version`
  インストールされていない場合は、次のコマンドでインストールしましょう。
  `brew install git`
  
2. VSCode インストール方法<br/>
  * [こちらを参照](https://qiita.com/watamura/items/51c70fbb848e5f956fd6)<br/>
  * 拡張機能のインストールはやらなくて大丈夫です。
 
3. Gitの設定　
    * 公開鍵の設定
      * 次のコマンドで表示された内容をgakkenのアカウントに登録します。表示されたら3つ下を行ってください。<br/>
        `cat ~/.ssh/id_rsa.pub`<br/>
      * 何も表示されなかった場合は、次のコマンドで鍵を生成してください。ひたすらエンターを押していくと、鍵が生成されます。<br/>
        `mkdir ~/.ssh`<br/>
        `cd ~/.ssh`<br/>
        `ssh-keygen -t rsa`<br/>
      * 鍵のパーミッションを変更します。<br/>
        `chmod 600 ~/.ssh/id_rsa`<br/>
      * 再び、次のコマンドを実行して、鍵を表示してください。<br/>
        `cat ~/.ssh/id_rsa.pub`<br/>
      * 表示された鍵を次のページの「秘密鍵をローカルに、公開鍵をGitHubに登録する」以降を参考にして設定します。<br/>
        [こちらを参照](https://qiita.com/nishina555/items/127f691a9e11e0fc5999)<br/>
      * 次のコマンドを実行して、gakken-itチーム内のリポジトリをclone出来たら成功です。<br/>
        `cd [好きな場所]` ディレクトリの移動<br/> 
        `git clone git@github.com:gakken-it/git_study.git`<br/>
       
     * ローカルアカウントの設定を行います。git_studyフォルダに移動し、次のコマンドを実行してローカルアカウントを設定してください。
        ```
        git config --local user.name "Githubのユーザー名"
        git config --local user.email "自分のgakkenメールアドレス。"
        ```
