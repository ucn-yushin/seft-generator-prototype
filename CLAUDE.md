# CLAUDE.md

## プロジェクト概要
- seft-generator-prototype: [一言説明]

## コーディング規約
- 言語: Python（バックエンド）、TypeScript（フロントエンド）
- すべての関数にdocstringを記載すること
- テストはpytestで記述
- 変数名: snake_case（Python）、camelCase（TypeScript）
- インデント: スペース4つ（Python）、スペース2つ（TypeScript）
1. パッケージ管理
   - `uv` のみを使用し、`pip` は絶対に使わない
   - インストール方法：`uv add package`
   - ツールの実行：`uv run tool`
   - アップグレード：`uv add --dev package --upgrade-package package`
   - 禁止事項：`uv pip install`、`@latest` 構文の使用

2. コード品質
   - すべてのコードに型ヒントを必須とする
   - パブリックAPIには必ずドキュメンテーション文字列（docstring）を付ける
   - 関数は集中して小さく保つこと
   - 既存のパターンを正確に踏襲すること
   - 行の最大長は88文字まで

## 禁止事項
- print文でのデバッグ（loggerを使うこと）
- 環境変数のハードコード

## コミットルール
- メッセージは日本語
- prefix: feat / fix / refactor / test / docs

