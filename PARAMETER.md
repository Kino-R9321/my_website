# Webポートフォリオサイト パラメータシート 

 

## 1. リポジトリ・環境基本パラメータ 

| パラメータ項目 | 設定値 / 値 | 備考 | 

| :--- | :--- | :--- | 

| **GitHub アカウント名** | `kino-r9321` | | 

| **リポジトリ名** | `my_website` | Publicリポジトリ | 

| **本番公開URL（トップ）** | `https://kino-r9321.github.io/my_website/` | GitHub Pages | 

| **本番公開URL（記事一覧）** | `https://kino-r9321.github.io/my_website/posts/` | ナビゲーション対象 | 

| **本番公開URL（障害対応ログ）**| `https://kino-r9321.github.io/my_website/posts/troubleshooting/` | ナビゲーション対象 | 

| **ローカル検証URL（トップ）** | `http://localhost:1313/my_website/` | `hugo server -D` 実行時 | 

| **ローカル検証URL（障害対応ログ）**| `http://localhost:1313/my_website/posts/troubleshooting/` | 実環境確認済パス | 

| **デフォルトブランチ** | `main` | ソースコード管理用 | 

| **デプロイ対象ブランチ** | `gh-pages` | GitHub Actionsが自動生成・配信 | 

 

--- 

 

## 2. Hugo設定ファイルパラメータ（`hugo.toml`） 

| パラメータキー | 設定値 | 説明 | 

| :--- | :--- | :--- | 

| `baseURL` | `'https://kino-r9321.github.io/my_website/'` | 本番サイトのベースURL（リンク切れ対策済） | 

| `languageCode` | `'ja-jp'` | 言語設定 | 

| `title` | `'My New Hugo Site'` （または任意の名称） | サイトタイトル | 

| `theme` | `'PaperMod'` | 使用テーマ名 | 

| `params.assets.disableHLJS` | `false` | シンタックスハイライト有効化 | 

| `[[menu.main]]` | `name = 'Posts'`, `url = '/posts/'`, `weight = 10` | メインメニュー（記事一覧）設定 | 

 

--- 

 

## 3. ディレクトリ・ファイル配置パラメータ 

| 配置パス | 役割・格納ファイル | 備考 | 

| :--- | :--- | :--- | 

| `content/posts/` | Markdown記事ファイル（`.md`） | 投稿データ格納場所 | 

| `content/posts/troubleshooting.md` | 障害対応・トラブルシューティングメモ | 全10項目の対応ログ | 

| `themes/PaperMod/` | PaperModテーマ本体 | サブモジュール／テーマ領域 | 

| `assets/css/extended/custom.css` | カスタムCSS | 見出しスタイル・カラー調整等 | 

| `.github/workflows/hugo.yml` | GitHub Actionsワークフロー定義 | 自動ビルド・デプロイ定義 | 

| `./DESIGN.md` | 基本設計書 | ルート直下に配置 | 

| `./PARAMETER.md` | 本パラメータシート | ルート直下に配置 | 
