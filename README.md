# DUNGEON BET — 欲望の迷宮

## Renderで公開（無料枠）
1. ZIPを解凍し、GitHubで新規リポジトリを作成。DungeonBetフォルダの中身をすべてアップロード（package.jsonがリポジトリ直下になるように）。
2. https://dashboard.render.com/ にGitHubでログイン。New → Web Service → リポジトリを選択。
3. Runtime Node、Build Command `npm install`、Start Command `npm start`、Instance Type Free。Root Directoryは空欄。Deploy。
4. 発行されたHTTPS URLを開き、名前を入力してルーム作成。友達にURLと6桁IDを共有。全員準備後、ホストが開始。

公式: https://render.com/docs/your-first-deploy
無料枠: https://render.com/docs/free
無料枠は休止・再起動があり、再起動で試合が消えます。初回アクセスは起動待ちになる場合があります。

## ローカル確認
Node.js 20以上で `npm start`、http://localhost:3000 を開く。依存ライブラリなし。別タブで別プレイヤーとして参加可能。

## 仕様
2〜6人、秘密投票、戦闘、宝箱、罠、商人、休息、祭壇、5階層ごとのボス、脱出、観戦、リザルト、手引き、1人練習、効果音。通常15/困難25/地獄50階層。時間切れ自動選択。サーバーのメモリのみ使用。通信はHTTPポーリング（約1.2秒間隔）。同じページで通信復帰可能。ページ更新では復帰不可。公開URLは友達だけに共有してください。1時間通信のないルームは削除。
