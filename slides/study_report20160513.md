class: center middle
# 進捗報告20160506
# 小町研究室 M2 北川善彬
---
# 前回のTodo
## 来週まで
* 1-4 gram のembedding 実験
* EMNLPの論文書き
* MS の CORE レビューミーティング（共同研究）の発表のポスター作り

## 次回以降 or できたら
* pre-training アンサンブル？
* コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* CNN、bi-directionalな手法

---
# 進捗状況
## 研究の進捗
* [◯]1-4 gram のembedding 実験
* [◯ → △]辞書素性の利用
* [◯]MS の CORE レビューミーティング（共同研究）の発表のポスター作り
* [✖︎]EMNLPの論文書き

## 次回以降 or できたら
* [✖︎]コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* [✖︎]pre-training アンサンブル
* [✖︎]CNN、bi-directionalな手法

## その他
* MSのインターン(5/31 - 7/31 )
* NTT研究所　プレゼンテーション 6/2
---
# trigram embedding を追加でさらに向上

* ほぼ KyTea と同程度
* LSTM (文字 + 文字種) 97.25 → LSTM (1-3gram(文字 + 文字種)) 98.37 (KyTea 98.34) on BCCWJ
* LSTM (文字 + 文字種) 89.27 → LSTM (1-3gram(文字 + 文字種)) 92.33 (KyTea 92.38) on Twitter
* 結果を整理できていないので直接見せます

---
# 辞書を入れたら上がると思ったが
* 結果: 上がらず
* 初めの入れ方はKyTeaの素性の作り方にならい embedding を作っていた
* ダメなので[Tsuboi ACL2014]を思い出して試す
* あんまり変わった感じがない
* 単語長が 1 のものを除く
* あんまり変わった感じが

---
# EMNLPに出せそうな場合に備えて
* 論文を少し書く 1page + 目次
* cloudTex 使わず普通に書く
* ほとんど進んでいない

---
# Microsoft インターン
* 5/31 - 7/31 の2か月間に決定。週3
* バックグラウンドスクリーニングや入社手続き中

---
# 次回までのTodo
* 月曜日に EMNLP 初稿?
* Pre-training に seq2seq autoencoder
* 辞書の使い方どうするか？
