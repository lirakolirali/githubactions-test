# Codex config (GitHub Actions learning)

Codex の設定はデフォルトで `$CODEX_HOME/config.toml`（通常は `~/.codex/config.toml`）が読み込まれます。

このリポジトリには、GitHub Actions 学習向けの **プロファイル例** を `.codex/config.toml` として置いてあります。

## 使い方（おすすめ）
### 1) 既存の `~/.codex/config.toml` に追記する
すでに `~/.codex/config.toml` がある場合は、`.codex/config.toml` の `[profiles.githubactions]` と
`[projects."..."]`（任意）をコピーして追記してください。

### 2) このリポジトリの設定を一時的に使う
`CODEX_HOME` を切り替えると、このリポジトリの `.codex/config.toml` を使えます。

```sh
CODEX_HOME="$PWD/.codex" codex -p githubactions
```

## ポイント
- `profiles.githubactions` は GitHub Actions の学習・デバッグを進めやすい指示（安全面も含む）を入れています。
- `projects."...".profile` を使うと、このリポジトリでは常に `githubactions` プロファイルを使う運用にできます（環境により無効な場合があります）。

