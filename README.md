# Eito Fukuda

**現場の業務を、AIで実際に回るところまで作り切る。**

理学療法士 → 法人営業 → AIエンジニア。
現在は生成AI（Claude API / Claude Code）を使って、社内業務の自動化基盤を設計・実装・運用しています。

新しいツールを試すことよりも、**「現場の人が本当に困っている場所」を見つけて、そこが実際に楽になるまでやり切ること**を大事にしています。営業と医療の現場にいた経験が、その課題設定の土台になっています。

---

## 取り組んでいること

### 業務における自動化（2024年2月〜）

| 領域 | 内容 | 成果 |
|---|---|---|
| **制作パイプライン** | 店舗向けLP・動画の自動生成（Astro + React + TypeScript / kintone連携 / 動画書き出し / CMS掲載まで一気通貫） | 従来3名体制で行っていた制作を自動化し、3名分の作業工数を削減。100店舗超の制作基盤を運用中 |
| **大規模データ処理** | 数百万件規模のリストの名寄せ・重複排除・判定ロジックをPythonで自動化 | 抽出作業を1日 → 約1時間に短縮 |
| **営業支援** | カレンダー連携 → 顧客調査 → 提案資料の自動生成 → 業務DBへの書き戻し | 商談準備の標準化と工数削減 |
| **ナレッジの資産化** | 反復業務をClaude Codeのスキルとして標準化（20本） | 担当者・端末が変わっても同一手順で再現可能に |

いずれも「動くものを作って終わり」にせず、**他の人が同じ手順で回せる形にして引き渡す**ところまでを1セットにしています。

### Claude Code の実務運用

2台のマシンで Claude Code と Codex を併用し、日常的に開発・自動化を行っています。特に以下を実務で運用中です。

- **CLAUDE.md による運用設計** — グローバル / ワークスペース / プロジェクトの3階層・59ファイルで運用。禁止操作と業務データ保護を明文化し、意図しない破壊的操作を防ぐ
- **Skills（20本）** — 反復する業務手順をスキル化。属人性を排除し、別環境でも再現できる状態に
- **MCP 連携** — kintone / LINE / X などの外部サービスをMCP経由で接続し、業務フローに組み込み
- **サブエージェント構成** — 役割を分割した複数エージェントによる並行処理

---

## 公開しているもの

### [kintone-aggregation-dashboard](https://github.com/83ptdesu/kintone-aggregation-dashboard)

kintone上の複数アプリを横断集計するダッシュボード。**MIT License / 外部ライブラリ依存なし**。

有償プラグイン（月額1万円〜）と同等の集計機能を、無料のJavaScriptカスタマイズで実現しています。COUNTIFS相当の集計、複数アプリ合算、サブテーブル対応、GUI条件ビルダー、権限制御まで実装。

> 既存の有償プラグインを否定する意図はありません。**予算の都合で導入できない現場にも選択肢があるように**、という動機で公開しています（v1.0.0 / 2026年4月）。現状はJSカスタマイズとして導入する構成のため、非エンジニアでも扱えるプラグイン化が次の課題です。

`JavaScript` `esbuild` `kintone REST API`

### [AI営業ラボ](https://ai-eigyo-lab.com)

生成AIの業務活用に関する検証記事を公開しているメディア（63記事）。

WordPress REST APIによる投稿自動化、Google Search Console APIによる検索パフォーマンス分析、SNS運用の自動化まで、**運用そのものを自動化する実験場**として構築・運営しています。企画・執筆・最適化・分析を役割分割したマルチエージェント構成で回しています。

`Python` `WordPress REST API` `Google Search Console API` `MCP`

---

## 技術スタック

**言語**
`Python` `TypeScript` `JavaScript` `SQL` `HTML/CSS`

**AI / LLM**
`Claude API` `Claude Code` `Codex` `MCP (Model Context Protocol)` `RAG` `プロンプト設計`

**フレームワーク / ツール**
`Astro` `React` `GSAP` `esbuild` `Git / GitHub`

**業務システム連携**
`kintone (REST API / JSカスタマイズ)` `WordPress REST API` `SharePoint` `Google Calendar API` `Google Search Console API` `LINE Messaging API`

---

## 資格

理学療法士（国家資格）

---

## Contact

- X: [@eito_salesdx](https://x.com/eito_salesdx)
- Blog: [ai-eigyo-lab.com](https://ai-eigyo-lab.com)
