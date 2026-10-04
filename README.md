# nyan Real サポート

nyan Real製品の公式サポートサイトです。

- [サポートトップ](https://support.nyanreal.jp/)
- [Spatial Wall](https://support.nyanreal.jp/spatial-wall/)
- [Media Player](https://support.nyanreal.jp/media-player/)
- [Virtual Display Driver](https://support.nyanreal.jp/vdd/)
- [VR Bridge](https://support.nyanreal.jp/vr-bridge/)（開発中）
- [Key Studio](https://support.nyanreal.jp/key-studio/)（ブラウザー用設定ツール）

## VR Bridge

**nyan Real / VR Bridge** は、対応メガネをSteamVR用のヘッドセットとして使うWindows向けソフトウェアです。現在開発中で、無料の試験版を準備しています。

- [日本語の製品情報](https://support.nyanreal.jp/vr-bridge/)
- [English product information](https://support.nyanreal.jp/vr-bridge/en/)

ダウンロード、導入手順、利用条件、問い合わせ窓口は試験版の公開時に案内します。

## Spatial Wall

- [日本語マニュアル](https://support.nyanreal.jp/spatial-wall/manual/ja/)
- [English manual](https://support.nyanreal.jp/spatial-wall/manual/en/)
- [不具合・問い合わせ](https://github.com/8796n/nyan-real-support/issues/new?template=spatial-wall.yml)

問い合わせの前に、アプリの「バージョン情報」→「問い合わせ用情報をコピー」を実行し、結果をフォームへ編集せず貼り付けてください。

このリポジトリはサポート資料を公開するためのもので、製品本体のソースコードは含みません。Spatial Wallは有償のクローズドソースソフトウェアです。使用条件は[使用許諾契約書（日本語・正文）](spatial-wall/legal/EULA.ja.txt)および[英語版](spatial-wall/legal/EULA.en.txt)を参照してください。

## ページの編集

マニュアル（`spatial-wall/manual/`）と法務文書（`spatial-wall/legal/`）以外のページは生成物です。
直接編集せず、`src/pages/`の本文を直してから`python tools/build_pages.py`を実行し、
生成されたHTMLも一緒にコミットします。ヘッダー・ナビ・フッターは`src/layout.html`、
製品の並びとトップの製品カードは`src/products.json`が正本です。CSSのキャッシュ版数は自動で更新されます。

製品を追加するときは、`src/products.json`へ1件足し、既存製品をまねて
`src/pages/<key>/index.html`と`src/pages/<key>/en/index.html`を作ります。

## English

This repository hosts the official support site for nyan Real products. It contains support material, not the product source code.

**nyan Real / VR Bridge** is Windows software for using supported glasses as a SteamVR headset. It is currently in development, with a free test release being prepared. See the [English product page](https://support.nyanreal.jp/vr-bridge/en/) for its scope and limitations.

Before opening a Spatial Wall issue, choose About → Copy support information and paste the unchanged block into the [support form](https://github.com/8796n/nyan-real-support/issues/new?template=spatial-wall.yml). Spatial Wall is paid, closed-source software; see the [English EULA](spatial-wall/legal/EULA.en.txt) and the authoritative [Japanese EULA](spatial-wall/legal/EULA.ja.txt).
