# demo-GitHuB
このページではGitHuBの利用で必要な環境構築とGitのコマンドについて説明をおこないます。
## 環境構築
GitHuBの利用にはGitのインストールが必要です。各OSごとに方法が異なるので紹介します。
#### Mac
MacではHomebrewを用いたインストールが簡単にインストールすることができます。そもそもHomebrewがインストールされていない場合は以下のコマンドでインストールできます。

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

その後、以下のコマンドでGitをインストールすることができます。

```
brew install git
```

#### Windows
Windows では以下のサイトで「Download」ボタンを押して、インストーラーをダウンロードしてください。  
<a href="https://gitforwindows.org/">Git for Windows</a>  
各種細かい設定は以下のサイトを読んでください。  
<a href="https://qiita.com/manabu-watanabe/items/ecf1b434baf305adaa00">いまさらGit for Windowsのインストール、GitHubに接続してみた。</a>  

#### Linux
OSによってインストールのコマンドが多少異なります。Ubuntu系のOSを利用している人は以下のコマンドでインストールできます。

```
sudo apt install git-all
```

Cent系のOSを利用している人は以下のコマンドでインストールしてください。

```
sudo yum install git-all
```

## コマンドについて
リモートリポジトリをコピーしてローカルリポジトリを作成する際は``git clone``を利用します。``git clone``後はリモートリポジトリのURLを貼り付けてください。例えば、今見ている記事をローカルに落としたい場合は以下のように書きます。

```
git clone https://github.com/yasu-yoshida-lab/demo-GitHuB_Markdown.git
```

ローカルに落としたMarkdownファイル等を編集や新しくファイルを作成した場合は以下のコマンドでファイルの状況を確認することができます。ファイル名が赤色のものはまだGitに管理されていない状態です。

```
git status
```

編集したファイルや新規作成したファイル等をGitの管理下におく場合は``git add <ファイル名>``となります。全ファイルをGitの管理下に置く場合は以下のコマンドを利用してください（これを「ステージング」と呼びます）。ステージング後に``git status``を行うとファイル名が緑色になります。

```
git add .
```

この状態ではまだローカルリポジトリにファイルが保存されていないので、コミットコマンドを実行する必要があります。その際、メッセージで変更点や追加点のメモを残すことができます。例えば以下のコマンドのように何度目のコミットか記録するなどがあります。

```
git commit -m "1st commit"
```

ローカルリポジトリに保存ができたらリモートリポジトリ先にアップロードします。アップロードには以下のコマンドを用います。「origin」はリモートサーバーを意味します。


