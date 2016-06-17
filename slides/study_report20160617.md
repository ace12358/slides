class: center middle
# 進捗報告20160617
# 小町研究室 M2 北川善彬

---
# 進捗状況
class: center middle 
#Todo
* [×] bi-directional
* [×] seq2seq の pretraining
* [×] ハイパーパラメータのセッティング確認と実験
* [×] BCCWJのジャンル分けによるエラー分析
* [△] 論文執筆
* TokyoCL

---
class: center middle
## 論文執筆
* あまり進んでません
* 貢献を明確にしたい（BCCWJのジャンル分けした際の分析に依存しそう）
    * ニューラル単語分割の日本語適用と日本語単語分割特有の問題への対処
    * ニューラルと既存手法の違いを分析 or Web文書の解析に貢献するかを評価

---
class: center middle 
# TokyoCL報告（内容3つ）
* 自然言語処理でメタファーをどう扱うか —いくつかのモデルとデータの紹介—
* モンテカルロ木探索を用いた統語情報を考慮した文生成
* CRFとNPYLMの統合による半教師あり形態素解析 (完全版)

---
class: center middle 
# 簡単にまとめ
* CRFと教師なし形態素解析を組み合わせた、 半教師あり形態素解析
    * JESS-CM法の枠組で EM 的な感じで「教え合う」
    * Semi-Markov(単語)<->Markov(文字) の情報相互変換

* 半教師ありにより、人での基準を守りつつ、未知語を自動的に検出
* Future Work 品詞付与をどうするか？理論的には内海さんのACL105の枠組みでできるけど

---
class: center middle 
#Todo
* [3] ハイパーパラメータのセッティング確認と実験
* [2] BCCWJ でジャンル分けして評価してみる
* [1] 論文執筆
