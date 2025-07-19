# Markdownライティングガイド

効果的なMarkdownドキュメントを作成するためのガイドラインです。

## 基本原則

### 1. 読みやすさを重視

- 1行の長さは80文字以内に収める
- 段落間には空行を入れる
- 見出しは階層構造を意識する

### 2. 一貫性を保つ

- 用語の統一
- フォーマットの統一
- ファイル命名規則の統一

### 3. 保守性を考慮

- 情報の重複を避ける
- 更新しやすい構造にする
- リンク切れを防ぐ

## 文書構造

### 見出し構造

```markdown
# タイトル（H1）

## 概要（H2）

### 詳細項目（H3）

#### 補足事項（H4）
```

### ファイル構成

```text
project/
├── README.md              # プロジェクト概要
├── docs/
│   ├── README.md         # ドキュメント目次
│   ├── guides/           # ガイドライン
│   │   ├── style-guide.md
│   │   └── writing-guide.md
│   ├── tutorials/        # チュートリアル
│   │   └── getting-started.md
│   └── api/              # API仕様
│       └── endpoints.md
```

## コードの記述

### インラインコード

コマンドやファイル名は`` `backtick` ``で囲みます。

例: `npm install`、`package.json`

### コードブロック

```markdown
\`\`\`言語名コードの内容 \`\`\`
```

### 言語指定の例

```javascript
// JavaScript
const greeting = 'Hello, World!'
console.log(greeting)
```

```bash
# Bash/Shell
npm install
npm run build
```

```json
{
  "name": "example",
  "version": "1.0.0"
}
```

## リストの使い方

### 箇条書き

- 順序が重要でない項目
- メリットやデメリット
- 機能の一覧

### 番号付きリスト

1. 手順を示す場合
2. 優先順位がある場合
3. 順序が重要な場合

### チェックリスト

- [ ] 未完了のタスク
- [x] 完了済みのタスク

## 表の作成

| 項目       | 説明                     | 例        |
| ---------- | ------------------------ | --------- |
| ヘッダー   | 表の見出し行             | Name, Age |
| データ行   | 実際のデータ             | John, 25  |
| 区切り文字 | ヘッダーとデータの区切り | `---`     |

### 表作成のコツ

- ヘッダーは必須
- 列の幅を揃える必要はない
- 複雑な表はHTMLを使用も可

## 画像とリンク

### 画像の挿入

```markdown
![代替テキスト](./images/example.png)
```

### リンクの種類

- **内部リンク**: `[テキスト](./path/to/file.md)`
- **外部リンク**: `[テキスト](https://example.com)`
- **アンカーリンク**: `[テキスト](#見出し)`

## 引用とノート

### 引用

> これは引用文です。複数行にわたって記述できます。

### 情報ボックス

> **注意**: 重要な注意事項
>
> **ヒント**: 役立つ情報
>
> **警告**: 危険な操作に関する警告

## Best Practices

### ✅ Good

- 見出しの前後に空行
- リストの階層を適切に使用
- コードブロックに言語を指定
- 意味のあるリンクテキスト

### ❌ Bad

- 見出しレベルを飛ばす
- 長すぎる行
- 曖昧なリンクテキスト（「こちら」など）
- フォーマットの不統一

## ツールとの連携

### Prettier

- 保存時に自動フォーマット
- 行の長さを80文字に調整
- 一貫したスタイルを維持

### markdownlint

- Markdown記法のチェック
- 問題箇所の自動修正
- 品質の向上

## 参考リンク

- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Flavored Markdown](https://github.github.com/gfm/)
- [Prettier Configuration](https://prettier.io/docs/en/configuration.html)
