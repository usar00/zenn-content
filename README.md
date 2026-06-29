# zenn-content

[Zenn](https://zenn.dev) の記事をGitHub連携で管理するリポジトリ。

## 記事

- `articles/voicein-linux-voice-input.md` — LinuxでAPIキー登録だけで使える音声入力ツール

## 連携の仕組み

Zennのダッシュボード（デプロイ管理）でこのリポジトリを連携すると、
`main` ブランチへの push で `articles/` 以下の記事が自動で反映されます。

各記事のフロントマター:

```yaml
---
title: "記事タイトル"
emoji: "🎤"        # サムネ用の絵文字ひとつ
type: "tech"        # tech(技術記事) または idea(アイデア記事)
topics: ["linux", "openai"]  # タグ(最大5つ)
published: true     # true で公開、false で下書き
---
```

## ローカルプレビュー（任意）

```bash
npx zenn-cli@latest preview   # http://localhost:8000 で確認
npx zenn-cli@latest new:article   # 新しい記事を作る
```
