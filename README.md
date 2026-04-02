# logical-ui-design

認知心理学、人間工学から紐解くUIデザインの学習コンテンツです。

「なんとなく見た目がいい」ではなく、なぜそのUIが理解しやすく、迷いにくく、操作しやすいのかを言語化して解説します。Markdownを中心に構成し、必要な箇所ではHTMLとCSSのサンプルを使って悪い例と良い例を比較します。

## コンテンツ方針

- 認知心理学の観点から、視認性、認知負荷、フィードバック、一貫性を整理する
- 人間工学の観点から、押しやすさ、読みやすさ、誤操作しにくさを整理する
- 見た目の好みではなく、根拠のあるUI設計として説明する
- GitHub Pagesで公開しやすいように、docs配下に教材をまとめる

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
- docs/_config.yml: GitHub Pages用の最小設定

## 拡張予定

今後は次のテーマを順次追加する想定です。

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

GitHub Pagesの公開元をmainブランチのdocsフォルダに設定する想定です。設定後はdocs/index.mdを起点にコンテンツを公開できます。

## ローカル確認

MarkdownはGitHub上またはエディタのプレビューで確認できます。HTMLサンプルはブラウザでdocs/samples/forms/index.htmlを開いて確認できます。
