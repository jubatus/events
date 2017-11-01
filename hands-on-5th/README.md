# 第5回Jubatusハンズオン

- 開催日時: 2017.11.01(WED)
- 開催場所: NTT-TX 品川オフィス
- 募集ページ: https://jubatus.connpass.com/event/67461/

## イベント用Slack登録のススメ

事前準備のインストールに躓いたり、イベント中にわからないことがあったら
Jubatusコミュニティメンバが質問にお応えします。

- 登録ページ: https://goo.gl/BSmynr
- slack: https://jubatus-event.slack.com/

## 事前準備：VMを使う場合

以下のURLからVirtualBox Imageを取得してください。Ubuntu 14.04で作成してあります。
http://download.jubat.us/event/1.0.5_ubuntu14.04/
- Jubatus-Handson.zip で解凍に失敗した場合には、Jubatus-Handson-mirror.zip を試してみてください。

※ アカウント名: jubatus、パスワード: jubatus

ハンズオン当日までに、VMが起動できることを確認しておいてください。

## 事前準備：Dockerを使う場合

### Dockerイメージのダウンロード
```
$ docker pull jubatus/hands-on-5th
```

### コンテナの起動確認
```
$ docker run -p 8888:8888 -it jubatus/hands-on-5th /bin/bash
$ jupyter notebook &
```
上記のコマンドを実行した後に、ブラウザで http://127.0.0.1:8888 にアクセスし、Jupyterが起動していることを確認しておいてください。


## 事前準備：自分の環境にJubatusをインストールする場合

### Jubatusのインストール

Jubatus公式ページを見ながらインストールしてください。

- 公式ホームページ: http://jubat.us/ja/quickstart.html

### Python依存パッケージのインストール

ハンズオンを実行するために、いくつかのPythonライブラリが必要になります。
なお、ハンズオンの特徴抽出プラグインの説明でPython2系を利用しますので、Python2で実行されることをオススメします。
（※ Python2系で上手くインストールできない場合には、Python3系でも試してみてください）

```
$ pip install --upgrade pip
$ pip install Cython
$ pip install numpy scipy pandas matplotlib scikit-learn statsmodels jupyter jubatus jubakit embedded_jubatus
```

### GitHubリポジトリの取得

ハンズオンスクリプトは以下のリポジトリから取得できますので、事前にcloneしておくことをオススメします。

```
$ git clone https://github.com/jubatus/events
```

### PYTHONPATHを通す

Python特徴抽出プラグインを利用した実験を試したい場合には、
`events/hands-on-5th/python-plugin`にPYTHONPATHを通しておいてください。

