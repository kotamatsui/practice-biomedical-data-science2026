# 医療データ科学実習（Practice of Biomedical Data Science）

| 講師  | 松井茂之，松井孝太，江本遼，西田一貴 (医療統計学)|
| --- | -------- |
| 日程  | 火曜日3，4限|

## 概要 
この演習では，医療データ科学（コア）の講義で学んだ医療データ科学の考え方を実際に実践することでその理解の定着を図ることを目的とします．フリーのデータ解析のソフトウエアとして今日幅広く使用されている「R」を用いた実習を中心に行います．後半は様々な実データを解析し，結果を整理してプレゼンテーションするグループ実習を行います．本実習の受講にあたり，各自のノートパソコン（Windows，Mac）を持参してください．

## 到達目標
- 医療データ科学の考え方，基本的なデータ解析法についての理解を深める．
- データ解析ソフトを用いて，データ読み込みからデータ解析までを適切に行い，解析結果を適切に解釈できるようになる．

## 成績評価
- 数回の個人レポートとグループによるプレゼンテーションと質疑応答を評価します．
- 配分はレポート70％，グループ実習でのプレゼンテーションと質疑応答30%相当とします．

## 準備
- [R](https://www.r-project.org)および[RStudio](https://posit.co/download/rstudio-desktop/)を各自のパソコンにインストールします（インストールについては初回の講義時に説明します）．
  - Rは統計を含むデータ解析に特化したオープンソースのプログラミング言語であり，医学・生物学研究をはじめ多くの領域で広く用いられています．
  - RStudioはR用の主要な統合開発環境 (Integrated Development Environment, IDE) です．多くの人がRStudioを使ってRのコーディング，実験管理を行います．
- 講義中のRコードの共有には[Google Colab](https://colab.research.google.com)を利用します．利用にはGoogleアカウントが必要となりますので，持っていない場合は作成をしてください（アカウントの作成は無料でできます）．

## 講義スケジュールとコンテンツ
凡例：📖 スライド資料，💻 Google Colab，💡 slido (質疑応答フォーラム)
### 第1回(4/8): データ解析ソフト「R」事始め, インストール, 環境設定
- Rのインストール方法 [📖](Session1/r-install.pdf)
- RStudioのインストール方法 [📖](Session1/rstudio-install.pdf)
- R言語で何ができるか？[📖](Session1/R_demo_logistic.pdf)
- R言語事始め [📖](Session1/R言語事始め.pdf)
  - Rの変数とデータ型 [💻](https://colab.research.google.com/drive/1xxZ20hLT_deXhGRLtRpkht2t9KJ6G4cw?usp=sharing)
  - ベクトル演算 [💻](https://colab.research.google.com/drive/1C_NLAvUe4bMCiv9lQGOqH6wAvTTFd_9P?usp=sharing)
  <!-- - Rによる擬似乱数生成 [💻](https://colab.research.google.com/drive/1A6nBKT40T_vSZuXONgFgAgMF8QVzqG7w?usp=sharing) -->

### 第2回(4/15): データセットの作成　[💡](https://app.sli.do/event/ntA1oiNfNnSgbddJ8sUhiQ)
- R言語事始め（続き）[📖](Session2/250415_pbds_session2.pdf)
  - Rにおけるデータテーブルの作成
  - R上のデータテーブルの外部ファイルへの書き出しと外部データのRへの読み込み
  - Rの組み込み関数
  - 外部パッケージのインストールとインポート
    - Rによる擬似乱数生成 [💻](https://colab.research.google.com/drive/1A6nBKT40T_vSZuXONgFgAgMF8QVzqG7w?usp=sharing)
    - ベクトル演算 [💻](https://colab.research.google.com/drive/1C_NLAvUe4bMCiv9lQGOqH6wAvTTFd_9P?usp=sharing)
    - 乱数生成とプロット [💻](https://colab.research.google.com/drive/1-1cKZQ1egoaITwGHS9bMvLQqipf9-9P3?usp=sharing)
- Microsoft Excelで作られたデータの取り扱い [📖](Session2/R_Excel_Data_ex.pdf)  [データセット](https://www.dropbox.com/scl/fo/bx4rkyx48eo1o209w69nl/ACSn0dwcNiWNhFl9g0LnLnI?rlkey=5iujgakjr7bqeepum3xqar7tk&st=bk8w0bfo&dl=0)
  - Rに正しくデータを読み込むための前処理
    - Excel上でのデータ作成，データテーブルの修正とCSVファイルへの変換
    - よくあるExcelやCSVの問題点と対処法
    - 適切なデータセットとは
  - Rへの読み込みとR上でのデータチェック

250418更新：
  - R言語事始め（続き）スライドp14 Rによる数値計算とベクトル演算の演習問題を正しいものに差し替え
  - R言語事始め（続き）スライドp18 乱数生成とプロットのサンプルコードを追加

### 第3回(4/22): データの集計 [📖](Session3/250422_pbds_session3.pdf) [💡](https://app.sli.do/event/6sQCjSZQvSq31Bvj2Q9aUa)　
- ベース機能を使っての表作成 [📖](Session3/Table_Creation_with_Base_R.pdf) [演習問題（発展）](https://www.dropbox.com/scl/fo/evreyzkmf7rsb51s1khrt/AIIALdV87EixxKG4kh_8QfM?rlkey=0wiqmbuqlhazc282ecmlkvllu&st=yqand3ao&dl=0)
  - 一変数：離散変数の頻度集計，連続変数の頻度集計
  - 二変数：離散変数のクロス集計
  - 要約統計量算出（連続変数の平均，中央値，分散，標準偏差など）
  - 層別の集計，要約統計量の計算　[💻](https://colab.research.google.com/drive/1P71QD40T-BcGgqJ-nTY6SPnucy2r1yJm?usp=sharing)
- 外部パッケージを使ってのデータ集計
  - dplyrとjanitorを使ったデータ操作・集計，クロス集計や頻度表の作成
  - 組み込み関数を用いた集計と外部パッケージを用いた集計の違い

### 第4回(5/13): グラフの作成1 [💡](https://app.sli.do/event/c3tMS5GsSGjpX49jYKgP4Q/live/questions)　
- ベース機能を使ったグラフの作成
  - 一次元の連続変数の経験分布（相対頻度，累積頻度，生存頻度），多群の重ね描き，ボックスプロット [📖](Session4/250513_pbds_session4.pdf)
  - 二次元の連続変数の散布図，多群の重ね描き，時系列 [📖](Session4/Figure_two_variables.pdf) [💻](https://colab.research.google.com/drive/1s3Bbdw9f8833uIpUJkdoJNt0f5UiKyMJ#scrollTo=e901a991)
  - タイトル，軸線，ラベルフォント・サイズ，プロット点の大きさ，凡例などの設定方法
 
250516更新：
- 一次元の連続変数のプロットのスライドに演習問題のサンプルコードと実行例を追加 [📖](Session4/250513_pbds_session4_updated.pdf)
 
### 第5回(5/20): グラフの作成2
- パッケージを使ったグラフの作成
  - 一次元の連続変数の経験分布（相対頻度，累積頻度，生存頻度），多群の重ね描き，ボックスプロット [📖](Session5/250520_pbds_session5.pdf)
  - 二次元の連続変数の散布図，多群の重ね描き，時系列 [📖](Session5/ggplot_two_variables.pdf)
  - タイトル，軸線，ラベルフォント・サイズ，プロット点の大きさ，凡例などの設定方法

### 第6回(5/27): 記述統計
- 一次元の離散変数，連続変数に対する  [📖](Session6/250527_pbds_session6.pdf)
  - 経験分布，要約統計量（平均，分散，標準偏差，パーセンタイル）
  - 歪んだ分布の問題と対応
  - 外れ値の影響
- 二次元の離散変数，連続変数に対する [📖](Session6/Descriptive_Statistics_Two_Variables.pdf)
  - 経験分布，要約統計量（平均，分散，標準偏差，パーセンタイル）
  - 歪んだ分布の問題と対応
  - 外れ値の影響
  - qq-plot
  - 相関計数

250603更新：
  - 前半のスライドに前回のslidoの回答を追加 [📖](Session6/250527_pbds_session6_update.pdf)
    
### 第7回(6/3): シミュレーション, 統計的推測の基本概念　前半 [📖](Session7/250603_pbds_session7_ver2.pdf) 後半 [📖](Session7/CLT_CI.pdf)
- 興味あるパラメータの推定
- 推定量の分布，分散，標準誤差，信頼区間，被覆確率（一様分布，正規分布，指数分布，ポアソン分布，ベルヌーイ分布）
- 多数の独立なシミュレーションの実行
- リスク差，リスク比，オッズ比の信頼区間
- 二群の平均の差の信頼区間

250603更新：
  - 前半のスライドの数式の崩れの修正，p66-67のサンプルコードのミスを修正

### 第8回(6/10): 統計的仮説検定の基本概念とサンプルサイズ設計
- 仮説検定の基本概念 [📖](Session8/250610_pbds_session8.pdf)， 検出力曲線のサンプルコード：[💻](Session8/power_simulation_sample_size.txt)
  - 仮説検定のロジック，片側/両側検定
  - 帰無仮説/対立仮説，有意水準，p値
  - 第一種の過誤と第二種の過誤
- サンプルサイズ設計 [📖](Session8/sample_size.pdf)

250613更新：
  - 前半の最後の演習問題のサンプルコードを追加（真の反応率を変えたときの検出力曲線の描画）[💻](Session8/power_simulation_true_response_rate.txt)

  
### 第9回(6/17): グループ実習1: データ選択・収集, 解析計画書　[💡](https://app.sli.do/event/gPjJ3NeA5yTPjNGRw7YDff)
- グループワーク実施要項 [📖](Session9/group_projects.pdf)
- 班分けはPandAにアップロードしてあるので各自確認の上班ごとの位置に着席する

### 第10回(6/24): グループ実習2: データ解析
- グループワーク実施要項 (更新) [📖](Session10/group_projects_ver2.pdf)
- 班分けはPandAにアップロードしてあるので各自確認の上班ごとの位置に着席する
  
### 第11回(7/1): グループ実習3: データ解析
### 第12回(7/8): コーディングテスト / グループ実習4: 報告資料の作成
  **コーディングテスト（3限目，13:15-14:45）**　試験問題 [📖](https://www.dropbox.com/scl/fi/tsqicav591psb58sumbvo/250708_-_.pdf?rlkey=fcrx5tk87jwcmiw4c6auvtw8r&st=0iwy9024&dl=0)
  - 試験問題はPandAにもアップロードします
  - 試験時間：60分（Exam duration: 60 minutes）
  - 資料の持ち込みおよびweb検索は可．生成AIの能動的な使用と周囲との相談は不可（You can bring reference materials and perform web searches. Active use of generative AI and consultation with others are not allowed）
  - 自身のR，RStudio，またはGoogle Colab環境で実施すること（You must complete the tasks using your own R, RStudio, or Google Colab environment）
  - テキストエディタは自由（You can use any text editor of your choice）
  - 各問題の出力は，指定された方法で問題ごとの提出フォームからアップロードしてください（Upload the output for each question using the designated submission form for that specific question）

　 **グループワーク(4限目,15:00-16:30)**
  - データ解析の内容をfix
    - 基本的にはこの時間までの内容をもとに最終プレゼンを作成する
    - 時間外に追加の解析をしたりプレゼン資料を作成することは認める
    
### 第13回(7/15): 診断・予後解析研究におけるデータ解析，グループワーク実習5
  **診断・予後解析研究におけるデータ解析の実習(30分程度)**  [📖](Session13/ROC.pdf)

  **グループワーク(150分程度)**
  - 発表資料の作成
  - 余裕がある班は追加の解析などを実施しても良い
  
### 第14回(7/22): グループ実習6: プレゼンテーション
プレゼン資料投稿フォーム（google form）[📮](https://docs.google.com/forms/d/e/1FAIpQLSd68HeTWuuv70LQpG3uI1x-WuazwYOM5tiMUueKjFdTf-AgXw/viewform?usp=dialog)

<!--
## 講義資料
- [スライド資料 (PDF)](slides/lecture1.pdf)
- [Python コード](notebooks/lecture1.ipynb)
-->

---
© 2025 Kota Matsui
