# Agent Company

高知県内の店舗向け「AI × Web制作」サービスのオペレーションシステム。

## リポジトリ一覧

| リポジトリ | 内容 | 用途 |
|---|---|---|
| [agent-company](https://github.com/gakukukiku/agent-company) | このリポジトリ。ドキュメント・ワークフロー | プロジェクト管理 |
| [beauty-salon-template](https://github.com/gakukukiku/beauty-salon-template) | 美容室向けAstroテンプレート | Cloudflare Pages デプロイ用 |
| [restaurant-templates](https://github.com/gakukukiku/restaurant-templates) | 飲食店デザイン案 A〜G | 鶏と魚など飲食店への提案用 |

## このリポジトリの構成

\`\`\`
agent-company/
  docs/
    reports/
      competitor_analysis.html  ← 競合分析レポート
  workflows/
    content-generator.json      ← n8nコンテンツ自動生成ワークフロー
  README.md
  .env.example                  ← 必要な環境変数の一覧
\`\`\`

## セットアップ

### テンプレートの確認
\`\`\`bash
# 美容室テンプレート
git clone https://github.com/gakukukiku/beauty-salon-template.git
cd beauty-salon-template && npm install && npm run dev

# 飲食店デザイン案（A〜G）
git clone https://github.com/gakukukiku/restaurant-templates.git
cd restaurant-templates && npm install && npm run dev
# → http://localhost:4321/ でA〜G案の一覧が確認できる
\`\`\`

### n8nワークフローのインポート
\`workflows/content-generator.json\` をn8n画面からインポートする。

## 環境変数

\`.env.example\` を参照。APIキーは直接チームメンバーに共有（Gitには含めない）。
