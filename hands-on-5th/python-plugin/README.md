# Python特徴抽出プラグイン

今までC++で実装する必要のあった特徴抽出プラグインを、Pythonで記述できるようになりました。

本フォルダに配置してある各種ファイルは、次のような役割を持ちます。
- ARModel.ipynb: 時系列特徴抽出プラグインを試すデモ用Jupyter Notebook
- autoregressive.ipy: Jubatusで時系列分析を実現するためのPython特徴抽出プラグイン
- config.json: 時系列分析用の設定ファイル

本分析スクリプトの利用手順は次のとおりです。

1. PYTHONPATHを通す

    ```
    $ export PYTHONPATH=$PYTHONPATH:$(where autoregressive.py exists)
    ```

2. 回帰用のJubatusサーバを起動する

    ```
    $ jubaregression -f config.json -t 1000
    ```

3. Jupyter Notebookを起動する

    ```
    $ jupyter notebook
    ```

4. Jupyterをポチポチして結果を眺める
