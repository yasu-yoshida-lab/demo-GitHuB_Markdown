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
