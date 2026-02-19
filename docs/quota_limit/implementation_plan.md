# AntigravityQuotaWatcher 導入計画

## 概要
ユーザーの要望である「QuotaLateLimit」(恐らくQuotaRateLimit/Quota monitoring) の導入として、提示された GitHub リポジトリ `AntigravityQuotaWatcher` (VS Code 拡張機能) をインストール・設定します。
この拡張機能は、AIモデルの配額(Quota)やレート制限(Rate Limit)の状態をVS Codeのステータスバーやダッシュボードで可視化するものです。

## 変更内容
このタスクはコードベースの変更ではなく、開発環境(IDE)へのツール導入となります。

### AntigravityQuotaWatcher 拡張機能のインストール
以下のいずれかの方法でインストールを行います：
1. **VS Code Marketplace からのインストール (推奨)**
   - 拡張機能ID: `wusimpl.antigravity-quota-watcher` (推測)
   - コマンドライン(`code --install-extension`) が利用可能であれば自動化を試みます。
2. **VSIX パッケージによる手動インストール**
   - GitHub Releases から `.vsix` をダウンロードしてインストール。

### 設定確認
- インストール後、Antigravity (IDE) の認証情報やポートを自動検出します。
- プロキシ設定が必要な場合は構成します (`http.proxySupport` 等)。

## 検証計画
### 自動検証
- `code --list-extensions` コマンドでインストール済み拡張機能リストに `wusimpl.antigravity-quota-watcher` が含まれているか確認します。

### 手動検証
- VS Code のステータスバーに Antigravity の配額情報が表示されているか確認してください。
- コマンドパレット (`Ctrl+Shift+P`) から `Antigravity Quota Watcher: Open Dashboard` を実行し、ダッシュボードが開くことを確認してください。
