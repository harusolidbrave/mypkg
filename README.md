# ROS 2マイパッケージ
これは、2つのノード間で基本的な通信を行うROS 2のパッケージです。

talkerノードから `countup` トピックにパブリッシュされたデータをlistenerノードがサブスクライブします。

![test](https://github.com/basiliskv/ros2_mypkg/actions/workflows/test.yml/badge.svg)

## 実行方法

   下記のコマンドを実行して、`talk_listen.launch.py`を使用してトピックのパブリッシャ(talker)とサブスクライバ(listener)を同時に起動します。

   ```bash
   $ ros2 launch mypkg talk_listen.launch.py
   ```

## 実行結果
   listenerは、talkerから受け取ったカウントを表示します。
   ```bash
    [INFO] [listener]: Listen: 1, Time: 2023-12-13 10:27:21
    [INFO] [listener]: Listen: 2, Time: 2023-12-13 10:27:21
    [INFO] [listener]: Listen: 3, Time: 2023-12-13 10:27:22
   ```
## トピック

   **countup**
      : 16ビットの符号付き整数 カウントアップデータ


## ソフトウェア要件

このパッケージを使用するには、以下のソフトウェアが必要です。

- Python 3
- ROS 2

## テスト環境

このパッケージは以下の環境でテストされています。

- Ubuntu 22.04.3 LTS

## ライセンス
  * このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  * このパッケージのコードの一部は，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
      * [https://ryuichiueda.github.io/my_slides/robosys_2022/lesson7.html#/](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson4.html#/)
      * [https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson5.html#/)
      * [https://ryuichiueda.github.io/my_slides/robosys_2022/lesson9.html#/](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson6.html#/)
      * [https://ryuichiueda.github.io/my_slides/robosys_2022/lesson10.html#/](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson6.html#/)
      * [https://ryuichiueda.github.io/my_slides/robosys_2022/lesson11.html#/](https://ryuichiueda.github.io/my_slides/robosys_2022/lesson6.html#/)
