# Tom's Film Lab — リリース / Releases

**Tom's Film Lab** は、スキャンしたフィルムネガを反転・編集するための macOS アプリです。
このリポジトリは配布用のビルド（バイナリ）を置く場所で、ソースコードは非公開で管理しています。

➡️ **[最新版をダウンロード（Download latest）](../../releases/latest)**

## インストール

1. 最新リリースから `.zip` をダウンロードして解凍します。
2. `TomsFilmLab.app` を「アプリケーション」フォルダへ移動します。
3. 下記「初回起動の許可」に従って、初回だけ実行を許可します。

## 初回起動の許可（重要）

このビルドは公証（notarization）されていないため、初回起動時に macOS の
Gatekeeper がブロックします。**一度だけ**次の操作で許可してください。

### 最新の macOS（Sequoia / 15 以降）

1. `TomsFilmLab.app` をダブルクリックする（「開けません」と表示されてOK）。
2. **システム設定 → プライバシーとセキュリティ** を開く。
3. 画面下の方に出る「**"TomsFilmLab" は…ブロックされました**」の欄の
   「**このまま開く**（Open Anyway）」ボタンを押す。
4. もう一度アプリを開き、確認ダイアログで「開く」を押す。

### それ以前の macOS

- `TomsFilmLab.app` を**右クリック →「開く」**→ 確認ダイアログで「開く」。

### うまくいかない場合（共通）

ターミナルで隔離属性を外すと確実に開けます：

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

**Install:** download the `.zip` from the [latest release](../../releases/latest) and
move `TomsFilmLab.app` to `Applications`. These builds are ad-hoc signed but **not
notarized**, so first launch needs a one-time approval:

- **macOS Sequoia (15)+**: double-click (it will be blocked) → **System Settings →
  Privacy & Security** → click **"Open Anyway"** for TomsFilmLab → open again and confirm.
- **Older macOS**: **right-click → Open**.
- Or clear quarantine: `xattr -dr com.apple.quarantine /Applications/TomsFilmLab.app`

The app checks this repo for updates from Settings → アップデート.
