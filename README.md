# Odin Privacy Policy

**Effective date:** September 2, 2026
**Applies to:** Odin for iOS, iPadOS, tvOS, and macOS, published by Orbital Builds ("we", "us").

Odin is a video player for media you already own. It connects to servers you control and plays the files stored there. This policy describes exactly what information the app handles, where it is stored, and which outside services the app contacts. It is written to be read, not skimmed, and it is complete.

---

## 1. Summary

- We do not collect personal data. Odin has no accounts, no sign-up, no analytics, no advertising, no crash reporting of our own, and no servers operated by us.
- Everything the app stores lives on your device, under your control, and is deleted when you delete the app.
- The app contacts third-party services only to do what you ask it to do: play files from your server, look up titles and artwork, and, if you opt in, sync your watch progress to your own Trakt or AniList account.
- We never sell, share, or receive your data, because we never have it.

---

## 2. Information stored on your device

Odin keeps the following on the device it is installed on. None of it is transmitted to us.

| Data | Purpose | Where it is kept |
|---|---|---|
| Media server address, username, and password | To connect to your WebDAV or Jellyfin server | Device Keychain (encrypted by the operating system) |
| Trakt and AniList access tokens, if you sign in | To sync watch progress to your account | Device Keychain |
| Library index, playback positions, watch history, watchlist, Continue Watching | App functionality | App's private storage |
| Profiles, profile names, avatars, and optional profile PINs | Multiple viewers on one device | App's private storage; PINs in the Keychain |
| Settings and preferences | App functionality | App's private storage |
| Cached artwork, thumbnails, and metadata | Faster loading, offline browsing | App's cache, cleared by the system or by you |

You can remove any of this by removing the server or account inside the app, or all of it by deleting the app. On tvOS the app also writes a small Continue Watching list to a shared container so the Top Shelf on the Home screen can display it; this stays on the Apple TV.

---

## 3. Your media servers

Odin connects only to the WebDAV or Jellyfin servers you add, using the address and credentials you enter. Requests go directly from your device to your server. We have no access to your servers, no knowledge of their addresses, and no visibility into their contents.

Depending on your settings, the app may send your Jellyfin server playback progress and watched state so that the server can keep your library in sync across Jellyfin clients. This is a feature of your own server, not of us.

---

## 4. Third-party services the app contacts

The app makes network requests to the services below. Each request contains only what is needed for the feature named. No request contains your name, email, device identifiers, or advertising identifiers. Each provider's own privacy policy governs what it receives.

### Metadata and artwork

To show titles, descriptions, posters, episode lists, and trailers for items in your library, Odin sends the title or public catalog identifier of the item to:

- **The Movie Database (TMDB)** — themoviedb.org
- **TheTVDB** — thetvdb.com
- **AniList** — anilist.co
- **MyAnimeList** (read-only, no account) — myanimelist.net
- **Jikan** (unofficial MyAnimeList API) — jikan.moe
- **Kitsu** — kitsu.io
- **ani.zip** — anime episode artwork supplement

Two community-maintained identifier mapping files, used to translate between these catalogs, are downloaded from GitHub (raw.githubusercontent.com).

Trailers listed by TMDB are loaded from **YouTube** or, where TMDB links there, **Vimeo**. Loading a trailer is subject to those services' policies, including their cookies.

If you enable "Prefer Local Metadata" for a Jellyfin server, titles and artwork come from your server instead, and fewer or no requests are made to the public services above.

### Optional account sync

If you choose to sign in to **Trakt** or **AniList**, the app sends your playback progress and watched state to that account so your history is recorded there. Sign-in happens on the provider's own web page; the app receives only an access token, stored in the Keychain. This feature is off until you sign in and can be disconnected at any time in Settings, which deletes the token from the device.

### Apple services

If iCloud is enabled on your device, Odin uses Apple's iCloud key-value store to sync your own anime episode-mapping overrides between your devices. That data is stored in your iCloud account under Apple's privacy terms, not with us. Odin does not use any other Apple service that transmits data on your behalf.

---

## 5. Direct video links

The Search field accepts a complete video URL that you paste. The app fetches that address only to play it. Odin never suggests, lists, indexes, or links to any URL; the app ships with no content and no directory of content.

---

## 6. What we do not do

- We do not collect analytics, usage statistics, or telemetry.
- We do not show advertising or use advertising identifiers.
- We do not use tracking, fingerprinting, or cross-app identifiers as defined by Apple's App Tracking Transparency framework.
- We do not sell, rent, or share personal information with anyone.
- We do not receive crash reports except those you choose to share with Apple through the system's own crash-reporting settings, which Apple anonymizes before making them available to developers.

---

## 7. Data retention and deletion

Because nothing is stored with us, there is nothing for us to retain or delete. All app data is on your device and in the accounts you own (your media server, your Trakt or AniList account, your iCloud). Deleting the app removes all local data. Tokens for connected accounts are removed when you disconnect the account in Settings, and you can additionally revoke Odin's access from your Trakt or AniList account settings.

---

## 8. Security

Credentials and tokens are stored in the operating system's Keychain, which encrypts them at rest and restricts access to the app. Connections to metadata services and to Trakt and AniList use HTTPS. Connections to your own media server use whatever protocol you configured; we recommend HTTPS for servers reachable over the internet.

---

## 9. Children

Odin is not directed at children and does not knowingly collect information from anyone, including children under 13 (or the applicable age in your region). The app contains no content of its own; what appears in the app is what you have placed on your own server.

---

## 10. Your rights

Users in the European Economic Area, the United Kingdom, California, and other regions have rights over personal data held by companies, including access, correction, deletion, and portability. Since we hold no personal data about you, there is nothing for us to provide, correct, or erase; your data is entirely in your possession. If you believe otherwise, contact us and we will respond.

---

## 11. Changes to this policy

If the app's behavior changes in a way that affects this policy, we will update this page and change the effective date at the top.

---

## 12. Contact

Orbital Builds
Email: **orbitalbuilds@gmail.com**
