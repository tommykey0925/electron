# Electron App

シンプルなElectronアプリケーションです。

## 必要な環境

- Node.js
- pnpm
- WSLgが有効なWSL環境（GUIアプリ起動のため）

## セットアップ

依存関係をインストール：

```bash
pnpm install
```

## 起動方法

### WSL環境で起動

WSLgが有効なWSL環境で以下を実行：

```bash
pnpm start
```

アプリケーションが起動し、開発者ツールが自動的に開きます。

### 開発者ツールについて

起動時に自動的に開発者ツール（DevTools）が開きます。以下の機能が利用できます：

- **Console**: JavaScriptのログやエラー確認
- **Elements**: HTMLとCSSの検証・編集
- **Network**: ネットワークリクエストの監視
- **Sources**: JavaScriptのデバッグ

## 注意事項

- このアプリはGUIを必要とするため、ヘッドレス環境（Dockerコンテナなど）では起動できません
- WSL環境での起動には、WSLg（Windows 11）またはX Server（VcXsrv、X410など）が必要です
- `DISPLAY`環境変数が正しく設定されていることを確認してください

## プロジェクト構成

```
.
├── main.js          # メインプロセス
├── preload.js       # プリロードスクリプト
├── renderer.js      # レンダラープロセス
├── index.html       # メインHTML
├── style.css        # スタイル
└── package.json     # プロジェクト設定
```
