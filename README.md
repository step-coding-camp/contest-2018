STEP Coding Camp 2018 Programming Contest
=========================================

STEP Coding Camp 2018 で行われる Programming Contest で使うプログラムです。

ファイルの説明
============

プログラムは python3 を用いて書かれています。

`gomoku.py`
---------
サンプルコードです。このファイルで定義されている `Think()` を改造してもらいます。下にある `Input()`、`Output()`、`main()` は変更しないでください。また `Think()` の入出力のデータ形式も変更しないでください。

対戦中の情報を表示したい場合はコード中に定義されている `DebugPrint()` 関数を使ってください。理解している場合は標準エラー出力や `logging` を利用してもらっても構いません。

`server.py`
------------------
AI を対戦させるスクリプトです。

```
 $ ./server.py my_gomoku.py gomoku.py
```

のようにプログラムを 2 つ引数に与えると 1 つ目のプログラムを先攻(`O`)、2 つ目のプログラムを後攻(`X`)として対戦させます。また

```
 $ ./server.py my_gomoku.py
```

のように 2 つめのプログラムの指定を省略した場合は `gomoku.py` を後攻に指定したものとして対戦させます。

`test/`
--------
対戦相手のサンプルですが、`.pyc` になっているので中身は読めないようになっています。改造した AI の強さを測る目安にしてください。`server.py` の引数には通常の `.py` ファイルと同様に与えれば動きます。
`sample_medium.pyc` は `sample_hard.pyc` より少し弱いです。
