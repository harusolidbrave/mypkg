# mypkg
これは、2つのノード間で基本的な通信を行うROS 2のパッケージです。

talkerノードから `countup` トピックにパブリッシュされたデータをlistenerノードがサブスクライブします。

![test](https://github.com/harusolidbrave/mypkg/actions/workflows/test.yml/badge.svg)

## 実行方法

下記のコマンドを実行し、`talk_listen.launch.py`を使用してトピックのパブリッシャ(talker)とサブスクライバ(listener)を同時に起動します。

listenerは、talkerから受け取ったカウントを表示します。
   ```bash
   $ ros2 launch mypkg talk_listen.launch.py
   ```

## 実行結果
   ```bash
    [listener-2] [INFO] [1703337477.964537567] [listener]: Listen: 0
    [listener-2] [INFO] [1703337478.464602186] [listener]: Listen: 1
    [listener-2] [INFO] [1703337478.964281611] [listener]: Listen: 2
    [listener-2] [INFO] [1703337479.464469949] [listener]: Listen: 3
    [listener-2] [INFO] [1703337479.964351436] [listener]: Listen: 4
   ```
## トピック

**countup**
: 16ビットの符号付き整数 カウントアップデータ


## 必要なソフトウェア

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
