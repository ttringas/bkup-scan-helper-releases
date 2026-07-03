# BKUP Scan Helper — Downloads

Public distribution point for **BKUP Scan Helper**, the macOS menu-bar utility that
routes QR-scanner input to the BK UP staff web app when the browser isn't focused.

The source code lives in a private repo. This repo holds only the release builds so
they can be downloaded on a workstation without a GitHub login.

## Install on a workstation

1. **[Download the latest version](https://github.com/ttringas/bkup-scan-helper-releases/releases/latest/download/BKUP-Scan-Helper.dmg)**
2. Open the downloaded `BKUP-Scan-Helper.dmg`.
3. Drag **BKUP Scan Helper** onto the **Applications** folder, then eject the disk image.
4. Open your **Applications** folder and double-click **BKUP Scan Helper**.
5. **First launch only:** macOS will say the app is from an unidentified developer.
   Click **Done**, then open **System Settings → Privacy & Security**, scroll to the
   bottom, and click **Open Anyway** next to "BKUP Scan Helper". Confirm with Touch ID
   or your password. (This app is unsigned on purpose — it only runs on BK UP's own
   machines. You only do this once per computer; after that it opens normally.)
6. When macOS asks, grant **Accessibility** permission (System Settings opens to the
   right place — flip the switch on).
7. Click the menu-bar icon (a QR square) and turn on **Launch at Login**.

That's it. Keep the front-desk Chrome window on the BK UP staff app, and scans will
route to it even when another app is in front.

## Updating

Download the latest DMG again and drag the new copy over the old one in Applications.
The one-time approval and Accessibility permission carry over — no need to redo them.
