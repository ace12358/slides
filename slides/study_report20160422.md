class: center middle
# 進捗報告20160422   
# 小町研究室 M2 北川善彬
---
# 前回のTodo
* コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* bi-gram tri-gram embedding の追加
* 辞書素性の利用
* pre-training アンサンブル？
* CNN、bi-directionalな手法


---
# 進捗状況
## 研究の進捗
* [△]コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* [◯]bi-gram tri-gram embedding の追加
* [△]辞書素性の利用
* [x]pre-training アンサンブル？
* [x]CNN、bi-directionalな手法
## その他
* MSのインターンの面接
* NTT研究所のオープンラボ
* DL-NLP 勉強会に参加
---
# GPUでバッチ処理で並列化
* つまって進まず
## 問題点
* RNNの構造だと入力の長さが文によって違う
* 前の隠れ層が計算し終わらないと次の隠れ層の計算ができない
* → 佐藤くん、宮崎くんに聞いて改善します

---
# bi-gram tri-gram embedding の追加
* 厳密には tri-gram embedding はまだ
* bi-gram embedding の初期化はランダム
* 文字、文字種両方ともに対して実装
* 結果は来週になりそう
---
# Microsoft のインターンのための面接
* 2時間の面接@品川 1人一時間 * 2 
* 技術的な質問は小町研の学生にしても。。と言われほぼ雑談に
* オファー待ちの状況

## 何をやるか
* りんなちゃんに関することなら何でもいいと言われる

## 候補
* 共同研究になっているひらがな単語分割
* りんなの新しい feature を考える
    * 例: ぼっち人狼

---
# 次回までのTodo
## 来週まで
* コードの書き直し（Chianer のverionアップ 1.4 → 1.7、高速化、）
* bi-gram tri-gram embedding の追加
* 辞書素性の利用
--
## 次回以降 or できたら
* pre-training アンサンブル？
* CNN、bi-directionalな手法
* MS の CORE レビューミーティング（共同研究）の発表のポスター作り

