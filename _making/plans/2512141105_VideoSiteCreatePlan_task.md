# 2512141105_VideoSiteCreatePlan_task

**元計画**: `2512141105_VideoSiteCreatePlan.md`

## Phase 1: 初期セットアップ
- [x] `./public` ディレクトリ作成
- [x] `./public/assets/css` ディレクトリ作成
- [x] `./public/assets/js` ディレクトリ作成
- [x] `./public/assets/images` ディレクトリ作成
- [x] `./public/movies` ディレクトリ作成

## Phase 2: アセットの移行と整理
- [x] 共通CSSの抽出・統合 (`assets/css/style.css`)
- [x] ページ固有CSSの対応
- [x] 画像リソースの配置 (`assets/images`)

## Phase 3: HTMLコーディング
### 1. トップページ (`public/index.html`)
- [x] `topページ/code.html` の内容移植
- [x] パス修正 (CSS/JS/Images)
- [x] リンク設定 (`movies/index.html`, `contact.html` 等)

### 2. 動画一覧ページ (`public/movies/index.html`)
- [x] `動画一覧ページ/code.html` の内容移植
- [x] 一覧リストのマークアップ整備
- [x] 詳細ページへのリンク設定

### 3. 動画詳細ページ (`public/movies/detail.html`)
- [x] `動画詳細ページ/code.html` の内容移植
- [x] 動画プレーヤー実装確認
- [x] 関連動画リンク整備

### 4. お問い合わせページ (`public/contact.html`)
- [x] `お問い合わせページ/code.html` の内容移植
- [x] フォームHTML構造整備

## Phase 4: JavaScript実装
- [x] `assets/js/main.js` 作成
- [x] 動的要素の実装 (ハンバーガーメニュー、スライダー等)

## Phase 5: 動作確認・微調整
- [x] ローカルサーバーでの動作確認
- [x] リンク切れ・画像表示確認
- [x] レスポンシブ表示確認 (PC/SP)
- [x] Metaタグ設定 (SEO)
