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
6. The **first time you scan**, macOS asks to let the app **control Google Chrome** — click **OK/Allow**. (This is how it switches Chrome to the staff-app tab.)
7. Click the menu-bar icon (a QR square) and turn on **Launch at Login**.

Keep a Chrome tab open on the BK UP staff app (`app.bkup.nyc`). When you scan while
another app or another tab is in front, the helper brings Chrome forward, switches to
the staff-app tab, and delivers the scan there.

## Updating

1. **Quit the running app first** — click the menu-bar QR icon and choose *Quit BKUP Scan Helper*. Dragging a new copy into Applications does **not** replace the copy already running in memory; this is the #1 reason an update seems to "not work".
2. Download the latest DMG and drag the new app over the old one in Applications.
3. In Terminal run `xattr -cr "/Applications/BKUP Scan Helper.app"` again.
4. Open it. Accessibility carries over; on the first scan re-approve the "control Chrome" prompt if asked. (The app is unsigned, so an update looks like a new app to macOS.)

**Verify which build is running:** click the menu-bar icon — the bottom of the menu shows *Version x.y.z*. It should read the version you just installed.
