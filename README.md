🚀 クラウド型リアルタイム授業支援ツール 技術スタック案
🎯 アーキテクチャ概要
css
コピーする
編集する
VS Code Extension / React Web UI
│
(WebSocket)
│
Node.js サーバー (Express + ws)
│
クラウドにデプロイ (Render / Fly.io / Railway)
🧩 技術スタック詳細
✅ フロントエンド（Web UI）

項目 内容
フレームワーク React（Vite + TypeScript 推奨）
状態管理 Zustand（軽量・ローカル状態向け） or Context
通信 socket.io-client または WebSocket API（軽量）
UI ライブラリ shadcn/ui（Tailwind ベースで洗練） or MUI
✅ VS Code 拡張

項目 内容
言語 TypeScript
API vscode パッケージ（公式）
通信 WebSocket (ws ライブラリ） or socket.io-client
ビルド Webpack or esbuild（拡張の標準）
配布 VS Code Marketplace or .vsix 配布
✅ バックエンド

項目 内容
サーバー Node.js + Express
通信 ws（WebSocket）または socket.io
DB（必要なら） なし（最初は状態だけで OK）
デプロイ Render（無料で簡単） または Fly.io / Railway
