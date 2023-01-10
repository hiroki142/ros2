![test](https://github.com/hiroki142/mypkg/actions/workflows/test.yml/badge.svg)
# 説明
ROS2 パッケージ  
## ノード
* talker
  * パブリッシャーを持ち、0.5秒ごとにカウントアップされる数値を送信するノード
* listener
  * サブスクライバーを持ち、talkerで送信されたメッセージを受け取り端末に表示するノード

## トピック
* countup
  * この名前のトピックを通してtalkerとlistenerは通信している。  メッセージの型はInt16

# 実行方法
次の操作はROS2ワークスペースのトップディレクトリで行う
```
$ colcon build
$ . install/setup.bash
$ . install/local_setup.bash
$ ros2 launch mypkg talk_listen.launch.py
```

# 必要環境
* ROS2
* Python 3

# テスト済み動作環境
* ROS2 Humble
* Ubuntu 22.04
* Python 3.10.6

# ブランチ
* メインブランチ
  * master

# ライセンス
* このソフトウェアパッケージは、3条項BSDライセンスの下、再配布及び使用が許可されます。
  * [LICENCE](https://github.com/hiroki142/mypkg/blob/master/LICENSE)
* このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
  * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)
* © 2023 Hiroki Nukui

