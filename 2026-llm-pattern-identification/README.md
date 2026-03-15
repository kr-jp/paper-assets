# LLMによる日本語の言語パターン識別―処理方式の効果と曖昧例の影響―

## データセットビューア

パターン一覧・候補文・プロンプトテンプレートの内容を閲覧できるウェブページ。

[言語パターン識別データセット — データセットビューア](https://pattern-identification.netlify.app/)

## リポジトリ構成

| ディレクトリ | 内容 |
|---|---|
| [`dataset/`](./dataset/) | 15パターンのデータセット |
| [`prompts/`](./prompts/) | 実験に使用したプロンプト |
| [`figures/`](./figures/) | 論文掲載図 |

### データセット構成

各パターン（P001〜P015）のフォルダーには以下の2ファイルが含まれている。

- **meta.json**: パターンの名称・用例・言語現象の記述
- **corpus_ja.jsonl**: ラベル付き候補文（正例5文・負例8文・境界例2文、計15文）

### プロンプト

`prompts/prompts.json` に、3つの処理方式（直接判定・段階的処理・多視点処理）で使用したプロンプトの全文が収録されている。

### 図リスト

1. [図1　3つの処理方式の概要](./figures/figure01-processing-methods-overview.pdf)
2. [図2　直接判定から多視点処理への適合率・再現率の変化（用例3文・除外モード）](./figures/figure02-pr-scatter-direct-to-multi.png)
3. [図3　厳格モードにおける誤検出の内訳（全6条件合計）](./figures/figure03-error-types-strict-mode.png)

