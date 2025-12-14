# 動画紹介Webサイト作成計画書

**作成日時**: 2025-12-14 11:05
**作成者**: Antigravity

## 1. 概要
デザインデータ（Google Stitch出力）を元に、動画紹介Webサイトを構築する。
コーディング規約に基づき、`./public` をドキュメントルートとして静的HTMLサイトを作成する。

## 2. ディレクトリ構成計画

### ドキュメントルート
`./public`

### 構成詳細
```text
./public/
├── index.html                  # トップページ (Source: topページ/code.html)
├── contact.html                # お問い合わせページ (Source: お問い合わせページ/code.html)
├── movies/
│   ├── index.html              # 動画一覧ページ (Source: 動画一覧ページ/code.html)
│   └── detail.html             # 動画詳細ページ (Source: 動画詳細ページ/code.html)
└── assets/
    ├── css/
    │   ├── style.css           # 共通スタイル
    │   └── [page].css          # ページ固有スタイル（必要に応じて）
    ├── js/
    │   └── main.js             # 共通スクリプト
    └── images/
        └── [extracted_images]  # デザインから書き出した画像
```

## 3. 作成ルール
1.  **公開ディレクトリ**: `public/`
2.  **アセット配置**: `public/assets/` 以下に配置。
3.  **JavaScript**: 標準機能（Vanilla JS）のみ使用。ライブラリ依存を避ける。
4.  **デザインソース**: `_making/stitch_desing/` 以下の各フォルダ内の `code.html` をベースにする。

## 4. 作業手順

### Phase 1: 初期セットアップ
1.  `./public` ディレクトリおよびサブディレクトリ（`assets/css`, `assets/js`, `assets/images`, `movies`）を作成する。

### Phase 2: アセットの移行と整理
1.  各 `code.html` から共通で使用されているCSSを抽出し、`assets/css/style.css` に統合する。
2.  各ページ固有のCSSは、共通CSSの下に記述するか、メンテナンス性を考慮して分離を検討する。
3.  デザインに含まれる画像リソースを `assets/images` に配置する（画像の書き出しやパスの修正を含む）。

### Phase 3: HTMLコーディング
各デザインフォルダの `code.html` をベースに、Web標準に合わせてマークアップを最適化する。

#### 1. トップページ (`topページ` -> `public/index.html`)
*   `code.html` の内容を移植。
*   CSS/JS/画像パスを `assets/` 以下のパスに修正。
*   リンク先を各HTMLファイルへのパス（`movies/index.html`, `contact.html` 等）に設定。

#### 2. 動画一覧ページ (`動画一覧ページ` -> `public/movies/index.html`)
*   一覧リストのマークアップを整備。
*   各動画へのリンクを詳細ページ（`detail.html`）へ繋ぐ。

#### 3. 動画詳細ページ (`動画詳細ページ` -> `public/movies/detail.html`)
*   動画プレーヤー部分（iframeやvideoタグ）の実装確認。
*   関連動画リンク等の整備。

#### 4. お問い合わせページ (`お問い合わせページ` -> `public/contact.html`)
*   フォームのHTML構造を整備。
*   （バックエンド機能がないため、静的フォームとしての体裁を整える）

### Phase 4: JavaScript実装
1.  `assets/js/main.js` を作成。
2.  ハンバーガーメニュー、スライダー、モーダル等の動的要素があれば実装する（デザイン依存）。

### Phase 5: 動作確認・微調整
1.  ローカルサーバーで動作確認。
2.  リンク切れ、画像表示崩れがないか確認。
3.  PC/SPレスポンシブ表示の確認。

## 5. 留意事項
*   Google Stitchが出力するコードは冗長な場合があるため、可読性とメンテナンス性を考慮して適宜リファクタリングを行う。
*   SEOの観点から、適切なmetaタグ（title, description等）を設定する。
