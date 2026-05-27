Roblox3 アップデートフォルダ（GitHub にこの中身を上げる）
================================================

■ このフォルダに入れるもの
  latest.yml          … 必須（最新版の情報）
  Roblox3-Setup-x.x.x.exe … 必須（インストーラー）
  *.exe.blockmap      … あれば差分更新が速い

■ ビルドして中身を揃える
  cd C:\Users\...\Roblox3
  npm run dist:installer:safe
  npm run dist:publish-update

■ GitHub Pages で公開する例
  1. GitHub にリポジトリを作る（例: roblox3-updates）
  2. このフォルダの中身をリポジトリ直下の updates/ に push
  3. Settings → Pages → main ブランチ /docs または /root
  4. 公開 URL 例: https://YOUR_NAME.github.io/roblox3-updates/
  5. apps/desktop/electron/update-feed.json の url をその URL に変更
  6. インストーラーを再ビルドして配布

■ 現在の設定 URL（update-feed.json）
  https://example.com/roblox3/updates/

■ 確認
  ブラウザで https://example.com/roblox3/updates/latest.yml が開けること

■ exe が 100MB 超のとき
  Git LFS を使うか、exe だけ GitHub Releases、latest.yml だけ Pages など検討
