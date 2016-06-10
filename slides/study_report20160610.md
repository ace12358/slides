class: center middle
# 進捗報告20160610
# 小町研究室 M2 北川善彬

---
class: center middle 
# 進捗状況

* [×] seq2seq の pretraining
* [○] 辞書について 外部辞書利用 singleton の削除
* [△] ハイパーパラメータのセッティング確認と実験
* [×] 論文執筆

---
class: center middle 
# singleton 削除でうまくいった？
* 実験したら F値 98.67 とかになり辞書素性がうまく効いていい感じ？
* → と思ったらtest の辞書が入ってた…
* でも、未知語がない場合の結果が分かった。辞書素性がうまく動いてることが分かった

---
class: center middle 
# KyTea  との違い分析 (定性的)
* 名詞の複合語の切れ目がうまく切れる（特にカタカナ）
* 漢字の接尾辞接頭辞などをうまく判別できる　（下　世話、不　遡及、異　文化 間 交流）
* 文字種混同していても切れないとこは切れない（ズ太い）
* nn の方がひらがなはまとまりで捉えやすい（くだっさい、って、すくない）

---
class: center middle 
# Hyper parameter search
* 表にしてまとめた
* まだ結果を載せてないところ、実験してないところあり
* Hyper parameter を変えていろいろ実験

---
class: center middle 
#Todo
* [4] bi-directional
* [3] seq2seq の pretraining
* [2] ハイパーパラメータのセッティング確認と実験
* [1] 論文執筆

