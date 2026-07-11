# 派生開発と XDDP

勉強会発表資料 / 発表枠：25分

---

## 構成

### ① 冒頭：成果物の提示（2分）

「突然ですが、このテーマの追究の過程で得られた、**現時点で**私が実務への適用を**考えている**成果物はこちらです」

- 要求仕様書（派生開発用）テンプレート
  - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.delta.template.tsv

「なぜこれを作ったのか、25分で話します」

---

### ② 派生開発とは？（3分）

定義と、新規開発との一言比較

---

### ③ なぜこのテーマか（10分）

- チームの当面の仕事はシステムの追加開発と予想される
- 世の開発ノウハウは新規開発前提のものが多い
  - システム開発の世界標準規格まで遡ってみた
    - 特に要求仕様化の段階に関与するのは BABOK と ISO/IEC/IEEE 29148（国内対応物：JIS X 0166）
    - 変更管理などの項目はあるものの、派生開発ノウハウの記述は薄い（本当か？）
  - **「新規開発用の要求仕様書テンプレートはこうなります」**
    - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.template.tsv
  - **「派生開発に適用するには何が足りないと思いますか？」** ← 聴衆への問いかけ

---

### ④ XDDP とは？（6分）

③の問いへの答えとして自然に接続

- 参考文献：清水吉男 著
  - 『「派生開発」を成功させるプロセス改善の技術と極意』2007年
  - 『【改訂第２版】［入門＋実践］要求を仕様化する技術・表現する技術』2010年

---

### ⑤ 収束：派生開発用テンプレートへ（3分）

①で見せたテンプレートに戻る

- 「③で挙がった "足りないもの" がここに入っています」
- **「まだやってる途中です。フィードバックいただければ幸いです」**（等身大）

---

### ⑥ Q&A（1分）

---

## 参照

| 資料 | リンク |
|---|---|
| 要求仕様書テンプレート（新規開発用） | [requirements.template.tsv](https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.template.tsv) |
| 要求仕様書テンプレート（派生開発用） | [requirements.delta.template.tsv](https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.delta.template.tsv) |
| 『「派生開発」を成功させるプロセス改善の技術と極意』清水吉男、2007 | https://gihyo.jp/book/2007/978-4-7741-3249-5 |
| 『【改訂第２版】要求を仕様化する技術・表現する技術』清水吉男、2010 | https://gihyo.jp/book/2010/978-4-7741-4257-9 |
| BABOK | https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/ |
| ISO/IEC/IEEE 29148 | https://www.iso.org/standard/72089.html |
| JIS X 0166 | https://webdesk.jsa.or.jp/books/W11M0090/?bunsyo_id=JIS%20X%200166:2021 |
