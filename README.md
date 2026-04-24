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

## GitHubアカウント名を出さずに公開する（独自ドメイン）

GitHub Pages のURL（`<your-account>.github.io`）を見せたくない場合は、独自ドメインを使います。
このリポジトリには `CNAME.example` を追加してあります。

### 手順（あなた側で必要）

1. ドメインを取得（例: `lab-intro.jp`）
2. DNSを設定
   - サブドメイン運用（推奨）例: `www.lab-intro.jp`
   - `CNAME` レコードを `ymd-yamada.github.io` に向ける
3. このリポジトリのルートに `CNAME` ファイルを作成し、独自ドメインのみを1行で記載
   - 例: `www.lab-intro.jp`
4. GitHub の **Settings > Pages** で Custom domain に同じ値を設定
5. 「Enforce HTTPS」を有効化

### 補足

- apexドメイン（`lab-intro.jp`）を使う場合は、DNSプロバイダごとの `A/ALIAS/ANAME` 設定が必要です。
- 設定反映には数分〜最大48時間かかる場合があります。

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
