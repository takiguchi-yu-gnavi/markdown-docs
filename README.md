# Knowledge Share

Markdownベースのナレッジ共有プロジェクトです。

## 概要

このプロジェクトは、Markdownを使用した文書作成とナレッジ共有を目的としています。Prettierによる自動フォーマットとMarkdownlintによる品質チェックを導入しています。

## セットアップ

### 前提条件

- Node.js (version 16以上)
- npm または yarn

### インストール

### 依存関係のインストール

```bash
npm install
```

### 開発用スクリプト

```bash
# Markdownファイルをフォーマット
npm run format

# フォーマットチェック
npm run format:check

# Markdownlint実行
npm run lint

# Markdownlint自動修正
npm run lint:fix
```

## 推奨VS Code拡張機能

このプロジェクトでは以下の拡張機能を推奨しています：

- **Prettier - Code formatter**: コードの自動フォーマット
- **markdownlint**: Markdownの品質チェック
- **Markdown All in One**: Markdown編集支援
- **Markdown Preview Enhanced**: プレビュー機能強化
- **Markdown Preview Mermaid Support**: Mermaid図表サポート

## フォーマット設定

- **行の長さ**: 80文字
- **インデント**: スペース2文字
- **改行コード**: LF
- **文末セミコロン**: なし
- **クォート**: シングル

## ディレクトリ構造

```text
knowledge-share/
├── .vscode/              # VS Code設定
│   ├── settings.json     # エディタ設定
│   └── extensions.json   # 推奨拡張機能
├── docs/                 # ドキュメント
├── .prettierrc.json      # Prettier設定
├── .markdownlint.json    # Markdownlint設定
├── .prettierignore       # Prettierignore設定
├── .gitignore           # Git除外設定
├── package.json         # プロジェクト設定
└── README.md           # このファイル
```

## 貢献方法

1. フォークしてください
2. フィーチャーブランチを作成してください (`git checkout -b feature/amazing-feature`)
3. 変更をコミットしてください (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュしてください (`git push origin feature/amazing-feature`)
5. プルリクエストを開いてください

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は
[LICENSE](LICENSE)ファイルを参照してください。
