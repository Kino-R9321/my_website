+++
date = '2026-08-03T10:18:14+09:00'
draft = false
title = 'Hugo Commands mean'
+++

## HugoとGitの基本コマンドの意味まとめ ##
* ※　～～はファイル名

### １．記事の作成・編集
* 'nano content/post/～～.md'：記事ファイル内のテキストを編集する
* 'hugo new content/posts/～～.md'：Hugo内のcontent/posts配下に新しい記事のテンプレートを作成する
* 'rm -rf ～～：フォルダやファイルを丸ごと強制削除
* 'mkdir -p ～～：新しいディレクトリの作成コマンド（-pを付けることでまとめて作成可能 'assets/css/extended'のように階層を作れる
* 'mv 移動元～～ 移動先～～：ファイル移動コマンド

### ２．ローカル環境でのテスト確認
* 'hugo server -D'：ローカルサーバー（http://localhost:1313/）を起動しプレビューを表示させる
（インターネット上でローカルのプレビューを見れるようにする）

### ３．本番用Webファイル生成（手動ビルド）
* 'hugo -d docs'：MarkdownをHTML等のWeb用ファイルに変換し、docsフォルダに書き出す
* ※　CI/CDでパイプライン構築したから今後は不要

### ４．Githubへの送信（世界公開）
* 'git add .'：変更された全ファイルを送信対象としてステージング
* 'git commit -m "メッセージ"'：変更内容の履歴を記録（"メッセージ"はGithubのダッシュボード上に表示されるもの）
* 'git push origin main'：ローカルの記録をGithubへアップロード  この後にユーザーネームとトークンを聞かれる（トークンはCtrl + Shift + Vで貼り付けできるが表示されない。※　セキュリティの都合

### ５．エディタ内でのショートカットコマンド
* Ctrl + K：1行ずつ削除
* Ctrl + O：保存　→　Enterで完了
* Ctrl + X：nanoエディタ終了して戻る

