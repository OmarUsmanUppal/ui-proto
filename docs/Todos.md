# Todos

1. 発注範囲、前提等
2. 画面/UI一覧
3. 画面遷移図
4. 画面詳細仕様書

---

# 発注範囲、前提等

1. PCブラウザでの閲覧用のUIのみを構築する
  * SP用のUI，レスポンシブの考慮は現時点では必要ない
  * SPのブラウザで閲覧する際は、PC用のUIがそのまま表示される形でよい
2. 全体を通して、クリックアクションに対するUIの動作は、画面のリロードを発生させず、JSによるUIの変化とデータの変化により実現する
  *  これを第一義としたいため、それ以外の詳細については交渉により作業量をへらすことも可能

----

# 最終ドキュメントの章構成

1. 発注範囲、前提等
2. 画面構成
  * 総画面パターン数
    * 一覧、詳細 w/ 画面パターンID
    * メニュー部品のパターンに関して
  * メニュー部品はIntroductionおよびカート以降の画面以外、表示しっぱなしにし、クリックアクションによってリロードされることが
4. 画面遷移図
4. 画面/UI一覧
  * 画面構成で降った画面パターンIDとのマッピング
5. 画面詳細


---






---

#  画面/UI一覧

1. Introduction
2. Top
  1. index
    1. NEW ARRIVAL
    2. MAISON EUREKA
      1. Top
      2. BOTTOM
      3. JACKET & COAT
      4. SHOES
    3. FAT LAVA
      1. TBD
    4. STUDIO KERAMIK
      1. TBD
    5. DESIGNERS VINTAGE
      1. TBD
    6. AFRICAN ANTIQUE
      1. TBD
    7. OTHER
      1. TBD
  2. Instagram Link
  3. Facebook  Link
  4. Email Link
3. Category
  * TBD: UIパターンは一つでOKの想定
4. Detail
  * TBD: UIパターンは一つでOKの想定
5. カート画面
  * ここはビルトインでもOK。一番はやく作れる方法で

-----

# 画面遷移図

* 1. Introduction -> 2. Top w/ 2-1. Index -> 以下の階層はIndex内でUIが変化。最下層をクリックすると次へ -> 3. Category 商品をクリックしたら次へ -> 4. Detail 購入アクションが一通り可能

-----

# 画面詳細仕様書

* ここは各ページ.mdを作るか

## 1. Introduction

* "Hallo ... " 的な文言を表示。クリックすると次へ
* このとき画面リロードではなく
