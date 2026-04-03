# Logical UI Design

[![Deploy GitHub Pages](https://github.com/Moto1829/logical-ui-design/actions/workflows/deploy-pages.yml/badge.svg)](https://github.com/Moto1829/logical-ui-design/actions/workflows/deploy-pages.yml)
[![GitHub Pages](https://img.shields.io/badge/site-GitHub%20Pages-0f172a)](https://Moto1829.github.io/logical-ui-design/)
[![MkDocs Material](https://img.shields.io/badge/docs-MkDocs%20Material-4051b5)](https://squidfunk.github.io/mkdocs-material/)

認知心理学と人間工学を土台に、UI デザインを感覚論ではなく言語化して学ぶための教材です。

「なんとなく見た目がいい」ではなく、なぜその UI が理解しやすく、迷いにくく、操作しやすいのかを説明できるようにすることを目的にしています。Markdown の解説記事と、HTML/CSS の比較サンプルを組み合わせて構成しています。

公開サイト: https://Moto1829.github.io/logical-ui-design/

## このリポジトリで扱うこと

- 認知負荷、視線誘導、一貫性といった UI 設計の基本
- フォーム、フィードバック、空状態、失敗状態、危険操作の設計
- モバイル UI、アクセシビリティ、UI 文言、レビュー観点
- 悪い例と良い例を比較できる HTML/CSS サンプル

## 特徴

- 見た目の好みではなく、判断根拠で UI を説明する構成
- 章ごとの解説と比較サンプルを行き来しやすい設計
- GitHub Pages でそのまま公開できる MkDocs 構成
- MkDocs Material を使った検索付きドキュメントサイト

## こんな人向け

- UI デザインを感覚で作っていて、レビュー時に言葉にしづらい人
- 実装者として、使いやすさの観点を設計に持ち込みたい人
- デザインレビューの観点を体系化したい人
- フォームやエラー設計など、実務で崩れやすい UI を整理したい人

## 読みはじめ方

- 基礎から読む: [docs/01-foundations.md](docs/01-foundations.md)
- サンプルから入る: [docs/samples/index.md](docs/samples/index.md)
- レビュー観点を先に見る: [docs/07-ui-review-checklist.md](docs/07-ui-review-checklist.md)

代表的な比較サンプル:

- フォーム UI: [docs/samples/forms/index.html](docs/samples/forms/index.html)
- フィードバック設計: [docs/samples/feedback/index.html](docs/samples/feedback/index.html)
- エラー状態: [docs/samples/error-states/index.html](docs/samples/error-states/index.html)
- UI レビューケース: [docs/samples/review-case/index.html](docs/samples/review-case/index.html)

## 収録テーマ

- UI 設計の基礎
- 人はどう画面を認知するか
- 情報設計とレイアウト
- フォームと入力 UI
- 状態変化とフィードバック
- アクセシビリティとインクルーシブデザイン
- UI レビューの観点
- ダッシュボードの情報優先順位
- テーブルとカードの使い分け
- 空状態と初回状態の設計
- エラー、権限不足、タイムアウトの設計
- オンボーディングと段階的開示
- 危険操作と安全設計
- モバイル UI とタッチ操作
- アクセシビリティ実践編
- UI 文言設計
- UI レビューのケーススタディ

## ローカルで確認する

前提:

- Python 3.12 以上を推奨

手順:

1. `pip install -r requirements-docs.txt`
2. `mkdocs serve`
3. 表示されたローカル URL を開く

ビルド確認だけ行う場合:

1. `pip install -r requirements-docs.txt`
2. `mkdocs build --strict`

補足:

- HTML サンプルは MkDocs サイト内のサンプル一覧から辿れます
- 個別に確認したい場合は `docs/samples/.../index.html` を直接開いても確認できます

## GitHub Pages で公開する

このリポジトリは GitHub Actions 経由で GitHub Pages にデプロイする前提です。`docs/` をそのままブランチ公開するのではなく、MkDocs でビルドした静的サイトを Actions から配信します。

理由:

- Material テーマを適用した状態で公開するため
- ナビゲーション、検索、追加 CSS を含んだサイトとして配信するため

公開手順:

1. GitHub の `Settings > Pages` を開く
2. `Source` を `GitHub Actions` に切り替える
3. `main` ブランチへ push する
4. `Deploy GitHub Pages` ワークフローの成功を確認する
5. 公開 URL を開く

設定ファイル:

- MkDocs 設定: [mkdocs.yml](mkdocs.yml)
- Pages ワークフロー: [.github/workflows/deploy-pages.yml](.github/workflows/deploy-pages.yml)

## ディレクトリ構成

```text
docs/
	index.md                        サイトトップ
	01-17 の各章                    学習コンテンツ本体
	review-template.md             UIレビュー用テンプレート
	samples/
		index.md                     サンプル一覧
		*/index.html                 各比較サンプル
		*/styles.css                 各サンプル用スタイル
	stylesheets/extra.css          MkDocs 用の追加スタイル
mkdocs.yml                       サイト設定
requirements-docs.txt            ドキュメント生成用依存関係
.github/workflows/deploy-pages.yml GitHub Pages デプロイ設定
```

## 技術構成

- MkDocs
- MkDocs Material
- GitHub Pages
- GitHub Actions
- HTML/CSS による比較サンプル

## カスタマイズポイント

- ナビゲーション構成は [mkdocs.yml](mkdocs.yml) の `nav` で管理
- テーマ設定は [mkdocs.yml](mkdocs.yml) の `theme` を編集
- 見た目の微調整は [docs/stylesheets/extra.css](docs/stylesheets/extra.css) に追加
- 教材本文は [docs](docs) 配下の Markdown を編集
- サンプル UI は [docs/samples](docs/samples) 配下の HTML/CSS を編集

## ライセンス

[LICENSE](LICENSE) を参照してください。
