# Codex instructions (project)

このリポジトリは Vite + React + Vitest の最小構成です。

## 目的
- 変更は小さく、意図が分かる単位で行う
- 可能なら `npm test` が通るところまで確認する

## よく使うコマンド
- 依存関係: `npm ci`
- テスト: `npm test`（= `vitest run`）
- ウォッチ: `npm run test:watch`
- ビルド: `npm run build`
- 開発: `npm run dev`

## 変更方針
- `node_modules/` は編集しない
- 依存関係を変えない限り `package-lock.json` は触らない
- 既存のスタイル（ESM, React関数コンポーネント）に合わせる

## 主要ファイル
- `index.html`
- `src/App.jsx`
- `src/App.test.jsx`
- `src/setUpTests.js`
- `.github/workflows/ci.yml`

