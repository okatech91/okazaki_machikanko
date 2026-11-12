# 岡崎まち感光 — 招待制ガイド

このリポジトリの公開ファイルは暗号化された旅程データと、アクセスキー入力ページのみです。
GitHub Pages のURL自体は公開されていますが、旅程はブラウザ内で AES-256-GCM / PBKDF2-SHA-256 を用いて復号されます。アクセスキーはリポジトリに保存していません。

## 公開URL
https://okatech91.github.io/okazaki_machikanko/

## 公開設定
Settings → Pages → Build and deployment → Source を `GitHub Actions` に設定してください。
`main` ブランチにpushしたとき `.github/workflows/pages.yml` が `site/` をデプロイします。

## 制約（重要）
- URLへの到達やアクセスキー入力画面自体は誰にでも可能です。
- 共有キーを知る人は閲覧できます。受信者を個別に識別・取り消すことはできません。
- 暗号化の安全性はアクセスキーの強度と秘匿性に依存します。
- GitHub Pagesはユーザー別ログインを提供しません。厳密なアクセス制御にはCloudflare AccessなどのID認証が必要です。
- キーの変更時は再暗号化・再デプロイが必要です。

イベント、人物、場所の情報には未確定の箇所があります。予約・訪問確定を意味しません。