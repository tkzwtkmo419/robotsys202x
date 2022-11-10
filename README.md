# robosys2022
ロボットシステム学の練習リポジトリ

# plusコマンド
![test](https://github.com/tkzwtkmo419/robosys2022/actions/workflows/test.yml/badge.svg)

## 目的
* 正しく計算が行われているかを判断する

## 使いかた
* 1 Ubuntuをインストール
* 2 Ubuntuの中でLinuxが使えるようにする
* 3 Pythonを使って以下のファイルを作る

  #!/usr/bin/python3
#SPDX-FileCopyrightText: 2022 Takumi Takazawa tkzwpen0419@outlook.jp
#SPDX-License=Identifier: GPL-3.0
import sys

ans = 0
for line in sys.stdin:
    try:
        ans += int(line)
    except:
        ans += float(line)

print(ans)

* 4 githubのリポジトリに.github/workflowsというディレクトリを作成
* 5 そこの中に.ymlという以下のファイルを作成
* 6 それらをすべてpushしてテストの結果を確認

## 必要なソフトウェア
* Python
  * テスト済み: 3.7~3.10

## テスト環境
* Ubuntu

## Pythonのバージョン
　3.10.4

## ライセンス

 このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます
© 2022 Takazawa takumi

