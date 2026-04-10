# 開発進捗

## 現在のステータス

**フェーズ：** Firebase基盤構築 完了 → 事前準備サイト 実装中

---

## 完了済み

### Firebase設定
- [x] Firebaseプロジェクト作成（`claude-code-support`）
- [x] Google認証（Firebase Authentication）有効化
- [x] Firestore Database 作成（東京リージョン）
- [x] Firebase Storage 設定（東京リージョン・Blazeプラン）
- [x] Firebase Hosting 設定
- [x] firebase init（Firestore / Hosting / Storage）

### インフラ
- [x] GitHubリポジトリ作成（iidaatcnt/claude-code-support）
- [x] Firebase Hosting へのデプロイ確認

### 事前準備サイト（フロントエンド）
- [x] OS選択画面（Mac / Windows）
- [x] チェックリストUI（リベシティスタイル）
- [x] 必須バッジ表示
- [x] アコーディオン形式（タイトルクリックで展開）
- [x] チェックボックス（タップで完了）
- [x] プログレスバー（X / Y 完了）
- [x] 未完了のみ表示フィルター
- [x] 全項目完了で「準備完了！」バナー表示
- [x] リセット機能（確認モーダル付き）
- [x] Claudeアカウント・プランのドロップダウン
- [x] macOSバージョン確認：ChatGPT手順付き
- [x] Windows CPU種類確認：msinfo32 + ChatGPT手順付き

---

## 未着手

### Firebase連携（認証・DB）
- [ ] Firebase SDK をHTMLに組み込む
- [ ] Googleログイン機能の実装
- [ ] ログイン状態の管理（ヘッダーにユーザー情報表示）
- [ ] チェック状態をFirestoreに保存
- [ ] ページ再訪時にFirestoreから復元
- [ ] アカウント削除機能（Auth + Firestore + Storage）

### 事前準備サイト（追加機能）
- [ ] プロフィール画像アップロード（Firebase Storage）
- [ ] 主催者による個別ユーザーリセット機能

### 当日ディスプレイ
- [ ] メンバーグリッド表示（30人対応）
- [ ] 11段階ステータスの実装
- [ ] ヘルプキューパネル
- [ ] ソート・フィルター機能
- [ ] 統計ダッシュボード
- [ ] Firestoreリアルタイム同期

### 管理者機能
- [ ] 手動進捗更新
- [ ] メンバー一覧管理
- [ ] データエクスポート（CSV）

---

## 公開URL

| 環境 | URL |
|------|-----|
| 本番 | https://claude-code-support.web.app |
| Firebase Console | https://console.firebase.google.com/project/claude-code-support |
| GitHub | https://github.com/iidaatcnt/claude-code-support |

---

## 直近の作業ログ

| 日付 | 内容 |
|------|------|
| 2026-04-10 | Firebase全設定完了・Hosting公開 |
| 2026-04-10 | チェックリストHTML作成・デプロイ |
| 2026-04-10 | Windows/Mac OS確認手順をChatGPT連携で詳細化 |
| 2026-04-10 | GitHubに初回コミット・プッシュ |
