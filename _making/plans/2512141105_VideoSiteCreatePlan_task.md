# 2512141105_VideoSiteCreatePlan_task

**元計画**: `2512141105_VideoSiteCreatePlan.md`

## Phase 1: 初期セットアップ
- [ ] `./public` ディレクトリ作成
- [ ] `./public/assets/css` ディレクトリ作成
- [ ] `./public/assets/js` ディレクトリ作成
- [ ] `./public/assets/images` ディレクトリ作成
- [ ] `./public/movies` ディレクトリ作成

## Phase 2: アセットの移行と整理
- [ ] 共通CSSの抽出・統合 (`assets/css/style.css`)
- [ ] ページ固有CSSの対応
- [ ] 画像リソースの配置 (`assets/images`)

## Phase 3: HTMLコーディング
### 1. トップページ (`public/index.html`)
- [ ] `topページ/code.html` の内容移植
- [ ] パス修正 (CSS/JS/Images)
- [ ] リンク設定 (`movies/index.html`, `contact.html` 等)

### 2. 動画一覧ページ (`public/movies/index.html`)
- [ ] `動画一覧ページ/code.html` の内容移植
- [ ] 一覧リストのマークアップ整備
- [ ] 詳細ページへのリンク設定

### 3. 動画詳細ページ (`public/movies/detail.html`)
- [ ] `動画詳細ページ/code.html` の内容移植
- [ ] 動画プレーヤー実装確認
- [ ] 関連動画リンク整備

### 4. お問い合わせページ (`public/contact.html`)
- [ ] `お問い合わせページ/code.html` の内容移植
- [ ] フォームHTML構造整備

## Phase 4: JavaScript実装
- [ ] `assets/js/main.js` 作成
- [ ] 動的要素の実装 (ハンバーガーメニュー、スライダー等)

## Phase 5: 動作確認・微調整
- [ ] ローカルサーバーでの動作確認
- [ ] リンク切れ・画像表示確認
- [ ] レスポンシブ表示確認 (PC/SP)
- [ ] Metaタグ設定 (SEO)
