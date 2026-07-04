# BKUP Scan Helper — Downloads

Public distribution point for **BKUP Scan Helper**, the macOS menu-bar utility that
routes QR-scanner input to the BK UP staff web app when the browser isn't focused.

The source code lives in a private repo. This repo holds the signed, notarized release
builds and the Sparkle auto-update feed.

## Install on a workstation (one time)

1. **[Download the latest version](https://github.com/ttringas/bkup-scan-helper-releases/releases/latest/download/BKUP-Scan-Helper.dmg)**
2. Open the downloaded `BKUP-Scan-Helper.dmg`.
3. Drag **BKUP Scan Helper** onto the **Applications** folder, then eject the disk image.
4. Open your **Applications** folder and double-click **BKUP Scan Helper**. It opens
   with no warning (the app is signed and notarized by Apple).
5. When macOS asks, grant **Accessibility** permission (the switch it points you to).
6. On the first scan, click **OK** when macOS asks to let it **control Google Chrome**
   (that's how it switches to the right staff tab).
7. Click the menu-bar icon (the BK UP mark) and turn on **Launch at Login**.

That's the whole setup — no Terminal, no security overrides.

## Updates are automatic

The app checks for updates in the background and installs them itself. You do **not**
need to re-download or reinstall when a new version ships — workstations update on their
own within an hour. (You can force a check anytime from the menu bar → **Check for
Updates…**, and the menu's **Version** line shows what's installed.)

Keep a Chrome tab on the BK UP staff app (`app.bkup.nyc/staff`) and scans will route to
it even when another app or tab is in front.
