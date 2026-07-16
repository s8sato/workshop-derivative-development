# 派生開発の上流をどう整備するか

勉強会発表資料 / 発表枠：25分

---

## 構成

用語に従って進行する。

- 開発種別
  - 新規開発
  - 派生開発
    - 手法
      - XDDP
        - 成果物
          - 変更要求仕様書
            - 構成要素
              - 要求 ID
              - 要求
              - 理由
            - 書き方
              - before/after で表現する
              - 範囲と理由を表現する
              - 変更仕様から変更要求を立てる
                - 例：仕様に踏み込んだ要求「カメラの首振り角度を増大したい」
          - トレーサビリティ・マトリクス（TM）
            - 行：変更要求
            - 列：機能単位
            - セルの値：関係の有無
          - 変更設計書
      - 命名未定の手法：試験運用検討中
        - 成果物
          - 変更要求仕様書
            - TM を兼ねる
            - 様式
              - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/spec/requirements.delta.template.tsv
            - 説明
              - https://github.com/s8sato/settings/blob/main/.vscode/blueprints/WORKFLOW.md#31-%E8%A8%AD%E8%A8%88%E5%8E%9F%E5%89%87
          - 差分設計書

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
