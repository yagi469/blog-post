---
description: Google Driveのドキュメント/PDFからはてなブログ向けのMarkdown記事を作成する
---

# ブログ記事作成ワークフロー

このワークフローでは、Google Driveのドキュメント/PDFからはてなブログ向けのMarkdown記事を作成します。

## 前提条件

- Google Drive MCP サーバーが利用可能であること
- ブログ記事のソースとなるドキュメント/PDFがGoogle Driveに存在すること

## 手順

### 1. スキルの読み込み

`.agent/skills/blog-post/SKILL.md` を読み込んで、ブログ記事作成の手順を確認する。

### 2. ソースの特定

ユーザーに投稿テーマまたはソースファイルを確認する。

- Google Driveでファイルを検索: `mcp_gdrive_gdrive_search` を使用
- フォルダ内のファイルを一覧: `mcp_gdrive_gdrive_list` を使用

### 3. ソースの読み込み

// turbo
`mcp_gdrive_gdrive_read` でソースファイルの内容を取得する。

### 4. アウトラインの作成と確認

ソース内容に基づいて記事のアウトラインを作成し、ユーザーに確認する。

- 記事タイトル案を3つ提案
- 適切なテンプレートを選択（tech_tutorial / review / learning_note）
- アウトラインを提示

### 5. 記事の執筆

承認されたアウトラインに基づいて、はてなブログ向けMarkdownで記事を執筆する。

### 6. レビューと修正

ユーザーにレビューしてもらい、フィードバックを反映する。

### 7. 保存

#### ローカルプロジェクトに保存

下書きの場合:

```
c:\Users\user\Dev\blog-post\drafts\YYYY-MM-DD_slug-title.md
```

公開版の場合:

```
c:\Users\user\Dev\blog-post\posts\YYYY-MM-DD_slug-title.md
```

#### Google Driveに保存

`mcp_gdrive_gdrive_create_file` を使って「ブログ記事」フォルダ (ID: `1ydDh4Ml7U756ZGnPg9_TdL9njeTdgDtb`) にGoogle Docs形式で保存する。
