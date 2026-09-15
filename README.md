# ひとり切り抜き v7

GitHub Pages向け。まず同梱 vendor/ を読み、無い場合のみCDNへフォールバックする構成です。

注意: この実行環境では外部npm/CDNからTensorFlow.js/BodyPix本体とモデル重みを取得できなかったため、vendorファイルは同梱できていません。完全オフライン版にはそれらの取得が必要です。
