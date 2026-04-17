# 群馬大学 吉原利忠教授 研究紹介ページ

教授紹介に特化した静的ページです。  
**メッセージ機能・ログイン機能は含まず**、第三者・教授とも同じ画面を利用します。

## できること

- 教授プロフィール、研究テーマ、経歴ハイライトの閲覧
- OpenAlex / Crossref からの最新文献自動取得
- 一次情報ソース（公式ページ・researchmap 等）の参照

## 起動方法

静的HTMLのみです。`index.html` をブラウザで開くだけで利用できます。

## 公開（GitHub Pages）

このリポジトリには `.github/workflows/deploy-pages.yml` があり、`main` 更新時に GitHub Pages へ自動デプロイされます。

1. GitHub リポジトリの **Settings > Pages** を開く  
2. Source は **GitHub Actions** を選択  
3. `main` へマージ後、Actions の `Deploy static site to GitHub Pages` が成功すれば公開完了

公開URL例:

- `https://<your-account>.github.io/<repository-name>/`

## 運用方針

- 第三者・教授で同一の利用体験（同一ページ）
- アカウント管理を不要化し、運用負荷を最小化
- 情報の鮮度は文献API同期で担保

## 参照情報（プロフィール根拠）

- 分子光化学研究室（吉原研究室）公式サイト
- メンバー・経歴ページ（群馬大学）
- 群馬大学 教員・研究紹介（吉原利忠）
- researchmap（吉原利忠）
- OpenAlex Author API
