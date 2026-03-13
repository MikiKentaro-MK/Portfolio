# Portfolio (シンプルな動画ポートフォリオ)

このリポジトリは、YouTube動画のサムネイルと埋め込み再生を持つシンプルでスタイリッシュな静的ポートフォリオページです。GitHub Pagesで公開できます。

セットアップ手順

1. リポジトリを作成する（GitHub上）
2. このフォルダをローカルで初期化してプッシュします。

```bash
# 作業ディレクトリへ移動
cd path/to/Portfolio

# 初期化（まだリポジトリがなければ）
git init
git add .
git commit -m "Initial commit: portfolio site"

# GitHub で作成したリポジトリを origin に追加してプッシュ
# 例: git remote add origin git@github.com:YOUR_USER/YOUR_REPO.git
git remote add origin <YOUR_GIT_URL>
git push -u origin main
```

GitHub Pages で公開する

- GitHub リポジトリの `Settings` → `Pages` に移動します。
- `Build and deployment` の `Source` を `Branch: main` / `Root` に設定して保存します。
- 数分で `https://YOUR_USER.github.io/YOUR_REPO/` で公開されます。

必要な編集

- `index.html` の `YOUTUBE_ID` を再生したいYouTube動画のIDに置き換えてください（例: `dQw4w9WgXcQ`）。
- サムネイル画像を `assets/thumbnail.jpg` に置いてください。無ければプレースホルダー画像が表示されます。
- `index.html` のタイトルやテキストを適宜編集してください。

カスタムドメイン

- カスタムドメインを使う場合は `CNAME` ファイルをルートに追加し、GitHub Pages 設定でドメインを設定します。

質問や追加要望があれば教えてください。例えば：
- 複数プロジェクトのカード表示に拡張する
- 画像の最適化、Lazy load の追加
- 自動デプロイ (GitHub Actions) を追加する
