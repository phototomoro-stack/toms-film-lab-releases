# Tom's Film Lab — Releases

Download builds of **Tom's Film Lab**, a macOS app for inverting and editing
scanned film negatives.

➡️ **[Download the latest release](../../releases/latest)**

## Install

1. Download the `.zip` from the latest release and unzip it.
2. Move `TomsFilmLab.app` to your `Applications` folder.
3. **First launch:** right-click the app → **Open** → confirm.

   These builds are ad-hoc signed but not notarized, so on first launch macOS
   Gatekeeper shows a warning. Right-click → Open bypasses it (you only need to
   do this once). Alternatively:
   ```sh
   xattr -dr com.apple.quarantine /Applications/TomsFilmLab.app
   ```

## Updates

The app checks this repository for new releases and offers to download them
from within Settings → アップデート.

---

Source code is maintained privately; this repository hosts release binaries only.
