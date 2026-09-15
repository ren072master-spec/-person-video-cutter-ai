# ひとり追跡

iPhone Safari対応のブラウザ内人物追跡MVPです。動画を選び、人物を指定すると、COCO-SSDで追跡しながらその人物を中心にクロップした動画を書き出します。

## GitHub Pages
1. このフォルダの中身をGitHubリポジトリのルートへアップロード
2. Settings → Pages
3. Source: Deploy from a branch
4. Branch: main / (root) → Save

数分後 `https://<username>.github.io/<repository>/` で公開されます。

## 注意
AIモデルとTensorFlow.jsはCDNから読み込みます。初回利用時は通信が必要です。ブラウザのMediaRecorder/canvas機能を使うため、端末・iOSバージョンによって書き出し形式が異なります。
