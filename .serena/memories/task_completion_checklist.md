# Lean by Example - タスク完了時のチェックリスト

## Lean ファイルを変更した場合
1. `lake build` でビルドエラーがないか確認
2. 変更したファイルが `LeanByExample/` 以下の場合、該当する `.lean` ファイルの `example` が正しく動作することを確認

## ドキュメントを変更した場合
1. `lake run build` で HTML が正しく生成されるか確認
2. `booksrc/SUMMARY.md` に新しいページが正しく追加されているか確認

## テストが必要な場合
1. `lake run test` でテストが全てパスすることを確認

## JavaScript (assets/) を変更した場合
1. Biome でフォーマット: `npx biome format --write assets/`
