# Lean by Example - プロジェクト概要

## 目的
Lean 言語（プログラミング言語かつ定理証明支援系）と主要ライブラリの使い方を、豊富なコード例と共に解説する日本語の学習資料。
- 公開URL: https://lean-ja.github.io/lean-by-example/
- GitHub: https://github.com/lean-ja/lean-by-example

## 技術スタック
- **言語**: Lean 4 (leanprover/lean4:v4.30.0-rc2)
- **ビルドツール**: Lake（Lean のパッケージマネージャー）
- **ドキュメント生成**: mdgen（Lean → Markdown）+ mdbook（Markdown → HTML）
- **依存ライブラリ**: Mathlib4, Std, mdgen
- **JavaScript フォーマッター**: Biome（インデントはスペース）
- **ライセンス**: CC BY-NC-SA 4.0

## プロジェクト構成
```
lakefile.lean         # Lake ビルド設定
lean-toolchain        # Lean バージョン指定
book.toml             # mdbook 設定
biome.json            # JS フォーマッター設定
LeanByExample/        # メインの Lean ソースファイル群
  Attribute/          # @[...] 属性の解説
  Declarative/        # 宣言コマンドの解説
  Diagnostic/         # 診断コマンドの解説
  DoSyntax/           # do 構文の解説
  Modifier/           # 修飾子の解説
  Option/             # オプションの解説
  Syntax/             # 構文の解説
  Tactic/             # タクティクの解説
  Type/               # 型の解説
  TypeClass/          # 型クラスの解説
Exe/                  # 実行可能な補助プログラム
booksrc/              # mdbook のソース（生成された Markdown）
assets/               # mdbook の JS/CSS アセット
```
