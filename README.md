# logical-ui-design

認知心理学、人間工学から紐解くUIデザインの学習コンテンツです。

「なんとなく見た目がいい」ではなく、なぜそのUIが理解しやすく、迷いにくく、操作しやすいのかを言語化して解説します。Markdownを中心に構成し、必要な箇所ではHTMLとCSSのサンプルを使って悪い例と良い例を比較します。

## コンテンツ方針

- 認知心理学の観点から、視認性、認知負荷、フィードバック、一貫性を整理する
- 人間工学の観点から、押しやすさ、読みやすさ、誤操作しにくさを整理する
- 見た目の好みではなく、根拠のあるUI設計として説明する
- MkDocs で公開しやすいように、docs配下に教材をまとめる

## ディレクトリ構成

- docs/index.md: コンテンツの入口
- docs/01-foundations.md: UI設計の基礎
- docs/02-perception-and-cognition.md: 認知と知覚の基礎
- docs/03-information-architecture-and-layout.md: 情報設計とレイアウト
- docs/04-forms-and-inputs.md: フォーム設計
- docs/05-feedback-and-response.md: 状態変化とフィードバック
- docs/06-accessibility-and-inclusive-design.md: アクセシビリティ
- docs/07-ui-review-checklist.md: UIレビューの観点
- docs/08-dashboard-prioritization.md: ダッシュボード設計
- docs/09-table-vs-card.md: テーブルとカードの使い分け
- docs/10-empty-states.md: 空状態と初回状態
- docs/11-error-permissions-timeouts.md: エラーと回復導線
- docs/12-onboarding-and-progressive-disclosure.md: オンボーディング
- docs/13-dangerous-actions.md: 危険操作の設計
- docs/14-mobile-ui-ergonomics.md: モバイルUI
- docs/15-accessibility-in-practice.md: アクセシビリティ実践編
- docs/16-ui-copywriting.md: UI文言設計
- docs/17-review-case-study.md: ケーススタディ
- docs/samples/index.md: サンプル一覧
- docs/samples/forms/index.html: フォームUIの比較サンプル
- docs/samples/forms/styles.css: サンプル用スタイル
- docs/stylesheets/extra.css: MkDocs 用の追加スタイル
- mkdocs.yml: MkDocs のサイト設定
- requirements-docs.txt: ドキュメント生成用依存関係

## 収録テーマ

現在は次のテーマを収録しています。

- ダッシュボードの情報優先順位
- テーブルとカードの使い分け
- 空状態と初回状態の設計
- エラー、権限不足、タイムアウトの設計
- オンボーディングと段階的開示
- 危険操作と安全設計
- モバイルUIとタッチ操作
- アクセシビリティ実践編
- UI文言設計
- UIレビューのケーススタディ

## 公開方針

GitHub Pages は GitHub Actions でデプロイする前提にしています。`mkdocs-material` で `docs` 配下をビルドして公開するため、章一覧、検索、サイドナビゲーション付きのドキュメントサイトとして配信されます。

このリポジトリは [mkdocs.yml](https://github.com/Moto1829/logical-ui-design/blob/main/mkdocs.yml) で Material テーマを使う設定になっているため、GitHub Pages の公開元はブランチではなく `GitHub Actions` にする必要があります。`main` ブランチの `docs/` をそのまま Pages 公開にすると、MkDocs のテーマは適用されず、Markdown を素の状態で配信する構成になります。

公開時の想定手順:

1. GitHub の `Settings > Pages` を開く
2. `Source` を `GitHub Actions` に切り替える
3. `main` ブランチへ push する
4. Actions の `Deploy GitHub Pages` が成功したら公開 URL を確認する

## ローカル確認

MkDocs で確認する場合は次の手順です。

1. `pip install -r requirements-docs.txt`
2. `mkdocs serve`
3. 表示されたローカル URL を開く

HTMLサンプルは MkDocs サイト内のサンプル一覧から辿るか、個別に `docs/samples/forms/index.html` などを直接開いて確認できます。

## 公開時の注意

- GitHub Pages 上では Markdown ファイルは `.html` として公開されるため、内部リンクは公開 URL 向けに `.html` を参照する構成にしてあります
- サンプルページは `docs/samples/` 配下の HTML をそのまま公開します
- 独自ドメインを使う場合は、別途 `docs/CNAME` を追加してください

## mkDocs の調整ポイント

- ナビゲーション構成は `mkdocs.yml` の `nav` で管理しています
- テーマは `mkdocs-material` を採用しています
- 配色や余白などの微調整は `docs/stylesheets/extra.css` に追加できます
