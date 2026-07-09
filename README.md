# Tom's Film Lab — リリース / Releases

**Tom's Film Lab** は、スキャンしたフィルムネガを反転・編集するための macOS アプリです。
このリポジトリは配布用のビルド（バイナリ）を置く場所で、ソースコードは非公開で管理しています。

➡️ **[最新版をダウンロード（Download latest）](../../releases/latest)**

## インストール

1. 最新リリースから `.zip` をダウンロードして解凍します。
2. `TomsFilmLab.app` を「アプリケーション」フォルダへ移動します。
3. **初回のみ**：アプリを右クリック →「**開く**」→ 確認ダイアログで「開く」。

   このビルドは公証（notarization）されていないため、初回起動時に macOS の
   Gatekeeper が「開けません」という警告を出します。上記の「右クリック →『開く』」で
   回避できます（**一度だけ**でOK）。うまくいかない場合は次のコマンドでも解除できます：

   ```sh
   xattr -dr com.apple.quarantine /Applications/TomsFilmLab.app
   ```

## アップデート

アプリは起動時にこのリポジトリの新しいリリースを自動で確認します
（設定 → **アップデート** →「今すぐ確認」でも手動確認できます）。
新しいバージョンがあれば通知され、その場でダウンロードできます。

---

## English (summary)

**Tom's Film Lab** is a macOS app for inverting and editing scanned film negatives.
This repo hosts release binaries only; the source is kept private.

**Install:** download the `.zip` from the [latest release](../../releases/latest),
move `TomsFilmLab.app` to `Applications`, then **right-click → Open** on first launch
(these builds are ad-hoc signed but not notarized). The app checks this repo for
updates from Settings → アップデート.
