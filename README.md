<div align="center">

# ⚡ Quick Launch

### The command palette your Android phone was missing.

**Spotlight for macOS. KRunner for KDE. Now, finally, one search bar to rule your whole phone.**

Type anything. Open apps, do math, convert units, search the web, find files, message a contact, flip your flashlight — all from one floating panel that appears over *any* app, on *any* screen, in under a second.

[![Android](https://img.shields.io/badge/Platform-Android%207.0%2B-3DDC84?logo=android&logoColor=white)](#requirements)
[![API](https://img.shields.io/badge/API-24--35-3DDC84)](#requirements)
[![Kotlin](https://img.shields.io/badge/Kotlin-2.0.21-7F52FF?logo=kotlin&logoColor=white)](#architecture)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)](#architecture)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
[![No Ads](https://img.shields.io/badge/Ads-none-success)](#privacy-first-by-design)
[![No Trackers](https://img.shields.io/badge/Trackers-none-success)](#privacy-first-by-design)
[![Internet Permission](https://img.shields.io/badge/INTERNET%20permission-not%20requested-success)](#privacy-first-by-design)

**[Download](#build-instructions) · [Features](#-why-youll-love-it) · [Screenshots](#-see-it-in-action) · [Setup](#-get-up-and-running-in-2-minutes) · [FAQ](#-faq)**

</div>

---

## 🤔 The problem

Your phone has 200 apps on it. Finding the one you want means unlocking, swiping through home screens, or digging through an app drawer. Need to do a quick calculation? Open a calculator app. Convert kilometers to miles? Open a browser, type a query, wait for ads to load. Want to flip on the flashlight? Swipe down, find the tile, tap it.

Every one of these is a *tiny* task that takes *too many* steps.

## ✨ The fix

**Quick Launch** puts a single, fast search bar on top of everything you do. Trigger it from almost anywhere — a floating bubble, a widget, a Quick Settings tile, a voice command, or even the same gesture that opens Google Assistant — type a few characters, and get exactly what you meant:

```
┌─────────────────────────────────────┐
│  🔍  Search apps, actions, web…  ✕  │
├─────────────────────────────────────┤
│  Apps                               │
│  📷  Camera                         │
│  🌐  Chrome                         │
│                                     │
│  Calculator                         │
│  =  (5 + 3) * 7                 56  │
│                                     │
│  🌐  Search web for "…"             │
└─────────────────────────────────────┘
```

Type it. Tap it. Gone. Back to what you were doing — now with the thing you needed.

---

## 🚀 Why you'll love it

| | |
|---|---|
| **⚡ Instant app search** | Fuzzy, typo-tolerant matching across every installed app — ranks by what you actually use, remembers your pins |
| **🧮 A real calculator, inline** | `(5+3)*7`, `25% of 80`, `10 % 3` — answered as you type, no separate app, no `eval()` hacks |
| **📐 Offline unit conversion** | `10 km to miles`, `5kg in lb`, `100 c to f` — length, mass, temperature, volume, time, storage, speed — zero network calls |
| **🌐 Web search, your engine** | Google, Bing, DuckDuckGo, or Brave — opens your actual browser, no in-app tracking |
| **📁 Find files by name** | Documents, photos, videos, music, archives, APKs — on-device MediaStore search, nothing leaves your phone |
| **🔦 Flashlight, by typing "torch"** | Because sometimes the fastest UI is just words |
| **👤 Contacts, one tap to call or text** | Optional and permission-gated — off until you turn it on |
| **⚙️ Jump straight to system settings** | `settings wifi`, `settings bluetooth` — skip the maze of menus |
| **📋 Smart clipboard suggestions** | Offers to copy or search whatever's on your clipboard, read only while the palette is open |
| **🕘 Recents & pins** | An empty search bar is never really empty — your last actions and favorite apps are right there |

### 🎯 Nine ways to summon it — use whichever fits your muscle memory

- **Assistant gesture** — set Quick Launch as your Android digital assistant and the *exact* gestures that open Google Assistant (long-press home, swipe from a bottom corner, long-press power) open Quick Launch instead. One-tap system dialog, no digging through menus.
- **Floating bubble** — an Assistive-Touch-style dot that follows you, snaps to the edge, survives a reboot.
- **Home-screen widget** — bolt icon for the palette, mic icon for voice search.
- **Voice search** — speak instead of type, works on any device, zero setup.
- **Share sheet** — share text or a link from any app straight into Quick Launch.
- **Quick Settings tile**, **persistent notification**, **launcher long-press shortcuts**, and an **in-app fallback** if you'd rather not grant the overlay permission at all.

---

## 🔐 Privacy-first, by design — not by policy

This isn't a privacy *policy* promise. It's a build-level guarantee:

- **No `INTERNET` permission in the manifest.** The app is *structurally incapable* of sending your data anywhere. The only "network" action is your device's browser opening a URL you explicitly chose.
- **No analytics. No ads. No trackers. No SDKs phoning home.**
- **Clipboard is read only while the palette is open and focused** — never in the background, per Android 10+'s own restrictions.
- **File search reads names only** — file contents are never opened, scanned, or logged.
- **Recents and pins live entirely in on-device storage.** Uninstall the app, and it's like it was never there.

If you've ever hesitated before granting a random launcher app "storage" and "contacts" and wondered where that data ends up — with Quick Launch, the honest answer is: nowhere. It can't. It doesn't have the permission to try.

---

## 🆚 How it compares

| | Quick Launch | Default launcher search | Web search apps |
|---|:---:|:---:|:---:|
| Works over *any* app, not just the home screen | ✅ | ❌ | ❌ |
| Inline calculator & unit conversion | ✅ | Sometimes | ❌ |
| Offline, no network required for core features | ✅ | ❌ | ❌ |
| No ads, ever | ✅ | Depends | ❌ |
| No `INTERNET` permission | ✅ | ❌ | ❌ |
| Assistant-gesture integration | ✅ | ❌ | ❌ |
| Open source | ✅ | ❌ | ❌ |

---

## 📱 See it in action

> Add your own screenshots or a short GIF here — a floating-palette demo sells this app faster than any paragraph can.

```
docs/
├── screenshot-palette.png
├── screenshot-settings.png
└── demo.gif
```

---

## 🛠 Get up and running in 2 minutes

1. **Install and open Quick Launch.**
2. Accept the one-tap **"Set as assistant?"** dialog (shown once) — this is the fastest way to get the Google-Assistant-style gesture trigger. Change it anytime in *Settings → Triggers*.
3. Tap **Open Quick Launch now** and grant **Display over other apps** so the palette can float above whatever you're doing.
4. Trigger it however you like: the assistant gesture, the floating bubble, the widget, voice search, the notification, the Quick Settings tile, or a launcher shortcut.
5. *(Optional)* Grant **Photos & files** access to unlock on-device file search.

That's it — no account, no sign-up, no onboarding survey.

---

## 🏗 Build it yourself

### Requirements

- **Android Studio** Koala (2024.1) or newer — or any IDE with JDK 17/21
- **JDK 17+** (the Gradle wrapper fetches Gradle 8.10.2 automatically)
- **Android SDK** platform 35 + build-tools 35
- An Android **7.0+ (API 24)** device or emulator

### Build instructions

```bash
# Clone it
git clone https://github.com/<your-username>/quick-launch.git
cd quick-launch

# Build a debug APK
./gradlew :app:assembleDebug
# → app/build/outputs/apk/debug/app-debug.apk

# Run the test suite (88 tests: ranking, calculator, conversion,
# command parsing, search engine, settings/view-model logic)
./gradlew :app:testDebugUnitTest

# Install straight to a connected device
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

Or in Android Studio: **File → Open…** → select the project folder → let it sync → **Run**.

---

## 🧩 Architecture

Built the way a modular launcher *should* be — every feature is a pluggable, independently testable search provider:

```
com.example.quicklaunch
├── overlay/     WindowManager-based floating panel, Compose UI in a service window
├── search/      SearchEngine — parallel providers, per-keystroke cancellation, ranking
├── providers/   apps · calculator · unit conversion · web · files · contacts ·
│                settings shortcuts · clipboard · flashlight
├── triggers/    9 independent entry points (bubble, widget, voice, assistant
│                gesture, share target, tile, notification, shortcuts)
├── data/        DataStore-backed settings & recents, corruption-safe by default
└── ui/          Material 3 (system/light/dark), compact mode, animation toggle
```

**Engineering highlights:**
- Hand-written recursive-descent expression parser — **no `eval()`, ever**
- Deterministic, unit-tested fuzzy-matching ranker
- Every coroutine scope guarded with a `CoroutineExceptionHandler`; DataStore reads self-heal from corruption
- App icon LRU cache, lazy package index invalidated only by install/uninstall broadcasts
- Every keystroke's search is cancelled before the next begins — stale results can never race ahead of fresh ones

Curious how it all fits together, or want to add your own provider? The codebase is small enough to read in an afternoon and modular enough to extend in an evening.

---

## 🔑 Permissions, in plain English

| Permission | What it's for | If you say no |
|---|---|---|
| `SYSTEM_ALERT_WINDOW` | Floats the palette over other apps | Palette still works inside the app itself |
| `POST_NOTIFICATIONS` | The optional persistent "Open Quick Launch" notification | That one trigger is disabled; everything else works |
| `RECORD_AUDIO` | Required by Android for any app registering as a digital assistant | Assistant-gesture trigger unavailable; every other trigger still works |
| `READ_CONTACTS` | Powers the optional contacts search/call/text provider | Contacts provider silently stays off |
| Media permissions (13+) / storage (≤12) | On-device file search by name | File search finds nothing beyond the app's own files |
| `RECEIVE_BOOT_COMPLETED` | Restores the floating bubble after a restart | Bubble comes back next time you open the app |

There is **no `INTERNET` permission** to opt out of, because it's never requested in the first place.

---

## ❓ FAQ

**Does this replace my launcher?**
No — Quick Launch layers on top of whatever launcher you already use. It doesn't touch your home screen.

**Will it slow my phone down?**
The palette is a lightweight overlay window that only exists while you're using it. No background service runs when it's closed (aside from an optional bubble/notification you can turn off).

**Does it need an internet connection?**
Only if you tap a web-search result, which opens your browser. Every other feature — calculator, conversions, app search, file search, contacts, settings shortcuts — works fully offline.

**Is my data safe?**
It never leaves your device — there's no permission in the app that would even let it.

**Can I contribute?**
Yes, please. See [Contributing](#-contributing) below.

---

## 🤝 Contributing

Pull requests are welcome — new search providers, ranking improvements, translations, bug fixes. Please open an issue first for anything larger than a small fix, so we can talk through the approach together.

## 📄 License

MIT — see [`LICENSE`](LICENSE) for the full text. Use it, fork it, ship your own version.

---

<div align="center">

**If Quick Launch saves you a few seconds a day, give it a ⭐ — it helps other people find it too.**

</div>
