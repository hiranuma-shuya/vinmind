# ワインブラインドノート — 公開ページ

iOS アプリ **ワインブラインドノート** のプライバシーポリシーとサポート窓口を配信するための静的サイト。
GitHub Pages で https://hiranuma-shuya.github.io/vinmind/ に出している。

| ページ | URL |
|---|---|
| プライバシーポリシー（日本語） | `/privacy-ja.html` |
| Privacy Policy (English) | `/privacy-en.html` |
| サポート・FAQ（日本語） | `/support-ja.html` |
| Support / FAQ (English) | `/support-en.html` |

## 更新のしかた

ポリシー本文の**正準は開発リポジトリ側**（`vin-mind` の `doc/legal/privacy-policy.{ja,en}.md`）。
本文を変えたらそちらを直し、pandoc で HTML を作り直してここに反映する。

```
pandoc <正準の.md> -o privacy-ja.html --template=template.html -V lang=ja \
  -V pagetitle="プライバシーポリシー — ワインブラインドノート" ...
```

サポートページ（`support-*.md`）はこのリポジトリが正準。
