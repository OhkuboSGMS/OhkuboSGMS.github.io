---
title: Portfolio
---

## 名前

大久保 成将 (Okubo Shigemasa)

{{<figure src="chao.jpg" width="35%" float="right">}}

## 簡単な自己紹介

```
仕事では主にpython 
ライブラリとしては OpenCV,Open3D,numpy,pytorch等を使用してCV系をメインで仕事しています．
趣味で flutter(dart),Android(kotlin)等でアプリ作成など

 仕事では，深層学習を利用したデスクトップアプリケーションの研究，開発に従事．
 主に機械学習系の案件を行っています.　

学生の頃はUnity(C#)やAndroid(Java,Kotlin),flutterを使用してアプリ等を作成しました．
```

## 公表物

 公開しているアプリ一覧
 
| プラットフォーム | リンク|
| --- | --- |
| Android| https://play.google.com/store/apps/developer?id=homura+LLC |
| iOS | https://apps.apple.com/jp/developer/homura-llc/id1236637936|

### 最近書いたブログ記事
 [whisper+voicevoxでポッドキャストを変える](https://ohkubosgms.hatenablog.com/entry/whiser_voicevox)
 
### 最近のOSS活動
 Kivyを使った，CV系検出，分類等のデモアプリの作成

 [![OhkuboSGMS/NullA - GitHub](https://gh-card.dev/repos/OhkuboSGMS/NullA.svg)](https://github.com/OhkuboSGMS/NullA)
 
 opencv-pythonで日本語の描画可能なカスタムビルド.

 [![OhkuboSGMS/opencv-python-freetype2 - GitHub](https://gh-card.dev/repos/OhkuboSGMS/opencv-python-freetype2.svg)](https://github.com/OhkuboSGMS/opencv-python-freetype2)

　なにか色々試したサンドボックス

 [![OhkuboSGMS/sandbox - GitHub](https://gh-card.dev/repos/OhkuboSGMS/sandbox.svg)](https://github.com/OhkuboSGMS/sandbox)

## 言語年数

| 言語 | 年数| 
| --- | --- |
|Python |5|
|Dart |2|
|kotlin |2|
|Cython | 1|

## Link

* [Qiita](https://qiita.com/Alt_Shift_N)
* [Github](https://github.com/OhkuboSGMS)
* [Mail](mailto:ginger.os777146th@gmail.com)
* [Zenn](https://zenn.dev/alt_shift_n)
* [Blog](https://ohkubosgms.hatenablog.com/)

## 略歴

- 2018年 熊本大学工学部情報電子工学系学科 卒業
- 2020年 熊本大学大学院自然科学教育部情報工学教育プログラム 卒業
- 2020年 4月 [ネクストシステム株式会社](https://www.next-system.com/)入社 ~ 現職

## 職歴詳細

## ネクストシステム

### 2020年4月 ~ 10月

[案件]Unity ml-agentsを用いた衝突回避移動エージェントの開発

#### 技術スタック
 
* git
* Unity(C#)
* [FinalIK](http://root-motion.com/)
* python
* pytorch
* [baselines](https://github.com/openai/baselines)

<details>
  <summary>詳細</summary>

[Unity ml-agents](https://github.com/Unity-Technologies/ml-agents)を使用して，6軸ロボットアームの衝突回避エージェント作成.
バージョンは [Beta 0.15.0](https://github.com/Unity-Technologies/ml-agents/releases/tag/0.15.0)付近を使用.

#### 概要

6軸ロボットの先端を目標に対して障害物を避けるように移動するエージェントを強化学習を用いて汎用的なモデルを作成する．

#### 具体的な内容

各アクチュエータの加速度を行動として，ロボットアームを移動させる．
Unityの物理環境内において，衝突判定のシミュレーションを行い，学習する．
状態は各アクチュエータの角度，レイの衝突判定などを使用．

#### チーム構成

| 役割 | 人数|
| --- | --- |
| マネージャ | 1 |
| エンジニア | 2 | 

#### 結果
プロジェクトは入社時に既に進行中のプロジェクトで途中から，強化学習の担当として参加．
 
ある程度決まった状況では回避行動が可能になったが汎用的な動きを学習はできなかった．
Unityでデフォルトで用意されている学習アルゴリズムでトライするに終わったため，より様々な手法を調査，論文等もロボットアームに関連する
情報をより集めたうえで，どう始めるかも含めて検討していければより良い結果が残せたのではないかと考えられる.



当時のml-agentドキュメントを翻訳した記事: [リンク](https://qiita.com/Alt_Shift_N/items/2c37fbb26d739b7f3046)
</details>

### 2020年10月 ~ 11月

[案件]Carlaを用いたCGによる衝突状況再現データセットによる物体認識.

#### 技術スタック

* git
* docker
* python
* keras
* [CARLA](https://carla.org/)
* pyQt


<details>
  <summary>詳細</summary>

#### 概要

車載カメラによる発生しづらいシチュエーションデータをCGによる作成,精度向上検証.

途中参加.

#### 具体的な内容

接触事故といった現実では 収集が難しい画像データを
Unreal Engine製の自動運転フレームワークワークであるCARLAを用いて，現実的なCGデータとして生成．

生成したCGデータを元データにミックスすることで精度向上を図る．

主に，精度向上の指標確認機能，データセット品質確認，統計情報収集機能等を作成．

#### チーム構成

| 役割 | 人数|
| --- | -- |
| マネージャ | 1 |
| エンジニア | 3 |
| CGエンジニア| 1 |

#### 結論

このプロジェクトもまた途中参加のプロジェクトでプチ炎上気味だった．
現実世界の映像とCG世界の間の誤差が大きく，目的となる現実世界での検出精度がなかなか上がらなかった．

プログラム自体のバグ等もあり，前提とする環境自体の間違いやアノテーションの特殊性など要因となりうる原因は
多岐にわたるため，それぞれについて報告して完了．

</details>

### 2021年12月 ~ 2月

[案件]Open3Dを用いた点群による物体形状の検索機能

#### 技術スタック

* python
* Open3D

<details>
  <summary>詳細</summary>

#### 概要

ICP位置合わせやFPFH特徴量等の古典的なアルゴリズムを用いて，物体形状検索システムを開発.

#### 具体的な内容

3Dメッシュデータ間の比較可能な機能を検討，作成．
検索が可能になることによって，メッシュデータ付随する付加情報を取得可能．
新規メッシュデータを作成時に以前のデータを参考にできるシステムが作成可能になる．

Open3Dに実装されている位置合わせアルゴリズム，KDTree,FLANN,視覚化機能等を活用し開発．
クライアントと開発の進捗状況の報告，方向性の検討等も行った．

開発は1人で行った．

#### チーム構成

| 役割 | 人数|
| --- | -- |
| マネージャ | 1 |
| エンジニア | 1 |

#### 結果

最終的にpythonのCLIプログラムとして，まとめて納品．
クライアントに満足してもらう結果が得られた．

#### 参考資料

| title   | url  |
| --- | --- |
|3次元レジストレーションの基礎とOpen3Dを用いた3次元点群処理 | https://www.slideshare.net/ttamaki/3open3d3|
| Open3D Doc| 　doc|
| 物体認識のための3次元特徴量とその周辺 |  http://isl.sist.chukyo-u.ac.jp/Archives/Nagoya-CV-PRML-2015March-Hashimoto.pdf|

</details>

### 2021年3月 ~ 4月

[案件]Visual SLAMによる深度画像からの3次元形状復元

#### 技術スタック

* python
* Open3D
* Intel RealSense
* D435,D415,T265

<details>
  <summary>詳細</summary>

#### 概要

RealSenseを用いたRGBD動画像+トラッキングデータからローカルデバイスでの物体形状の3D復元.

#### 具体的な内容

ノートPCに取り付けられたデプスセンサ(D415,D435)とトラッキングセンサ(T265)を用いて
RGBDとPoseを取得.

センサデータをOpen3DのReconstruction Systemを用いて3Dメッシュを生成．

スキャンデータから生成したメッシュと元のCADデータを位置合わせして比較する．

一連の作業をアプリケーションとして動作するよう作成．

#### チーム構成

| 役割 | 人数|
| --- | -- |
| マネージャ | 1 |
| エンジニア | 2 |

#### 結論

スキャン対象の物体の反射率や表面のテクスチャ，形状等によって生成データの
精度が全くことなるため，できるだけテストケースの物体で正常にスキャンできるようパラメータを調整.
納品．


</details>

### 2021年4月 ~ 7月

オプティカルフローを用いた工場監視アプリの作成

[案件]

#### 技術スタック

* python
* kivy
* opencv
* pytorch
* pyinstaller

<details>
  <summary>詳細</summary>

#### 概要

工場の誤動作検出アプリケーションの作成.

#### 具体的な内容

工場内の作業レーンが誤動作でストップする問題があり，問題を検出するアプリケーションを作成．
画像ベースの異常検出等のアルゴリズム等を検討．
最終的にオプティカルフローによる移動検出による停止検出でアプリケーションを作成．
アプリケーションを作成するにあたって，pythonでGUIアプリを作成可能なkivyを採用．

アプリ内でIPカメラ設定機能，検出機能，検出結果を出力等の監視アプリとしての一通りの機能を作成．
検出箇所のマスク機能，クロップ機能なども開発．
opencvでcudaの機能を使うため，cudaをwindowsでカスタムでビルド.
アプリケーションとして納品する際にはpyinstallerを用いてビルド，exe形式で納品．

同案件に参加した新入社員に対しても指導を行う．

開発のメインを担当.

#### チーム構成

| 役割 | 人数|
| --- | -- |
| マネージャ | 1 |
| エンジニア | 2 |

#### 結論

GUIアプリケーションとして納品．
クライアントに満足してもらえる結果が得られた．
アプリケーションとして必要なGUIの構造，os周辺，デバイス，動画コーデックなど総合的なスキルが必要となり，本案件で
かなり広範囲の経験と知見が得られた．
このアプリは次に紹介する自社開発の原型ともなるアプリケーションになった．
</details>

### 2021年8月 ~ 現在

[自社開発]  学習可能な行動分類アプリの開発

#### 技術スタック

* python
* kivy
* opencv
* open3d
* pytorch
* win32api
* C++
* TensorRT
* onnx
* jenkins
* Cython
* zmq

<details>
  <summary>詳細</summary>

#### 概要

ユーザ側でローカルに行動分類のアノテーション，学習，推論が可能なオールインワンアプリケーションの開発.

#### 具体的な内容

骨格推定を利用した行動分類アプリケーションの開発を目的として，
解決タスクの調査，アルゴリズムの調査，検討，アプリケーション設計，実装，GUI作成，ビルドなど

アプリケーションの作成にあたって必要となる作業を最初から終わりまですべてにメインで関わりました．

##### 2021/8 ~ 10

行動分類アルゴリズムの調査，動作検討

#### 2021/11

データ構造，変換機能，学習機能設計，実装

#### 2022/12 ~1

アプリケーションのドラフトをkivyで作成．アプリケーション構成の設計，実装

案件で実際に利用，フィードバックをもらいなら実装を進めていく

#### 2022/2 ~ 3

デザイナーにGUIのデザインを調整してもらう．提供された画面に従って，GUIを修正．

#### 2022/4 ~ 5

アプリの動作の問題や機能の改善，マニュアルの作成等4~5人で修正を行う．
jenkinsによるアプリケーションの自動ビルド機能の導入，スクリプトによりビルド処理の書き出し，
giteaを用いたissueベースでの機能改善等.

#### 2022/6 ~ 現在

2022年5月製品版公開,発売.
現在も機能追加，バグ修正等をメインで継続.
さらなる作業解析のアルゴリズム等の調査も継続中.

#### チーム構成

時期によって変動あり.
| 役割 | 人数|
| --- | -- |
| マネージャ | 1 |
| エンジニア | 2~ 4|
| 広報 | 2 |
| デザイナ | 2 |
| ローカライズ | 1 |

#### 結論

アプリケーションを製品としてパブリッシュ,本格的な複数人でのチーム開発を行う．

問題の切り出しや再現方法，説明の仕方等，他人への情報の伝え方の難しさ，考え方の違い等を実感．

チームとしていかに効率よく開発を行うための方法などを考える機会が得られた．

ただ，その機会を生かせる立場ではないため，最近思うところがあります．

</details>

## ポッドキャスト

その週の気になった記事などを紹介.

議論の練習としても行っています．

[ウェブサイト](https://anchor.fm/yoshi-kyusu)

[matt](https://twitter.com/matt76t)さんと一緒に大体週1で15分程度でやってます.

## 使用機材

* [内田洋行 パルスチェア](https://office.uchida.co.jp/products/pulse/)
* [ProgressTouch RETRO(日本語配列)　赤](https://archisite.co.jp/products/archiss/progres-touch/retro-jp/)
* [BAROCCO MD770](https://archisite.co.jp/products/mistel/barocco-md770/)
