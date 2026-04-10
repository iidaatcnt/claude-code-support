# claude-code-support

Claude Code デスクトップアプリ インストールサポートイベント用のWebシステムです。

## 概要

PC初心者向けに、Claude Codeのインストールから初期体験までをサポートします。
インストールは手段であり、**Claudeを正しく理解して使いこなせるようになること**がゴールです。

## システム構成

| システム | URL | 説明 |
|--------|-----|------|
| 事前準備サイト | https://claude-code-support.web.app | 参加者が当日までに使う宿題リスト |
| 当日ディスプレイ | 開発中 | 会場の大型ディスプレイ用進捗管理 |

## 技術スタック

| 項目 | 技術 |
|------|------|
| フロントエンド | HTML5 / CSS3 / Vanilla JavaScript |
| 認証 | Firebase Authentication（Googleログイン） |
| データベース | Cloud Firestore |
| ストレージ | Firebase Storage |
| ホスティング | Firebase Hosting |
| ソース管理 | GitHub |

## ローカル開発

```bash
# リポジトリをクローン
git clone https://github.com/iidaatcnt/claude-code-support
cd claude-code-support

# Firebase CLIをインストール
npm install -g firebase-tools

# Firebaseにログイン
firebase login

# ローカルでプレビュー
firebase serve --only hosting
```

## デプロイ

```bash
# public フォルダにファイルをコピー
cp preparation_checklist.html public/index.html

# Firebase Hosting にデプロイ
firebase deploy --only hosting
```

## ファイル構成

```
claude-code-support/
├── public/
│   └── index.html              # デプロイされるファイル
├── preparation_checklist.html  # 事前準備チェックリスト（開発元）
├── firebase.json               # Firebase設定
├── firestore.rules             # Firestoreセキュリティルール
├── storage.rules               # Storageセキュリティルール
├── README.md                   # このファイル
├── SPEC.md                     # 機能仕様
└── progress.md                 # 開発進捗
```
