# THE fool head helper

Androidのユーザー補助機能を使い、他アプリで選択中の入力欄へ定型文を入力する補助アプリです。

## v0.3の仕組み

- 初回だけ8桁の共有キーを保存
- Fボタンを開くたびに共通APIから定型文を取得
- 取得した定型文は端末内にも保存
- 通信できない場合は前回取得分を使用
- helperから定型文の変更・送信は行わない
- WebサイトのHTMLや画面構成には依存しない

管理と送信は `the-fool-head`、保存と取得は `the-fool-shared-api` が担当します。

## APK作成

`main` ブランチへ更新するとGitHub ActionsがプロジェクトZIPを展開し、debug APKを作成します。
