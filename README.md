# BKUP Scan Helper — Downloads

Public distribution point for **BKUP Scan Helper**, the macOS menu-bar utility that
routes QR-scanner input to the BK UP staff web app when the browser isn't focused.

The source code lives in a private repo. This repo holds only the release builds so
they can be downloaded on a workstation without a GitHub login.

## Install on a workstation

These builds are unsigned (they only run on BK UP's own machines), so macOS quarantines
the download and will say the app "is damaged" until you clear that flag once.

1. **[Download the latest version](https://github.com/ttringas/bkup-scan-helper-releases/releases/latest/download/BKUP-Scan-Helper.dmg)**
2. Open the downloaded `BKUP-Scan-Helper.dmg` and drag **BKUP Scan Helper** onto the **Applications** folder. Eject the disk image.
3. Open the **Terminal** app (Spotlight → type "Terminal"), paste this line exactly, and press Return:
   ```sh
   xattr -cr "/Applications/BKUP Scan Helper.app"
   ```
4. Open your **Applications** folder and double-click **BKUP Scan Helper**. It opens normally now.
5. When macOS asks, grant **Accessibility** permission (System Settings opens to the right place — flip the switch on).
6. Click the menu-bar icon (a QR square) and turn on **Launch at Login**.

Keep the front-desk Chrome window on the BK UP staff app, and scans will route to it
even when another app is in front.

## Updating

Download the latest DMG, drag the new copy over the old one in Applications, and run the
same `xattr -cr` line again. The Accessibility permission carries over.
