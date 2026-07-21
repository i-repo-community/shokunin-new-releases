# shokunin-new-releases

職人.new (Shokunin.new) の公開サイト（ランディングページ + ユーザーマニュアル、GitHub Pages）。
Public website for Shokunin.new: landing page + user documentation, served via GitHub Pages.

## 運用ルール / Curation rule

- このリポジトリには**新規に書き起こした公開用ドキュメントのみ**を置く。ソースリポジトリのミラーやフィルタコピーではない。
- 掲載するのは「ユーザーが見るもの」のみ。インフラ構成・運用手順・開発ドキュメント・環境変数・DB スキーマ・本番ホスト名は**絶対に置かない**。
- スクリーンショットは**デモテナント（ダミーデータ）**で撮影したもののみ。実テナントの画面は使わない。
- 日本語（`ja/`）と英語（`en/`）は**必ず同時に更新**する（EN が JA から乖離しないため）。

- This repo contains **only newly written public docs** — never a mirror or filtered copy of the source repo.
- Publish what users see; never how the service is built or operated (no infrastructure docs, env vars, DB schema, production hostnames).
- Screenshots come from a **demo tenant with dummy data** only.
- Japanese (`ja/`) and English (`en/`) must be updated **in the same change**.

## サイト構成 / Site structure

- `index.md` + `_layouts/landing.html` — ランディングページ（日本語）
- `en/index.md` + `_layouts/landing-en.html` — landing page (English)
- `ja/` — 日本語ドキュメント（更新情報・はじめに・ユーザーマニュアル）
- `en/` — English docs (What's New, Getting Started, User Manual)

## ローカルプレビュー / Local preview

```
bundle install
bundle exec jekyll serve
```

→ http://localhost:4000
