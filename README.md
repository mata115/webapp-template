# webapp-template

React + Vite による Hello World Webアプリのテンプレートプロジェクトです。
新しいプロジェクトの出発点としてご利用ください。

## 必要環境

- Node.js 18 以上

## セットアップ

```bash
npm install
```

## 開発サーバーの起動

```bash
npm run dev
```

ブラウザで `http://localhost:5173/` を開くと **Hello World** が表示されます。

## ビルド

```bash
npm run build
```

`dist/` に静的ファイルが生成されます。

## ビルド結果のプレビュー

```bash
npm run preview
```

## ディレクトリ構成

```
webapp-template/
├── index.html          # エントリーポイント HTML
├── vite.config.js      # Vite 設定
├── package.json
├── .gitignore
└── src/
    ├── main.jsx        # React マウント処理
    └── App.jsx         # ルートコンポーネント
```
