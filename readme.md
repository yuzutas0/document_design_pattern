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

## What is Pattern

パターンとは

> 繰り返し発生する構造的な形で、あるコンテキストにおける問題を解決するもの。
> なんらかの全体の全体性あるいはシステムに寄与し、美的あるいは文化的な価値を反映する。

James O. Coplien ほか『組織パターン』(邦訳:翔泳社,2013)より引用

上記書籍では以下の形式で、パターンを体系化している。

- パターンの名前
- コンテキスト
- フォース・扱われている問題
- 解決策
- なぜそのパターンがうまく機能するのか
- そのパターンの強み・傾向・注意点
- 関連する他のパターン

## How to increment DDP 

1. [論点を整理する](1_hypothesis)
    - [ ] [ドキュメント構成・管理の課題を洗い出す](1_hypothesis/1_problem_of_document)
    - [ ] [[WIP] ソフトウェア開発・設計の各種手法を洗い出す](1_hypothesis/2_solution_of_engineering)
    - [ ] [適用方法を模索する](1_hypothesis/3_adapt_solution_to_problem)
2. [有効性を検証する](2_effectiveness)
    - [取り組み、成功、失敗の事例を集める](2_effectiveness/1_case_study)
    - [成功パターン・アンチパターンを分類する](2_effectiveness/2_classified_knowledge)

## Contribution

- Issueでのディスカッション
- Fork -> Commit -> PullRequest
  - PRでのディスカッション
- Gitter/Slack（Todo:作成）でのディスカッション
