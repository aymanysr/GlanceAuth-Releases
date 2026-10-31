# GlanceAuth

**GlanceAuth** unlocks and authenticates your Mac using your iPhone's Face ID with end-to-end Secure Enclave encryption, smart clamshell routing, and proximity auto-lock.

<p align="center">
  <a href="https://github.com/aymanysr/GlanceAuth-Releases/releases/latest/download/GlanceAuth-0.1.0.dmg">
    <img src="https://img.shields.io/badge/Download_for_macOS-DMG-black?style=for-the-badge&logo=apple" alt="Download macOS DMG">
  </a>
  &nbsp;
  <a href="https://github.com/aymanysr/GlanceAuth-Releases/releases/latest/download/GlanceAuth-0.1.0.ipa">
    <img src="https://img.shields.io/badge/Download_for_iOS-IPA-blue?style=for-the-badge&logo=apple" alt="Download iOS IPA">
  </a>
  &nbsp;
  <a href="https://github.com/aymanysr/GlanceAuth-Releases/releases">
    <img src="https://img.shields.io/badge/Latest_Release-v0.1.0-green?style=for-the-badge" alt="Latest Release">
  </a>
</p>

---

## Previews

<p align="center">
  <img src="assets/settings_window.png" width="48%" alt="GlanceAuth Mac Settings">
  &nbsp;
  <img src="assets/companion_screen.png" width="45%" alt="GlanceAuth iOS Companion">
</p>

---

## Key Features

- **iPhone Face ID for macOS**: Approve `sudo`, screensaver unlock, and authentication dialogs instantly from your phone.
- **Smart Clamshell Routing**: Automatically detects MacBook lid state — routes challenges to iPhone Face ID when closed or docked with external monitors, and uses Mac Touch ID when open.
- **Proximity Auto-Lock**: Measures Bluetooth Low Energy (BLE) signal strength and automatically locks your Mac within 30 seconds when you carry your iPhone away.
- **Dual Transport Failover**: Seamless transition between Bluetooth Low Energy (BLE) and Local Network Wi-Fi without dropped sessions.
- **Hardware-Grade Security**: P-256 ECC keys generated inside your iPhone's Secure Enclave. Private keys never leave your phone.

---

## Installation & Setup Guide (5 Minutes)

### Step 1: Install on Your Mac

1. Download **[GlanceAuth-0.1.0.dmg](https://github.com/aymanysr/GlanceAuth-Releases/releases/latest/download/GlanceAuth-0.1.0.dmg)**.
2. Open the `.dmg` and drag **`GlanceAuth.app`** into your **`Applications`** folder.
3. Double-click **`GlanceAuth-0.1.0.pkg`** inside the DMG to install the background service.
4. **First Launch (One-Time Gatekeeper Approval)**:
   - Because this is a private beta build without an Apple commercial certificate:
   - **Right-click `GlanceAuth.app` in Applications → click "Open" → click "Open"** in the popup.
   - GlanceAuth will appear in your top menu bar.

---

### Step 2: Install on Your iPhone (2 Minutes from Home)

You do **not** need a jailbroken iPhone. You can install the companion app in 2 minutes using a free desktop utility called **Sideloadly**:

1. **Download Sideloadly on Your Mac**:
   - Download the free Mac app from [https://sideloadly.io](https://sideloadly.io) and open it.
2. **Connect iPhone via USB**:
   - Plug your iPhone into your Mac (tap **"Trust This Computer"** on your iPhone if prompted).
3. **Transfer GlanceAuth to Your iPhone**:
   - Download **[GlanceAuth-0.1.0.ipa](https://github.com/aymanysr/GlanceAuth-Releases/releases/latest/download/GlanceAuth-0.1.0.ipa)**.
   - In Sideloadly, your iPhone will appear under **"iDevice"**.
   - Drag **`GlanceAuth-0.1.0.ipa`** into the large app icon box in Sideloadly.
   - Enter your personal Apple ID email in the **"Apple ID"** box (used only to sign the free developer certificate locally).
   - Click **"Start"**. GlanceAuth will install directly onto your iPhone home screen!
4. **One-Time Trust on iPhone**:
   - Open iPhone **Settings → General → VPN & Device Management**.
   - Under **Developer App**, tap your Apple ID and tap **Trust**.
   - Open **GlanceAuth** from your iPhone home screen!

```
 ┌────────────────────────────────────────────────────────┐
 │                      Sideloadly                        │
 │                                                        │
 │  iDevice: [ Your iPhone (USB)                    ▼ ]   │
 │                                                        │
 │  ┌──────────────────────────────────────────────────┐  │
 │  │      [  GlanceAuth-0.1.0.ipa  ]                  │  │
 │  │        (Drag & Drop IPA Here)                    │  │
 │  └──────────────────────────────────────────────────┘  │
 │                                                        │
 │  Apple ID: [ your-email@icloud.com                ]    │
 │                                                        │
 │                    [ ▶ START ]                         │
 └────────────────────────────────────────────────────────┘
```

---

### Step 3: Wireless QR Pairing

Now you can disconnect the USB cable — it is never needed again!

1. On your iPhone: In **Settings → GlanceAuth**, ensure **Bluetooth**, **Face ID**, and **Background App Refresh** are all **ON**.
2. On your Mac: Click the GlanceAuth menu bar icon and select **"Re-pair Phone / Show QR..."**.
3. On your iPhone: Open GlanceAuth and tap **"Scan QR Code"**.
4. Point the camera at the Mac screen. Once verified, the menu bar indicator turns **Green: "Ready — phone connected"**!

---

## How Updates Work

When a new version is released:
1. Download the new `.dmg` and `.ipa` from the [Releases page](https://github.com/aymanysr/GlanceAuth-Releases/releases).
2. On Mac: Replace `GlanceAuth.app` in `/Applications`.
3. On iPhone: Drop the new `.ipa` into Sideloadly and click **Start**.
4. **Your pairing is preserved**: iOS performs an in-place update. You do **not** need to re-scan the QR code or configure settings again!

---

## The 7-Day Free Certificate & Wi-Fi Auto-Refresh

Apple places a 7-day expiration on apps signed with free personal Apple IDs:
- **Automatic Wi-Fi Refresh**: Sideloadly includes an automatic background renewal feature. Leave Sideloadly running on your Mac while your phone and Mac are on the same home Wi-Fi network, and it will silently renew the certificate over the air before it expires.
- **Manual Reset**: Installing any update also resets the 7-day clock back to full.

---

## Bug Reports & Feedback

If you encounter any issues or have feature requests, please open an issue on the [GitHub Issues](https://github.com/aymanysr/GlanceAuth-Releases/issues) tab!

---

## License

GlanceAuth is closed-source freeware. All rights reserved. Third-party open-source notices are bundled in the distribution.
