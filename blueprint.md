### ディレクトリ構成
```
├── assets/                       # CSS, JavaScript, 画像などの静的アセット
│   ├── critical.css              # クリティカルCSS（パフォーマンス最適化）
│   ├── icon-account.svg          # アカウントアイコン
│   ├── icon-cart.svg             # カートアイコン
│   └── shoppy-x-ray.svg          # テーマロゴ/アイコン
├── blocks/                       # テーマブロック（Shopify 2.0対応）
│   ├── group.liquid              # グループブロック
│   └── text.liquid               # テキストブロック
├── config/                       # テーマ全体の設定
│   ├── settings_data.json        # テーマカスタマイザーで設定された値
│   └── settings_schema.json      # テーマ設定の定義
├── layout/                       # サイト全体のレイアウト
│   ├── password.liquid           # パスワード保護ページのレイアウト
│   └── theme.liquid              # すべてのページの基礎となるメインのレイアウトファイル
├── locales/                      # 多言語対応用の翻訳ファイル
│   ├── en.default.json           # 英語の翻訳
│   └── en.default.schema.json    # 英語設定スキーマ翻訳
├── sections/                     # 再利用可能なページの構成要素
│   ├── 404.liquid                # 404エラーページセクション
│   ├── article.liquid            # ブログ記事セクション
│   ├── blog.liquid               # ブログ一覧セクション
│   ├── cart.liquid               # カートセクション
│   ├── collection.liquid         # コレクション一覧セクション
│   ├── collections.liquid        # コレクション詳細セクション
│   ├── custom-section.liquid     # カスタムセクション
│   ├── footer-group.json         # フッターグループ（Shopify 2.0）
│   ├── header-group.json         # ヘッダーグループ（Shopify 2.0）
│   ├── header.liquid             # ヘッダーセクション
│   ├── hello-world.liquid        # サンプルセクション
│   ├── page.liquid               # ページセクション
│   └── product.liquid            # 商品詳細セクション
├── snippets/                     # セクション内で使われる、より小さなコード部品
│   ├── css-variables.liquid      # CSS変数の定義
│   ├── image.liquid              # 画像レンダリング用スニペット
│   └── meta-tags.liquid          # メタタグ用スニペット
├── templates/                    # 各ページのテンプレート（JSON形式 - Shopify 2.0）
│   ├── 404.json                  # 404エラーページ
│   ├── article.json              # ブログ記事ページ
│   ├── blog.json                 # ブログ一覧ページ
│   ├── cart.json                 # カートページ
│   ├── collection.json           # コレクション詳細ページ
│   ├── gift_card.liquid          # ギフトカードページ（Liquidテンプレート）
│   ├── index.json                # ホームページ
│   ├── list-collections.json     # コレクション一覧ページ
│   ├── page.json                 # 固定ページ
│   ├── password.json             # パスワード保護ページ
│   ├── product.json              # 商品詳細ページ
│   └── search.json               # 検索結果ページ
├── .gitignore                    # Git除外ファイル
├── .shopifyignore               # Shopify CLI除外ファイル
├── .theme-check.yml             # テーマチェック設定
├── blueprint.md                 # プロジェクト設計書（このファイル）
├── CODE_OF_CONDUCT.md           # 行動規範
├── CONTRIBUTING.md              # 貢献ガイド
├── LICENSE                      # ライセンス
├── LICENSE.md                   # ライセンス詳細
└── README.md                    # プロジェクト概要
```

### 実際のファイル構成の特徴
- **Shopify 2.0対応**: JSON形式のテンプレート、section groups使用
- **パフォーマンス重視**: critical.css によるクリティカルCSS読み込み
- **開発環境整備**: .theme-check.yml, .shopifyignore等の設定ファイル完備
- **Dawn theme基盤**: Shopify公式Dawnテーマの構造に準拠