# TalkTime

A free, anonymous social + private messaging app for Android. No account, no
sign‑up, no email — you just open it and go.

## Features

- **Free & no account** — no signup, no email, no phone number.
- **Anonymous** — you get a random username (change it if you like); your posts
  don't reveal who you are.
- **Encrypted** — the app and the server negotiate a fresh key each session
  (ECDH); no secret key is stored inside the app.
- **Posts** — share text over colorful backgrounds; **like** and **reply** to
  posts. Browse **Latest**, **Local** (near you), or by **#tag**.
- **Private messages (DMs)** — one‑to‑one chats with **images** and **short
  videos (up to 10 seconds)**, plus **read receipts**.
- **Find people nearby** — opt‑in location to discover other TalkTime users near
  you and start a chat.
- **Safety** — **block**, **report**, and **delete chat** from the ⋮ menu.
- **Optional app lock** — set a PIN (Me → App lock) to lock the app on your phone.
- **Fair posting** — post as much as you want, with a 30‑minute gap between posts.
  Posts age out of the app after about a month.

## Download

**`TalkTime.apk`** (in this repo)

- Size: **4.21 MB**
- SHA‑256: `f7207c405e25f10a40e9be17c03e08e6c2dab630a164d62c12fa078b929c538d`

Verify the download (optional):
```
# Android (Termux) or any Linux/macOS
sha256sum TalkTime.apk
# Windows PowerShell
Get-FileHash TalkTime.apk -Algorithm SHA256
```

## Install (Android)

1. **Download** `TalkTime.apk` onto your Android phone.
2. Open it (Files app or your browser's Downloads). Android will ask to allow
   installs from this source:
   - Tap **Settings** on the prompt → enable **Allow from this source**
     (a.k.a. *Install unknown apps*), then go back and tap **Install**.
   - Or set it ahead of time: **Settings → Apps → Special access →
     Install unknown apps** → pick your browser/Files → **Allow**.
3. Tap **Install**, then **Open**.

> This is a **debug build** (not from the Play Store), so Android shows the
> "unknown app" warning — that's expected for sideloaded apps.

## Requirements

- Android 7.0+ (roughly — modern Android WebView).
- **Internet connection.** TalkTime talks to a small server that the host runs.
  As long as that server is online, the app works from **any Wi‑Fi or mobile
  data, anywhere** — the phone does **not** need to be on the same network.

## Server address

TalkTime ships pointing at its server. If the host tells you the address has
changed, update it in‑app: **Me → Server address**, paste the new URL, **Save**
(the app reloads). No reinstall needed.

## Privacy & safety notes

- Posts are anonymous to other users, but the **server can read content** (it's
  not end‑to‑end). Encryption protects your traffic from the network in between.
- All content lives on the host's server, not on public cloud storage.
- Report abuse with the **Report** option in any chat — it's sent to the server.

## Version

- TalkTime debug build — see commit history for changes.
