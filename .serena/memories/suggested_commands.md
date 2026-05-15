# Lean by Example - 開発コマンド

## ビルド
```bash
# Lean ファイルをビルド（LeanByExample ライブラリ全体）
lake build

# mdgen + mdbook で HTML 生成（book/ ディレクトリに出力）
lake run build
```

## テスト
```bash
# テストスクリプトを実行（get_elem, parse, IO テスト等）
lake run test
```

## 個別 Lean ファイルの実行
```bash
lean --run LeanByExample/Type/IO/Cat.lean <ファイル>
```

## Lake 関連
```bash
# 依存関係の更新
lake update

# キャッシュを使ってビルド（Mathlib のキャッシュ取得）
lake exe cache get
```

## JavaScript フォーマット
```bash
# assets/ 以下の JS を Biome でフォーマット
npx biome format --write assets/
```

## Git
```bash
git status
git log --oneline
git diff
```

## CI
- `.github/workflows/ci.yml`: Lean ビルドとテスト
- `.github/workflows/deploy.yml`: mdbook のデプロイ
- `.github/workflows/update.yml`: 依存関係の自動更新
- `.github/workflows/devcontainer.yml`: devcontainer のビルド
