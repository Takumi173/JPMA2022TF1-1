# 有害事象判定モデル
日本製薬工業協会 データサイエンス部会 2022年度のタスクフォースで作成したプログラムです。詳細は[データマネジメントにおけるArtificial Intelligenceの活用 ～ これから始めるAI ～](https://www.jpma.or.jp/information/evaluation/results/allotment/DS_202305_2022TF1_1_AI_DM.html)をご参照ください。


## 実行環境
[Colaboratory](https://colab.research.google.com/?hl=ja)のみで完結します。必要な事前準備はGoogleアカウントの取得のみです。
各ファイルを開いた後に<img src ="https://github.com/Takumi173/JPMA2022TF1-1/assets/109738801/522a6fd7-b171-4ad3-8f56-e73a718a6542">のアイコンをクリックすることでColaboratoryで開けます。

なお、プログラム間のデータの受け渡しにはGoogle Driveを使用します。

## 形態素解析器と辞書
形態素解析器は[Mecab](https://taku910.github.io/mecab/)を使用し、システム辞書に[mecab-ipadic-NEologd](https://github.com/neologd/mecab-ipadic-neologd)を、
ユーザ辞書に[万病辞書](https://sociocom.naist.jp/manbyou-dic/)を使用させていただきました。


## 事前学習モデル
東北大学で作成された以下の2つのモデルを使用させていただきました。
 - [Wikipedia Entity Vectors](https://github.com/singletongue/WikiEntVec)
 - [Pretrained Japanese BERT models](https://github.com/cl-tohoku/bert-japanese)

## データの用意
[モデルの構築及び検証に使用したデータ](https://github.com/Takumi173/JPMA2022TF1-1/releases/download/20221226/Training.txt)は[厚生科学審議会 (予防接種・ワクチン分科会 副反応検討部会)](https://www.mhlw.go.jp/stf/shingi/shingi-kousei_284075.html)で公開されている症例経過に記載された文章を一部改変し、タスクフォースで用意した文章と組み合わせて用意しました。

## ライセンス
東北大学で作成された事前学習モデルのライセンスを継承し、学習済みモデルは[Creative Commons Attribution-ShareAlike 3.0](https://creativecommons.org/licenses/by-sa/3.0/)の下に配布されます。

このリポジトリにあるコードは、MITライセンスの下に配布されます。
