Roblox3 Windows Installer
=========================

配布ファイル: Roblox3-Setup.exe （この1ファイルだけ渡せます）

ユーザー手順:
1) Roblox3-Setup.exe を実行
2) 画面の指示に従ってインストール
3) デスクトップまたはスタートメニューの「Roblox3」を起動
4) 登録 / ログイン → ゲーム作成 or Starter World をプレイ

データ保存先:
  %APPDATA%\roblox3\

アンインストール:
  Windows の「アプリと機能」から Roblox3 を削除

開発者向けビルド:
  npm run dist:installer:safe
  npm run dist:publish-update   ← 自動更新用ファイルを release/updates/ に出力

自動更新:
  deploy/updates/README.txt を参照
