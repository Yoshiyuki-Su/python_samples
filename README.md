# Pythonで作ったサンプルプログラム群です。
- [Pythonで作ったサンプルプログラム群です。](#pythonで作ったサンプルプログラム群です)
  - [コマンドライン引数に指定した件数分の文字列を表示するプログラム](#コマンドライン引数に指定した件数分の文字列を表示するプログラム)
    - [内容](#内容)
    - [使い方](#使い方)
  - [九九の表を表示するプログラム](#九九の表を表示するプログラム)
    - [内容](#内容-1)
    - [使い方](#使い方-1)
  - [縦10×横10の逆三角形、三角形を表示するプログラム](#縦10横10の逆三角形三角形を表示するプログラム)
    - [内容](#内容-2)
    - [使い方](#使い方-2)
  - [+1だけで四則演算処理するプログラム](#1だけで四則演算処理するプログラム)
    - [内容](#内容-3)
    - [引数について](#引数について)
    - [演算子](#演算子)
    - [使い方](#使い方-3)
  - [占いプログラム](#占いプログラム)
    - [内容](#内容-4)
    - [使い方](#使い方-4)
  - [じゃんけんプログラム](#じゃんけんプログラム)
    - [内容](#内容-5)
    - [使い方](#使い方-5)


## コマンドライン引数に指定した件数分の文字列を表示するプログラム
### 内容
```md
引数に指定した件数分の文字列を表示し、指定しない場合は「引数が未入力です。」と表示するプログラム
```
### 使い方
```md
python commandline_args.py Python Ruby Java
「Python」が入力されました。
「Ruby」が入力されました。
「Java」が入力されました。
```

## 九九の表を表示するプログラム  
### 内容
```md
九九の表を表示するプログラム  
```
### 使い方
```md
python multiplication_table.py

1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 

2 | 4 | 6 | 8 | 10 | 12 | 14 | 16 | 18 | 

3 | 6 | 9 | 12 | 15 | 18 | 21 | 24 | 27 | 

4 | 8 | 12 | 16 | 20 | 24 | 28 | 32 | 36 | 

5 | 10 | 15 | 20 | 25 | 30 | 35 | 40 | 45 | 

6 | 12 | 18 | 24 | 30 | 36 | 42 | 48 | 54 | 

7 | 14 | 21 | 28 | 35 | 42 | 49 | 56 | 63 | 

8 | 16 | 24 | 32 | 40 | 48 | 56 | 64 | 72 | 

9 | 18 | 27 | 36 | 45 | 54 | 63 | 72 | 81 | 
```

## 縦10×横10の逆三角形、三角形を表示するプログラム

### 内容
```md
縦10×横10の逆三角形、三角形を表示するプログラム
```
### 使い方
```md
python triangle_representation.py
●●●●●●●●●●●
●●●●●●●●●●
●●●●●●●●●
●●●●●●●●
●●●●●●●
●●●●●●
●●●●●
●●●●
●●●
●●
●

●
●●
●●●
●●●●
●●●●●
●●●●●●
●●●●●●●
●●●●●●●●
●●●●●●●●●
●●●●●●●●●●
●●●●●●●●●●●
```

## +1だけで四則演算処理するプログラム

### 内容
```md
+1だけで四則演算処理するプログラム
引数に指定した四則演算子と数値で計算を実施する。
指定しない場合は「引数が未入力です。」と表示する。
四則演算子以外だと「演算子(+,-,*,/)を入力してください。」と表示する。
```
### 引数について
- 第一引数：下記の四則演算子を入力
- 第二引数：計算する数値
- 第三引数：計算する数値

### 演算子
- 足し算：+
- 引き算：-
- 掛け算：*
- 割り算：/

### 使い方
```md
python commandline_args.py + 10 2
operator: +
answer: 12

python commandline_args.py - 10 2
operator: -
answer: 8

python commandline_args.py * 10 2
operator: *
answer: 20

python commandline_args.py / 10 2
operator: /
answer: 5
```

## 占いプログラム  
### 内容
```md
0～10のランダムな整数を生成する。
生成した値によって下記をコンソールに表示する。
10の場合は「大吉」
6以上10未満の場合は「中吉」
3以上6未満の場合は「吉」
1以上3未満の場合は「凶」
0の場合は「大凶」
```

### 使い方
```md
python fortune.py
10
【大吉】です。

python fortune.py
7
【中吉】です。

python fortune.py
3
【吉】です。

python fortune.py
1
【凶】です。

python fortune.py
0
【大凶】です。
```

## じゃんけんプログラム  
### 内容
```md
仕様
プログラムが起動したらずっとじゃんけんが出来る。
じゃんけんをやめる場合は下記のパラメータを入力する。
じゃんけんの出す手は下記のパラメータから入力する。
成績表示機能を作成し、下記のパラメータ入力時にプログラムが起動していた際の成績を表示する

パラメータ
1:グー、2:チョキ、3:パー、4:成績を表示、0:じゃんけん終了

判定スコアの定義
グー：0点、チョキ：1点、パー：2点
判定スコア
じゃんけんの判定スコア = [プレイヤーの手 - コンピュータの手 + 3] Mod 3
判定スコアが0の時は引き分け、1の時はプレイヤーの負け、2の時はプレイヤーの勝ち

勝ったら+1点
```
### 使い方
```md
python rock_scissors_paper.py

----------------------------
じゃんけんスタート
下記の数値を入力してください。
0:グー 1:チョキ 2:パー 3:成績を表示 4:じゃんけん終了
じゃんけんに勝ったら+1点
----------------------------
>>> 0
あなたはグーを出しました。
コンピュータはグーを出しました。
じゃんけんの結果：あいこ

----------------------------
じゃんけんスタート
下記の数値を入力してください。
0:グー 1:チョキ 2:パー 3:成績を表示 4:じゃんけん終了
じゃんけんに勝ったら+1点
----------------------------
>>> 1
あなたはチョキを出しました。
コンピュータはパーを出しました。
じゃんけんの結果：勝ち

----------------------------
じゃんけんスタート
下記の数値を入力してください。
0:グー 1:チョキ 2:パー 3:成績を表示 4:じゃんけん終了
じゃんけんに勝ったら+1点
----------------------------
>>> 2
あなたはパーを出しました。
コンピュータはパーを出しました。
じゃんけんの結果：あいこ

----------------------------
じゃんけんスタート
下記の数値を入力してください。
0:グー 1:チョキ 2:パー 3:成績を表示 4:じゃんけん終了
じゃんけんに勝ったら+1点
----------------------------
>>> 3
-----成績表-----
3 戦
スコア：1 点
勝率：33 %

----------------------------
じゃんけんスタート
下記の数値を入力してください。
0:グー 1:チョキ 2:パー 3:成績を表示 4:じゃんけん終了
じゃんけんに勝ったら+1点
----------------------------
>>> 4

```
