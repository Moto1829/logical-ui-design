---
title: UIデザインを言語化する
---

# UIデザインを言語化する

このコンテンツは、UIデザインを感覚ではなく根拠で説明できるようにするための学習ノートです。

見た目が整っていることは大切ですが、それだけでは十分ではありません。ユーザーは画面を鑑賞するのではなく、理解し、判断し、操作します。つまりUIデザインでは、次の3点を同時に考える必要があります。

- すぐ理解できること
- 迷わず選べること
- 安心して操作できること

そのために本コンテンツでは、認知心理学と人間工学を土台にして、UIがどうあるべきかを整理します。

## はじめての方へ

最初に迷わないために、入口を3つに分けています。

- 基礎から順に学ぶ: [第1章 UI設計の基礎](01-foundations.html) から読み進める
- よくある実務テーマから入る: [フォームと入力UI](04-forms-and-inputs.html) や [状態変化とフィードバック](05-feedback-and-response.html) を先に読む
- 画面比較から入る: [サンプル一覧](samples/index.html) から悪い例と良い例を見る

## この教材で身につくこと

本コンテンツは、次の流れで学べるように設計しています。

1. UIの基礎概念を理解する
2. 人が画面をどう知覚し、どう迷うかを理解する
3. レイアウト、文字、色、余白を根拠を持って扱えるようにする
4. フォーム、ボタン、フィードバックなど具体的なUI部品に落とし込む
5. アクセシビリティとレビュー観点まで含めて、自分で評価できるようにする

## 対象読者

- 見た目のバランスでUIを作ってきた人
- デザインレビューで根拠をうまく言語化できない人
- 実装者として、使いやすさの観点を設計に持ち込みたい人

## 読み進め方

1. まずは[UI設計の基礎](01-foundations.html)を読む
2. HTMLとCSSのサンプルを開いて、悪い例と良い例を比較する
3. 実案件の画面に当てはめて、どの原則が崩れているかを確認する

## 目的別の読み方

### まずは基礎を固めたい

1. [第1章 UI設計の基礎](01-foundations.html)
2. [第2章 人はどう画面を認知するか](02-perception-and-cognition.html)
3. [第3章 情報設計とレイアウト](03-information-architecture-and-layout.html)

### 実務でよく触るUIから見たい

1. [第4章 フォームと入力UI](04-forms-and-inputs.html)
2. [第5章 状態変化とフィードバック](05-feedback-and-response.html)
3. [第10章 空状態と初回状態の設計](10-empty-states.html)
4. [第11章 エラー、権限不足、タイムアウトの設計](11-error-permissions-timeouts.html)

### レビュー観点を先に持ちたい

1. [第6章 アクセシビリティとインクルーシブデザイン](06-accessibility-and-inclusive-design.html)
2. [第7章 UIレビューの観点](07-ui-review-checklist.html)
3. [第17章 UIレビューのケーススタディ](17-review-case-study.html)
4. [UIレビュー用テンプレート](review-template.html)

## 順番に読む

1. [第1章 UI設計の基礎](01-foundations.html)
2. [第2章 人はどう画面を認知するか](02-perception-and-cognition.html)
3. [第3章 情報設計とレイアウト](03-information-architecture-and-layout.html)
4. [第4章 フォームと入力UI](04-forms-and-inputs.html)
5. [第5章 状態変化とフィードバック](05-feedback-and-response.html)
6. [第6章 アクセシビリティとインクルーシブデザイン](06-accessibility-and-inclusive-design.html)
7. [第7章 UIレビューの観点](07-ui-review-checklist.html)
8. [第8章 ダッシュボードの情報優先順位](08-dashboard-prioritization.html)
9. [第9章 テーブルとカードの使い分け](09-table-vs-card.html)
10. [第10章 空状態と初回状態の設計](10-empty-states.html)
11. [第11章 エラー、権限不足、タイムアウトの設計](11-error-permissions-timeouts.html)
12. [第12章 オンボーディングと段階的開示](12-onboarding-and-progressive-disclosure.html)
13. [第13章 危険操作と安全設計](13-dangerous-actions.html)
14. [第14章 モバイルUIとタッチ操作](14-mobile-ui-ergonomics.html)
15. [第15章 アクセシビリティ実践編](15-accessibility-in-practice.html)
16. [第16章 UI文言設計](16-ui-copywriting.html)
17. [第17章 UIレビューのケーススタディ](17-review-case-study.html)
18. [UIレビュー用テンプレート](review-template.html)

## サンプルから入る

画面比較から理解したい場合は、次のサンプルから入ると全体像をつかみやすくなります。

- 迷いやすい入力画面: [フォームUIの比較サンプル](samples/forms/index.html)
- 反応が弱く不安になりやすい画面: [フィードバック設計の比較サンプル](samples/feedback/index.html)
- 一覧や検索で情報整理に迷いやすい画面: [一覧画面の比較サンプル](samples/list-view/index.html)
- 実務で崩れやすい失敗状態: [エラー状態の比較サンプル](samples/error-states/index.html)
- レビューの言語化例を見たい場合: [UIレビューケースの比較サンプル](samples/review-case/index.html)

## 学習の前提

UIデザインの評価軸は、単に美しいかどうかではありません。少なくとも次の観点で説明できる必要があります。

- 情報がすばやく知覚できるか
- 次に何をすべきか判断しやすいか
- 操作結果が予測しやすいか
- 誤操作しにくく、復帰しやすいか

この軸を持つと、配色、余白、文字サイズ、ボタン配置などの見た目上の判断にも意味づけができます。

## 収録コンテンツ

- [第1章 UI設計の基礎](01-foundations.html)
- [第2章 人はどう画面を認知するか](02-perception-and-cognition.html)
- [第3章 情報設計とレイアウト](03-information-architecture-and-layout.html)
- [第4章 フォームと入力UI](04-forms-and-inputs.html)
- [第5章 状態変化とフィードバック](05-feedback-and-response.html)
- [第6章 アクセシビリティとインクルーシブデザイン](06-accessibility-and-inclusive-design.html)
- [第7章 UIレビューの観点](07-ui-review-checklist.html)
- [第8章 ダッシュボードの情報優先順位](08-dashboard-prioritization.html)
- [第9章 テーブルとカードの使い分け](09-table-vs-card.html)
- [第10章 空状態と初回状態の設計](10-empty-states.html)
- [第11章 エラー、権限不足、タイムアウトの設計](11-error-permissions-timeouts.html)
- [第12章 オンボーディングと段階的開示](12-onboarding-and-progressive-disclosure.html)
- [第13章 危険操作と安全設計](13-dangerous-actions.html)
- [第14章 モバイルUIとタッチ操作](14-mobile-ui-ergonomics.html)
- [第15章 アクセシビリティ実践編](15-accessibility-in-practice.html)
- [第16章 UI文言設計](16-ui-copywriting.html)
- [第17章 UIレビューのケーススタディ](17-review-case-study.html)
- [UIレビュー用テンプレート](review-template.html)
- [サンプル一覧](samples/index.html)
- [フォームUIの比較サンプル](samples/forms/index.html)

## 主要サンプルへの近道

- [フォームUIの比較サンプル](samples/forms/index.html)
- [ボタン優先順位の比較サンプル](samples/buttons/index.html)
- [フィードバック設計の比較サンプル](samples/feedback/index.html)
- [モーダル設計の比較サンプル](samples/modals/index.html)
- [一覧画面の比較サンプル](samples/list-view/index.html)
- [検索UIとフィルタUIの比較サンプル](samples/search-filters/index.html)

## 章とサンプルの対応

- 第4章: [フォームUIの比較サンプル](samples/forms/index.html)
- 第4章: [ボタン優先順位の比較サンプル](samples/buttons/index.html)
- 第5章: [フィードバック設計の比較サンプル](samples/feedback/index.html)
- 第5章: [モーダル設計の比較サンプル](samples/modals/index.html)
- 第3章: [一覧画面の比較サンプル](samples/list-view/index.html)
- 第3章: [検索UIとフィルタUIの比較サンプル](samples/search-filters/index.html)
- 第8章: [ダッシュボードの比較サンプル](samples/dashboard/index.html)
- 第9章: [テーブルとカードの比較サンプル](samples/table-vs-card/index.html)
- 第10章: [空状態の比較サンプル](samples/empty-states/index.html)
- 第11章: [エラー状態の比較サンプル](samples/error-states/index.html)
- 第12章: [オンボーディングの比較サンプル](samples/onboarding/index.html)
- 第13章: [危険操作の比較サンプル](samples/danger-actions/index.html)
- 第14章: [モバイルUIの比較サンプル](samples/mobile/index.html)
- 第15章: [アクセシビリティ実践サンプル](samples/accessibility/index.html)
- 第16章: [UI文言設計の比較サンプル](samples/copywriting/index.html)
- 第17章: [UIレビューケースの比較サンプル](samples/review-case/index.html)

## 次に深められる内容

- 章ごとのチェックリスト拡充
- 実案件ベースのケーススタディ追加
- GitHub Pages向けの見た目と導線の最終調整

## 補助リンク

- [サンプル一覧](samples/index.html)
- [UIレビュー用テンプレート](review-template.html)
- [第8章以降を読む](08-dashboard-prioritization.html)