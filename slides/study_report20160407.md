# 進捗報告20160129
## 小町研究室 M1 北川善彬

---
##前回のTo do
* NLP 第4稿 〆17:00
* 文字種情報を残り2通りの手法に追加


---
##進捗状況
* NLP 投稿完了
* 論文紹介
    * English POS tag state-of-the-artのやつ    
* chainer の batch を使った高速化
* 今後の方針の整理

---
##今後の大雑把な方針の整理
* 学習の高速化
* bi-gram trai-gram embdedding, pre-training の利用（最低限やらないといけないもの）
* transition の利用
* 辞書の利用
* ニューラル日本語形態素解析器のオープンソース化（いいものができたら）

---
##高速化について
![right,200%](https://qiita-image-store.s3.amazonaws.com/0/76221/2717f35b-6aa3-d0e0-a561-9475dcd4cab3.png "Kobito.wcKJJe.png")

* batch 次元を使い行列演算にして高速化
* 入力をベクトルでなく行列にする
* 早くなったっぽい
* GPUを使うことで真価を発揮すると思われる

---
##論文紹介について
* POS tag で state-of-the-art の論文を読む
* 読んだ理由は今後の POS 付加作業のこととモデルの参考になるのではと徳永さんに勧められたので
* モデルは離散スパースな素性と連続密な素性をうまく組み合わせること

![right, 200%](https://qiita-image-store.s3.amazonaws.com/0/76221/608a3c8a-c423-ba95-8c0a-f2e91df23572.png "Kobito.xTXh62.png")

---
##transition の利用
* [Chen+ EMNLP2015]のモデルは結局、B → Iなどのラベル遷移の確率分布をだしているだけ
* なら、実際のコーパスを先になめて、P(B|I)などの確率分布を出しておいても良さそう？
* さらにP(B|あ,I)　みたいなのも計算できればよりリッチなのでは？
* 組み合わせ方は[Tsuboi EMNLP2014]も役に立つかも？

---
##辞書素性の利用
* 日本語の形態素解析は品詞やその他要素がアノテーションされたリッチなコーパスがあるので使わないと損？
* まずは KyTea の素性に使われているような方式でモデル化を考えるべき
* 判定する文字の左の文字で終わる単語があるかないか、判定する文字から始まる単語が存在するかないか

---


##To do
* bi-gram tri-gram embedding の追加
* pre-training の有効性の評価

--

* label-transition の追加
* 辞書素性の追加
