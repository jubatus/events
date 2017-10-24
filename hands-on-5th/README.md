# 第5回Jubatusハンズオン

- 開催日時: 2017.11.01(WED)
- 開催場所: NTT-TX 品川オフィス
- 募集ページ: https://jubatus.connpass.com/event/67461/

## イベント用Slack登録のススメ

事前準備のインストールに躓いたり、イベント中にわからないことがあったら
Jubatusコミュニティメンバが質問にお応えします。

- 登録ページ: https://jubatus-event-slackin.herokuapp.com/
- slack: https://jubatus-event.slack.com/


## 事前準備 (DockerやVMを使わない場合)

### Jubatusのインストール

Jubatus公式ページを見ながらインストールしてください。

- 公式ホームページ: http://jubat.us/ja/quickstart.html

### Python依存パッケージのインストール

ハンズオンを実行するために、いくつかのPythonライブラリが必要になります。

```
$ pip install --upgrade pip
$ pip install Cython
$ pip install numpy scipy pandas matplotlib scikit-learn statsmodels jupyter jubatus jubakit embedded_jubatus
```

- scikit-learn >= 0.18 である必要がるので注意してください。

## 事前準備 (Dockerを使う場合)

```
$ docker pull jubatus/hands-on-5th
```

## 事前準備（VMを使う場合）

以下のURLからVirtualBox Imageを取得してください。Ubuntu 16.04で作成してあります。

- URL: 

VMは以下のアカウント/パスワードで入ることができます。

- アカウント名: jubatus
- パスワード: jubatus


