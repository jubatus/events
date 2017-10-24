## Jubaclassifierハンズオン

Jubatus本に準拠しながら、classifierのハンズオンを行います。基本的な流れは同じですが、データやパラメータなどを少々変えています。

本フォルダの各種ファイルの役割は以下の通りです。

- hands_on.ipynb : jubaclassifierを試すデモ用のJupyter Notebook
- config : jubaclassifierの設定を入れるためのディレクトリ。
    - `linear.json`には線形分類器用の設定を書いている。本ハンズオンではlinear.jsonを用いる。
    - `nonlinear.json`には非線形分類器用の設定を書いている。
- data : 今回使用するデータを格納しているディレクトリ。データ元は->[default of credit card clients Data Set](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)


ハンズオンの利用手順は以下のとおりです。
1. 分類用のJubatusサーバを起動する  
```
jubaclassifier -f config/linear.json -t 1000&
``` 

2. Jupyter notebookを起動する
```
jupyter notebook
```

3. Jupyterを実行しながら結果を眺める