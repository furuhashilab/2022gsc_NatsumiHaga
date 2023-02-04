# 2022gsc_NatsumiHaga

2022年度古橋卒論用レポジトリ

# PokemonGo GOスナップショットにおけるAR空間の機能拡大の実践と提案

青山学院大学 地球社会共生学部 地球社会共生学科 4年A組153番

学籍番号：1A119128　

氏名：葉賀 なつみ

指導教員：古橋 大地 教授

©Furuhashi Laboratory/Natsumi Haga, CC BY 4.0

## Abstract
本研究では、PokemonGoのGOスナップショットにおけるVR空間のマテリアル拡充と自由性、遊びを向上するために、PLATEAU LOD2建物データを応用した「キャラクターが特定の建物に触れると建物が(一時的に)キャラクターを連想させるカラーに変わる」機能の実践と提案を行う。

## Introduction 
『PokemonGo』は『Ingress』などで有名なナイアンティックとポケモンがタッグを組んで開発されたゲームアプリで、位置情報を活用することにより、現実世界そのものを舞台としてプレイする。北米などで2016年7月6日から配信が開始され、2016年（平成28年）7月22日からは日本でもスマートフォン用アプリ『ポケモンGO』がサービスを開始した。ポケモンを捕まえて育てたり、他のプレイヤーとバトルしたり、様々な遊び方ができる。GOスナップショットは同ゲームで、現実の風景と合わせて、お気に入りのポケモンのAR写真を撮ることができる機能である。現在GOスナップショットでは、捕まえたポケモンや相棒とふれあっている様子が撮影できる。

　　本研究では、PokemonGoのGOスナップショットにおけるVR空間のマテリアル拡充と自由性、遊びを向上するために、PLATEAU LOD2建物データを応用した「キャラクターが特定の建物に触れると建物が(一時的に)キャラクターを連想させるカラーに変わる」機能の実践と提案を行う。建物データのデザインはBlender、Adobe Illustratorを用いる。
  
## Method
制作過程と方法を「材料の準備（要素や素材）」と「組立（材料からデザインし建物データに落とし込む方法と手順）」の大きく２つにわける。

1. 「材料の準備（要素や素材）」
![IMG_1549](https://user-images.githubusercontent.com/67300697/216748278-a77bafea-7517-4be1-a986-34d19c72783d.jpg)

	1-1. 対象とする建物データの選考基準:その地域でランドマークとなる有名な建物 
  今回は渋谷駅周辺の[渋谷PARCO](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwit3OrAgvv8AhVysVYBHWygAPIQFnoECAoQAQ&url=https%3A%2F%2Fshibuya.parco.jp%2F&usg=AOvVaw0tJvFl_DX0SQXDJ2dw79_E)をランドマークとする。
  
	1-2. データの種類
		この機能はキャラクターがAR空間内で実際に建物に触れることを起点とするためPLATEAU LOD2建物データを用いる。
    
	1-3. Blenderに選出した建物データをインポート
  
  ・[G空間情報センター](https://front.geospatial.jp)よりPlateau CityGML LOD2建物データをFBX形式でダウンロード
  
  <img width="1440" alt="スクリーンショット 2023-01-10 22 28 05" src="https://user-images.githubusercontent.com/67300697/216748157-b46b9674-635c-4532-8daf-00680b950ef3.png">

2. 「組立（材料からデザインし建物データに落とし込む方法と手順）」

	2-1. ペイントするキャラクターを決定
		プレイヤーのパートナーキャラクター(今回は試験的にピカチュウ)

	2-2. キャラクターの容姿(画像)から適宜1~3色のカラーコードを抽出
		[Adobe Color](https://color.adobe.com/ja/create/image)でカラーコードを抽出
    
     <img width="1440" alt="スクリーンショット 2023-01-11 10 42 48" src="https://user-images.githubusercontent.com/67300697/216748163-3263188f-f723-4105-ae27-58b1f5e70e81.png">

	2-3. 建物データを抽出したカラーにカスタム
  
  ・BlenderのTexture Paintを使ってモデルに色を重ねていく
  
  <img width="1440" alt="スクリーンショット 2023-01-11 0 10 12" src="https://user-images.githubusercontent.com/67300697/216748193-22f8007a-9b95-4d47-b961-37be51d673f1.png">
  
  <img width="1440" alt="スクリーンショット 2023-01-11 0 14 33" src="https://user-images.githubusercontent.com/67300697/216748205-4142d781-2f5f-452a-a932-2a2c518418bf.png">
  
  <img width="1440" alt="スクリーンショット 2023-02-04 4 22 30" src="https://user-images.githubusercontent.com/67300697/216748126-9141f558-c57e-40f5-89a9-7afd7f72ee9c.png">
  
  
3. Blender、Adobe Illustratorを利用し、PokemonGoの世界に制作物をコラージュ

## Results
渋谷区渋谷駅一部周辺を対象にPLATEAU LOD2建物データをBlenderにインポートし、特に渋谷PARCOをランドマークとして選択・キャラクターデザインのカスタムを行なった。また、デザインした建物データを実際のGOスナップのようにコラージュした画像を作成した。他の建物と視覚的に区別しやすく、キャラクターとの統一性もみられ、特別感がある。

## Discussion 
本研究では、GML LOD2の建物データを応用して、街中で特定の建物データにのみ着色して表現した。実際に制作して発見した課題として、多数の個性を表現する難しさがある。配色は１〜３色で行うためカラーが似ているポケモンが複数ある場合、違いがあまりなく見分けがつかない点がある。建物の側面や屋根を利用して違いをつけることもできるが、建物ごとに形に特徴があり一つひとつに合わせてカスタマイズするのはかなりの手間がかかる。代わりに、変わるカラーをポケモンのカラーではなく、ポケモンのタイプに合わせて変化するようにすることで少ない数で被りもなく、すべてのポケモンに対応させることができる。ポケモンのタイプは全18種類に分かれ、それぞれカラーとマークがある。グラデーションを入れたり、タイプに合わせた要素のパターンを使ってもより華やかになり、識別性も上がるだろう。また、対象のランドマークとなる建物の選定に関しても、側面のサイズや建物数がデザインにおける重要なポイントであり、これらを含めた基準となる指標を立てることが表現の幅を広げることにつながると考える。

<img width="682" alt="スクリーンショット 2023-02-02 17 32 15" src="https://user-images.githubusercontent.com/67300697/216748256-223f101a-d148-44ec-aee0-5b4a54fa0afe.png">

![waterTear](https://user-images.githubusercontent.com/67300697/216748073-87fad3f8-b2ad-43fc-9768-34097bd9d707.PNG)

<img width="1440" alt="スクリーンショット 2023-02-04 5 58 02" src="https://user-images.githubusercontent.com/67300697/216747822-255c5ff0-b01a-4159-9076-f08c1ca44765.png">

## Conclusion

## Acknowledgements
本研究を進めるにあたり青山学院大学地球社会共生学部教授の古橋大地氏をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## 先行研究

・[PLATEAU](https://www.mlit.go.jp/plateau/new-service/4-010/)

・[OSMへのインポート](https://qiita.com/nyampire/items/1c10afdd36750c87154d)

・[PLATEAUデータのマインクラフト化](https://qiita.com/nyampire/items/0f46cc38109acd0c70c8)

## 参考文献・参考資料リスト

https://docs.google.com/spreadsheets/d/1sQpJR7FnUbqRURUpNo9xf2Z2i2gX-a8ZcWz6Vt3131k/edit#gid=0

## プロジェクト管理

https://github.com/orgs/furuhashilab/projects/21/views/1

## 中間発表(2022.11.8)

・Medium

https://medium.com/furuhashilab/卒論中間発表-26c0ccf2a3c5

・Google Slides

https://docs.google.com/presentation/d/1WeXSfyOX_zXab1UgCIGrFo4yTMEZ6LF-u-LvFYfQ-CM/edit#slide=id.p

## 最終発表(2023.2.4)

・Medium

・Google Slide

https://docs.google.com/presentation/d/1yLyhu8fEkhYLIKPF5sv8_UNL_Dfb7j-U6LCm7OXoPQA/edit?usp=sharing


