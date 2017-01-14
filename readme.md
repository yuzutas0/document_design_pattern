# Document Design Pattern

- 邦題：ドキュメント・デザイン・パターン
- 略称：DDP

## What is DDP

- 目的：ドキュメント構成の保守性・可用性の向上
- 仮説：ソフトウェアエンジニアリングの概念・設計手法をドキュメント構成に適用する

```
例) 3つのドキュメント

「A:管理しているサーバの基本情報一覧」
「B:X日のインフラ保守作業手順書」
「C:Y日の試験環境に関するメモ」

これらは「A <- B」「A <- C」の依存関係にある。
この場合、各所から参照されるAを「Util」として隔離してはどうか。
少なくとも、BやCのように1度しか使われない「ログ」のような情報と、
Aのように更新される「レコード」のような情報は分けて管理してはどうか。
```

## How to increment DDP 

1. 論点を整理する
    - 各種設計手法を洗い出す。
    - ドキュメント構成・管理の課題を洗い出す。
    - 適用方法を模索する。
2. 有効性を検証する
    - 取り組み、成功・失敗の事例を集める。
    - 成功パターン・アンチパターンを分類する。

## Contribution

- Gitter/Slack（Todo:作成）でのディスカッション
- Issueでのディスカッション
- Fork -> Commit -> PullRequest
  - PRでのディスカッション
