# 派生開発の上流をどう整備するか

勉強会発表資料 / 発表枠：25分

## 構成

用語に従って進行する。

### 開発種別

- 新規開発
- 派生開発

### 手法：XDDP

派生開発向けの手法。

#### 変更要求仕様書

- 構成要素
  - 要求 ID
    - トレーサビリティの担保に必要
  - 要求
    - 仕様化するまで再帰的に分解する
      - 仕様とは
        - 設計以降のフェーズの入力として適格な具体性があり、各フェーズ担当者間で解釈が一致するような記述である
        - 関係者のレビューを経て確定している
        - 検証可能性があり、仕様からテストを立てることができる
  - 理由
    - 要求の妥当性の判断に必要
- 要求の書き方
  - 範囲を表現する
  - before/after を表現する
  - 仕様から逆に要求を立てる
    - 例：仕様に踏み込んだ要求「監視システムのカメラの首振り角度を大きくしたい」
      - 安直に引き受けると...手戻りの連続
        - 「首振り角度を大きくしたら往復周期も長くなり死角が大きくなった」
        - 「死角をカバーするために首振り速度を上げたらサンプリングが追いつかず映像がコマ送りになった」
      - 最上位の要求を突き止めれば全体を見渡せる
        - 「より少ない台数でより広範囲をカバーすることでコストを下げたい」

#### トレーサビリティ・マトリクス（TM）

- 行：変更要求
- 列：機能単位
- セルの値：関係の有無
- 中心的価値は、似たような要求から似たような影響範囲への類推を視覚的に誘発すること

#### 変更設計書

### 手法：命名未定（試験運用検討中）

XDDP を参考に、自社向けに整備した手法。

#### 変更要求仕様書（TM を兼ねる）

- 様式
  - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.delta.template.tsv
- 説明
  - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/WORKFLOW.md#3-%E4%B8%8A%E6%B5%81%E6%96%87%E6%9B%B8%E7%BE%A4

#### 差分設計書

## 参照

| 資料 | リンク |
|---|---|
| 要求仕様書テンプレート（派生開発用） | [requirements.delta.template.tsv](https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.delta.template.tsv) |
| 要求仕様書の設計 | [WORKFLOW.md §3. 上流文書群](https://github.com/s8sato/settings/blob/main/.vscode/blueprints/WORKFLOW.md#31-%E8%A8%AD%E8%A8%88%E5%8E%9F%E5%89%87) |
| 『「派生開発」を成功させるプロセス改善の技術と極意』清水吉男、2007 | https://gihyo.jp/book/2007/978-4-7741-3249-5 |
| 『【改訂第２版】要求を仕様化する技術・表現する技術』清水吉男、2010 | https://gihyo.jp/book/2010/978-4-7741-4257-9 |
| BABOK | https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/ |
| ISO/IEC/IEEE 29148 | https://www.iso.org/standard/72089.html |
| JIS X 0166 | https://webdesk.jsa.or.jp/books/W11M0090/?bunsyo_id=JIS%20X%200166:2021 |
