# Lean by Example - コードスタイルと規約

## Lean ファイルの規約
- `autoImplicit = false`（暗黙の変数宣言を禁止）
- `relaxedAutoImplicit = false`
- ファイルエンコーディング: UTF-8
- 日本語コメント・説明を多用する

## ディレクトリとファイル命名
- ディレクトリ名: PascalCase（例: `LeanByExample/`, `TypeClass/`）
- Lean ファイル名: PascalCase（例: `Tactic.lean`, `SetOption.lean`）
- 各トピックに `README.lean` を配置する慣習がある

## Lean コードの書き方
- 各概念ごとに独立した `.lean` ファイルを作成
- ファイル内に豊富な `example` を記述し、動作を示す
- `#check`, `#eval`, `#print` などの診断コマンドを積極的に使用
- `/- ... -/` のブロックコメントで説明を記述
- `-- コメント` の行コメントも使用

## lakefile.lean のスクリプト
- `script build` でドキュメントビルド
- `script test` でテスト実行
- `@[test_driver]` アノテーションを使用

## JavaScript (assets/)
- インデント: スペース（Biome の設定に従う）
