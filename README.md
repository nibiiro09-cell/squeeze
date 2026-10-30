# Squeeze

バカラのスクイーズ練習ゲーム。配られた自分のカードを指でめくり（絞り）、数字を当てる静的サイト。
`index.html` 1枚だけで動く（サーバー不要）。

- 8デッキのシュー、バカラの3枚目ルールどおりに進行（相手側のカードは表向き）
- カードの端から内側へドラッグでめくる。長辺からはサイド、短辺からは足が見える
- 見えている範囲と残りのシューから、各数字の確率をヒント表示（オン/オフ可）
- 正解率はブラウザに保存

## GitHub Pages で公開する

1. GitHub で新しいリポジトリ（例: `squeeze`、Public）を作る
2. このフォルダで:

   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<ユーザー名>/squeeze.git
   git push -u origin main
   ```

3. リポジトリの Settings → Pages → Source を「Deploy from a branch」、Branch を `main` / `/ (root)` にして Save
4. 数分後に `https://<ユーザー名>.github.io/squeeze/` で開ける

GitHub を使わない場合は Netlify Drop（https://app.netlify.com/drop）にこのフォルダをドラッグするだけでも公開できる。
