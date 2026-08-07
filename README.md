# IKOMA FC奈良 × 生駒市 モルック大会 LP — GitHub Pages 公開手順

## ファイル構成
```
index.html      ← ランディングページ本体（GitHub Pagesはこのファイル名を自動でトップページとして表示）
assets/img/     ← 写真・QRコード・エンブレム画像
.nojekyll       ← GitHubのJekyll変換を無効化（画像パスの不具合防止）
```
この3点（フォルダ含む）をそのままリポジトリのルートに置いてください。

## 公開手順（無料・GitHub Pages）

1. **リポジトリを作成**
   - github.com にログイン → 右上「+」→「New repository」
   - Repository name: 任意（例: `ikoma-molkky-2027`）
   - Public を選択 → 「Create repository」

2. **ファイルをアップロード**
   - 作成したリポジトリ画面で「Add file」→「Upload files」
   - `index.html` と `assets` フォルダ（中身ごと）、`.nojekyll` をまとめてドラッグ＆ドロップ
   - 下部の「Commit changes」をクリック

3. **GitHub Pagesを有効化**
   - リポジトリの「Settings」タブ →左メニュー「Pages」
   - 「Build and deployment」→ Source: `Deploy from a branch`
   - Branch: `main` ／ フォルダ: `/(root)` を選択 →「Save」

4. **公開URLを確認**
   - 数分後、同じPages画面に以下の形式でURLが表示されます
     ```
     https://（あなたのGitHubユーザー名）.github.io/（リポジトリ名）/
     ```
   - このURLがそのまま公開ランディングページになります

## 更新したいとき
`index.html` や `assets/img` の中身を差し替えて再度アップロード（Commit）すれば、数分で反映されます。

## 独自ドメインを使いたい場合
Settings → Pages → 「Custom domain」に取得済みのドメインを入力し、DNS側でCNAMEレコードを設定してください（このステップのみ有料のドメイン取得が必要です。GitHub Pages自体は無料です）。
