## はじめに

このパッケージは中澤研究室で開発しているROSパッケージです。

`nakbot_ROS`パッケージ内に各々が開発した機能を追加していくような形を想定しています。`nakbot_ROS`ディレクトリの中に自分のディレクトリを作成し、そこに自作のコードを追加していってください。

## 開発環境

- ubuntu 18.04
- ROS melodeic
- iai-kinect2

iai-kinect2等のセットアップは[こちら](https://qiita.com/keinko/items/5ed026c46f6b308701af)を参照してください。

## インストール

developブランチをインストールするようにしてください。よく分からない人は以下のコマンドでインストールできます。

```
$ cd ~/catkin_ws/src
$ git clone https://github.com/kei15/nakbot_ROS/tree/develop
```

インストールが完了したら以下のように「好きな名前」でディレクトリを作成し、そこにコードを書いてください。　

```
$ cd nakbot_ROS
$ mkdir 好きな名前
```

## 実行テスト

ターミナルを3つ開き、以下を実行してください。

ターミナル1
```
$ roscore
```

ターミナル2
```
$ roslaunch kinect2_bridge kinect2_bridge.launch
```

ターミナル3
```
$ rosrun kinect2_viewer kinect2_viewer kinect2 sd cloud
```

## 開発
