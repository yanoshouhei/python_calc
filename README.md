# 計算機のプログラム

皆さんが応用プログラミングの授業後半で開発を行った計算機のプログラムの
作成見本です。

PySimpleGUIをインストールする必要があります。

# 動作準備

最初にコマンドプロンプトを立ち上げ、コマンドプロンプトでpythonが動作可能かを確認します。
下記のように、pythonのバージョンが表示されていればpythonが動作可能です。

```
$ python -V
Python 3.11.9
```

仮想環境を作成します。

```
 $ python -m venv venv 
```

作成した仮想環境をアクティブにします。

```
 $ ./venv/Scripts/activate
```

仮想環境にPySimpleGUIをインストールします。

```
 $ pip install pysimplegui==4.60.5
```

pythonコマンドの後にスクリプトファイルを指定することでプログラムを実行します。

```
 $ python python_calc.py
```

# レポジトリーのクローン

矢野先生のgithubレポジトリを自分のPCにコピーするためには、クローンを使います。

```
 $ git clone https://github.com/ShouheiYano2020/python_calc.git
```

python_calcというディレクトリが作成されその中に、矢野先生のリモートリポジトリと同じ内容がコピーされているはずです。

コピーしたディレクトリに移動します。

```
 $ cd python_calc
```

dir または　ls　などのコマンドを使ってディレクトリー内にファイルがコピーされていることを確認してみてください。

# ブランチの作成

もらってきた矢野先生のリモートブランチを編集したいと思いますが、
そのまえにブランチを作成し、ブランチで編集を行いましょう

```
 $ git branch test_branch
```

切り換え
```
 $ git checkout test_branch
```


確認
```
 $ git branch t
```

変更点を登録
```
 $ git add .
```

コミット
```
 $ git commit -m "README修正"
```


プッシュ

```
 $ git push -u origin test_branch
```

このとき、ユーザ名とパスワードを聞かれる。

ユーザ名は自分のユーザ名を入れてください。
パスワードには、GitHubの「Settings」→「Developer settings」→「Personal access tokens」→「Generate new token」から新しいトークンを生成します。
その後、HTTPS URLの認証でこのトークンを使用します。

なお、pushするするリモートブランチは

- https://github.com/ee40100x/pyrhon_calc.git

です。ee40100xは自分のユーザ名です。


こうすると、自分のgithubに新しくpython_calcというリモートリポジトリが作成されると思います。またそのブランチはbranch_ee4_00のみだと思います。

矢野先生のリポジトリにはそのブランチが接続されています。

- https://github.com/ShouheiYano2020/python_calc.git


そうなのです、ブランチは自分のgithubのプロジェクトとして作成され、矢野先生のgithubには接続された形になるのです。

なので、矢野先生のブランチにpushするのではなく、自分のサイトのgithubにpushすることを行っているのです。



