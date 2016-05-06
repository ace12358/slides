class: center middle
# 進捗報告20160506
# 小町研究室 M2 北川善彬
---
# 前回のTodo
* コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* bi-gram tri-gram embedding の追加
* 辞書素性の利用
## 次回以降 or できたら
* pre-training アンサンブル？
* CNN、bi-directionalな手法
* MS の CORE レビューミーティング（共同研究）の発表のポスター作り

---
# 進捗状況
## 研究の進捗
* [✖︎]コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* [◯]bi-gram tri-gram embedding の追加
* [◯]辞書素性の利用

## 次回以降 or できたら
* [✖︎]pre-training アンサンブル
* [✖︎]CNN、bi-directionalな手法
* [✖︎]MS の CORE レビューミーティング（共同研究）の発表のポスター作り

## その他
* MSのインターン(5月下旬 or 6月 〜 )
* NEologd 勉強会@LINE
* B4のテーマ案を作成

---
# bigram embedding を追加
* 精度が大幅に向上
* LSTM (文字 + 文字種) 97.25 → LSTM (1-2gram(文字 + 文字種)) 98.05 (KyTea 98.34) on BCCWJ
* LSTM (文字 + 文字種) 89.27 → LSTM (1-2gram(文字 + 文字種)) 91.07  (KyTea 92.38) on Twitter

* 3-gram 、辞書素性は結果がまだ
* Adagrad の収束がめっちゃ早い

---
# EMNLPに出せそうな場合に備えて
* 論文を少し書く 1page + 目次
* https://cloudlatex.io/home/filetree?locale=ja

---
# Microsoft インターン
* オファーをもらいました
* 5月下旬以降から三か月程度の予定

---
#NEologd Casual Talk @LINE
* NEologdの使いみちの話
    * 検索クエリのサジェストの前処理に利用
    * 正規化をする NEolodn の話 ウェーーーーイ→ウェイ
    * フリマアプリに適用した話 ファー　ローファー　ローリングスファーズ
    * 東北大の人の Wikitification の話 知識を紡ぐための言語資源
* 今後の方針

---
# 次回までのTodo
## 来週まで
* 1-4 gram のembedding 実験
* EMNLPの論文書き
* MS の CORE レビューミーティング（共同研究）の発表のポスター作り

## 次回以降 or できたら
* pre-training アンサンブル？
* コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* CNN、bi-directionalな手法

