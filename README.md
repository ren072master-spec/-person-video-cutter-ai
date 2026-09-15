# ひとり切り抜き v8 — GitHub Actions自己ホスト版

目的は、iPhone Safariが unpkg 等からAI JavaScriptを直接読み込む問題を避けることです。

## 導入
1. ZIPの中身をリポジトリのルートへアップロードします（`.github` フォルダも必要）。
2. GitHubの **Actions** タブを開きます。
3. **Build self-hosted AI assets** を選び、**Run workflow** を押します。
4. 成功すると `vendor/tf.min.js` と `vendor/body-pix.min.js` がリポジトリにコミットされます。
5. Pagesが更新された後、サイトを再読み込みします。

## 重要
このv8はまず「AIライブラリをGitHub Pages自身から安定してロードできる」状態を確立する診断版です。
BodyPixのモデル重みは推論時に別途必要になるため、次段階でモデル重みも自己ホスト化します。
