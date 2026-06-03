# Agent Company

高知県内の店舗向け「AI × Web制作」サービスのオペレーションシステム。

## リポジトリ構成

```
agent-company/
  templates/
    beauty-salon/   ← 美容室テンプレート（Astro + Tailwind）
    ramen/          ← 飲食店テンプレート A〜G案
  workflows/
    content-generator.json  ← n8nコンテンツ自動生成ワークフロー
```

## 関連リポジトリ

| リポジトリ | 用途 |
|---|---|
| [beauty-salon-template](https://github.com/gakukukiku/beauty-salon-template) | Cloudflare Pages デプロイ用テンプレート |

## セットアップ

### テンプレート開発
```bash
cd templates/beauty-salon
npm install
npm run dev
```

### デプロイ
mainブランチへpushすると GitHub Actions が自動でCloudflare Pagesにデプロイします。

## 環境変数

`.env.example` を参照してください。APIキーは直接チームメンバーに共有します（Gitには含めません）。
