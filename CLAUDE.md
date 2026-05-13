# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 開発コマンド

```bash
npm run dev      # 開発サーバー起動 (http://localhost:5173/)
npm run build    # プロダクションビルド (dist/ へ出力)
npm run preview  # プロダクションビルドのプレビュー
```

テスト・リントの設定は現時点では未構成。

## 技術スタック

- **フレームワーク:** React 18 (StrictMode / createRoot API 使用)
- **ビルドツール:** Vite 6 + @vitejs/plugin-react
- **モジュール形式:** ES Modules (`"type": "module"`)
- **言語:** JSX（TypeScript 未導入）

## アーキテクチャ

エントリポイントの流れ: `index.html` → `src/main.jsx` → `src/App.jsx`

`vite.config.js` でサーバーが `0.0.0.0` にバインドされているため、同一ネットワーク上の他端末からもアクセス可能。

新機能追加時は `src/` 以下にコンポーネント・ページ・ユーティリティを整理して配置すること。
