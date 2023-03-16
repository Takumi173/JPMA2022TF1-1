# 有害事象判定モデル
日本製薬工業協会 データサイエンス部会 2022年度のタスクフォースで作成したプログラムです。詳細は報告書（公開後にリンクを掲載予定）をご参照ください。


## 実行環境
[Colaboratory](https://colab.research.google.com/?hl=ja)のみで完結します。必要な事前準備はGoogleアカウントの取得のみです。
各ファイルを開いた後に<img src ="https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667">のアイコンをクリックすることでColaboratoryで開けます。

なお、プログラム間のデータの受け渡しにはGoogle Driveを使用します。

## 形態素解析器と辞書
形態素解析器は[Mecab](https://taku910.github.io/mecab/)を使用し、システム辞書に[mecab-ipadic-NEologd](https://github.com/neologd/mecab-ipadic-neologd)を、
ユーザ辞書に[万病辞書](https://sociocom.naist.jp/manbyou-dic/)を使用させていただきました。


## 事前学習モデル
東北大学で作成された以下の2つのモデルを使用させていただきました。
 - [Wikipedia Entity Vectors](https://github.com/singletongue/WikiEntVec)
 - [Pretrained Japanese BERT models](https://github.com/cl-tohoku/bert-japanese)

## ラベル付きデータの用意
[ラベル付きデータ](https://github.com/Takumi173/JPMA2022TF1-1/releases/download/20221226/Training.txt)は[厚生科学審議会 (予防接種・ワクチン分科会 副反応検討部会)](https://www.mhlw.go.jp/stf/shingi/shingi-kousei_284075.html)で公開されている症例経過に記載された文章を一部改変し、タスクフォースで用意した文章と組み合わせて用意しました。

## ライセンス
学習済みモデルは[Creative Commons Attribution-ShareAlike 3.0](https://creativecommons.org/licenses/by-sa/3.0/)の下に配布されます。

このリポジトリにあるコードは、MITライセンスの下に配布されます。
