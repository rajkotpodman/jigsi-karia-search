# Jigsi Karia — Cyber OSINT Gateway & Hacker Scanner

<p align="center">
  <img src="https://img.shields.io/badge/version-5.0.0-00ff00?style=for-the-badge&logo=github" alt="Version" />
  <img src="https://img.shields.io/badge/tools-900+-ff0055?style=for-the-badge&logo=search" alt="Tools" />
  <img src="https://img.shields.io/badge/categories-30-00bcff?style=for-the-badge" alt="Categories" />
  <img src="https://img.shields.io/badge/platform-web_|_android_|_pwa-black?style=for-the-badge&logo=android" alt="Platform" />
  <img src="https://img.shields.io/badge/size-213_KB-00ff00?style=for-the-badge" alt="Size" />
  <img src="https://img.shields.io/badge/license-educational_only-ff4444?style=for-the-badge" alt="License" />
</p>

<p align="center">
  <b>Zero-dependency | Single-file | PWA + Native Android | Gujarati UI</b>
</p>

A professional-grade cyber intelligence dashboard aggregating 900+ search engines, OSINT tools, exploit databases, API fetchers, dark web scanners, tire/vehicle lookups, and AI-powered intelligence modules — available as a single-file web app, a PWA, and a native Android APK.

---

## Table of Contents

- [Overview](#overview)
- [Features Matrix](#features-matrix)
- [Platform Availability](#platform-availability)
- [Quick Start](#quick-start)
- [Category Index](#category-index)
- [AI Intelligence Fetcher](#ai-intelligence-fetcher)
- [Android Application](#android-application)
  - [Installation](#android-installation)
  - [Project Structure](#android-project-structure)
  - [Build from Source](#android-build-from-source)
  - [JavaScript Bridge API](#android-javascript-bridge-api)
  - [Key Files](#android-key-files)
- [Web Deployment](#web-deployment)
- [Repository Structure](#repository-structure)
- [Architecture & Data Flow](#architecture--data-flow)
- [Technical Specifications](#technical-specifications)
- [Color System](#color-system)
- [Authentication](#authentication)
- [Security Notice](#security-notice)
- [Contributing / Build Guide](#contributing--build-guide)
- [Contact & Links](#contact--links)

---

## Overview

Jigsi Karia (Gujarati: જિજ્ઞાસુ કારિયા) is an all-in-one cyber investigation portal built as a single HTML file with zero external dependencies. Every tool, API endpoint, and search engine is mapped to a URL template. Enter a query like a phone number, IP address, domain, email, username, or vehicle VIN — then launch it across any of the 900+ pre-configured services with one click.

**What makes it unique:**
- Entire application in **one file** — no build step, no bundler, no npm
- **900+ URL templates** covering search engines, OSINT tools, blockchain explorers, tire catalogs, vehicle databases, and more
- **11 AI Fetch modules** that launch multiple intelligence tabs simultaneously
- **Native Android APK** with full WebView integration, JavaScript bridge, and offline support
- **PWA installable** with service worker caching
- **Matrix digital rain** canvas background with dark/light mode toggle
- **Gujarati-language UI** for the primary audience with English mixed labels

---

## Features Matrix

| Feature | Web | PWA | Android APK |
|---------|:---:|:---:|:-----------:|
| Matrix Canvas Animation | ✅ | ✅ | ✅ |
| 900+ Search Engine Launchers | ✅ | ✅ | ✅ |
| AI Fetch Intelligence Panel (12 modules) | ✅ | ✅ | ✅ |
| Dark/Light Mode Toggle | ✅ | ✅ | ✅ |
| Smart Autocomplete (30 keywords) | ✅ | ✅ | ✅ |
| Search History (MRU 10) | ✅ | ✅ | ✅ |
| Clipboard Copy | ✅ | ✅ | ✅ |
| Category Quick-Jump Toolbar | ✅ | ✅ | ✅ |
| Stats Counter Dashboard | ✅ | ✅ | ✅ |
| WhatsApp Floating Button | ✅ | ✅ | ✅ |
| Pro Action Hub (Buy/Donate/Store) | ✅ | ✅ | ✅ |
| Offline Caching | ✅ | ✅ | ✅ |
| Install to Home Screen | ❌ | ✅ | ✅ |
| Native Splash Screen | ❌ | ❌ | ✅ |
| Fullscreen Immersive Mode | ❌ | ❌ | ✅ |
| External App Launching | ❌ | ❌ | ✅ |
| JavaScript Bridge (Android API) | ❌ | ❌ | ✅ |
| Back Button Navigation | ❌ | ❌ | ✅ |
| Share Intent | ❌ | ❌ | ✅ |
| Toast Notifications | ✅ | ✅ | ✅ |

---

## Platform Availability

| Platform | Type | File | Size |
|----------|------|------|:----:|
| **Web** | Single HTML file | `index.html` | 213 KB |
| **PWA** | Progressive Web App | `index.html` + `manifest.json` + `sw.js` | 214 KB |
| **Android** | Native APK (signed) | `jigsi-karia-v5.apk` | 4.6 MB |
| **Android** | Android Studio project | `android/` directory | source only |

---

## Quick Start

### Web / PWA

```bash
# Clone the repository
git clone https://github.com/rajkotpodman/jigsi-karia-search.git
cd jigsi-karia-search

# Start local server (Python 3)
python3 -m http.server 8080 --bind 0.0.0.0

# Or with Node.js
npx serve .
```

Open `http://localhost:8080` in your browser.  
**Default credentials:** `admin` / `admin`

### Android APK

Download `jigsi-karia-v5.apk` from the repository root and install directly on any Android device (5.0+).
Or build from source (see [Build from Source](#android-build-from-source)).

---

## Category Index

| # | Category | Buttons | Key Tools |
|:--:|----------|:-------:|-----------|
| 1 | Mega Search Engines | 56 | Google, Bing, Yandex, Baidu, DuckDuckGo, Brave AI, SearX |
| 2 | OSINT & Intelligence | 96 | Shodan, IntelX, Maltego, HaveIBeenPwned, Censys, ZoomEye |
| 3 | Network & Domain Tools | 55 | DNSDumpster, MXToolBox, BGPView, SecurityTrails, ViewDNS |
| 4 | Exploit & Vulnerability DB | 47 | Exploit-DB, NVD, CVE Details, Metasploit, VulHub, GTFOBins |
| 5 | Threat Intelligence & Malware | 38 | VirusTotal, MalwareBazaar, MISP, YARA, CrowdStrike, ThreatFox |
| 6 | Social & People Search | 48 | Pipl, Spokeo, WhatsMyName, UserSearch, LinkedIn, TrueCaller |
| 7 | Advanced AI Suites | 30 | ChatGPT, Claude, Gemini, DeepSeek, Hugging Face, Ollama |
| 8 | Cryptocurrency & Blockchain | 30 | Blockchair, Etherscan, DeBank, CoinGecko, Glassnode, Messari |
| 9 | Dark Web & TOR | 23 | Ahmia, DarkSearch, Tor Project, OnionShare, I2P, Freenet |
| 10 | Cloud & DevOps OSINT | 28 | AWS, Azure, GCP, Kubernetes, Docker Hub, Vercel, Supabase |
| 11 | Forensic & Data Leak | 36 | Autopsy, Volatility, BreachDirectory, DeHashed, Cellebrite |
| 12 | Misc Hacker Tools | 47 | CyberChef, Hash Killer, JWT.io, Regex101, CodePen, CodeBeautify |
| 13 | Cyber Security News | 20 | Krebs, TheHackerNews, BleepingComputer, SANS, DarkReading |
| 14 | Pentest, CTF & Lab | 25 | HackTheBox, TryHackMe, HackerOne, Bugcrowd, PentesterLab |
| 15 | Sandbox & File Analysis | 20 | Cuckoo, CAPE, Joe Sandbox, Intezer, Triage, FileScan.io |
| 16 | Privacy, VPN & Anonymity | 20 | NordVPN, Mullvad, ProtonVPN, PrivacyTools, Tails OS, Whonix |
| 17 | Email Intel & Spam Check | 19 | MXToolBox, EmailRep, Mail-Tester, NeverBounce, ZeroBounce |
| 18 | Geo, Map & Location | 20 | Google Maps, OpenStreetMap, Sentinel Hub, GeoNames, GPS Visualizer |
| 19 | Paste & Archive Sites | 14 | Pastebin, Rentry, PrivateBin, Wayback Machine, Archive.today |
| 20 | Developer Tools | 20 | NPM, PyPI, MDN, LeetCode, CodeWars, StackOverflow, DevDocs |
| 21 | Wireless & IoT | 15 | WiGLE, CellMapper, Shodan IoT, RouterPwn, Insecam, Mirai Tracker |
| 22 | Phishing Detection | 15 | Google SafeBrowse, PhishTank, CheckPhish, ScamAdviser, Trustpilot |
| 23 | Government & Cert DB | 15 | CISA, NIST, FBI IC3, INTERPOL, Europol, NCSC UK, CERT/CC |
| 24 | Image, Video & Media | 15 | TinEye, PimEyes, Forensically, EXIF Viewer, FaceCheck.id |
| 25 | Extra Bonus Tools | 22 | Nmap, SQLMap, FFUF, Nuclei, GAU, Amass, Masscan, RustScan |
| 26 | Free Tire Search & Price | 35 | TireRack, Discount Tire, eBay, Walmart, Freecycle, OfferUp |
| 27 | Real-Time API Fetchers | 40 | ipapi.co, OpenWeatherMap, GitHub API, CoinGecko, Agify.io |
| 28 | Vehicle Database & Specs | 25 | NHTSA VIN, Kelley Blue Book, Carfax, Edmunds, CarMax, Copart |
| 29 | Price Comparison & Deals | 20 | Google Shopping, CamelCamelCamel, Slickdeals, Rakuten, Groupon |
| 30 | Web Fetchers & Scrapers | 30 | SerpAPI, Diffbot, ScrapingBee, Apify, Common Crawl, Bright Data |

---

## AI Intelligence Fetcher

The AI Fetch Panel provides one-click multi-tab intelligence gathering across 11 domains. Each module opens 3 URLs simultaneously with a 400ms stagger delay, logs progress to an inline result panel, and shows a toast notification.

```
┌─────────────────────┬──────────────────────────────────────────┐
│ Module              │ Endpoints Launched                       │
├─────────────────────┼──────────────────────────────────────────┤
│ Full OSINT Scan     │ IP Geo + WHOIS + Shodan                  │
│ Geo IP Lookup       │ ipapi.co + ipinfo.io + AbuseIPDB         │
│ WHOIS Fetch         │ DomainTools + crt.sh SSL + DNSDumpster   │
│ Breach Check        │ HaveIBeenPwned + DeHashed + LeakCheck    │
│ Phone Intel         │ TrueCaller + PhoneInfoga + Numverify     │
│ Tire & Vehicle      │ TireRack + Discount Tire + SimpleTire    │
│ Social Scan         │ WhatsMyName + UserSearch + Social Search │
│ Crypto Trace        │ Blockchair + Etherscan + BSCScan         │
│ DNS Enumeration     │ DNSDumpster + SecurityTrails + ViewDNS   │
│ Malware Check       │ VirusTotal + HybridAnalysis + URLScan    │
│ Reverse Image       │ TinEye + Google Images + Yandex Images   │
│ DarkWeb Monitor     │ Ahmia + DarkSearch + Tor Project         │
└─────────────────────┴──────────────────────────────────────────┘
```

**Total: 36 API endpoints** configurable via `FETCH_MAP` in JavaScript.

---

## Android Application

The native Android app wraps the entire web application in a hardened `WebView` with full JavaScript bridging, offline asset loading, external URL intent handling, and immersive fullscreen mode.

### Android Installation

1. Download `jigsi-karia-v5.apk` from the [repository root](https://github.com/rajkotpodman/jigsi-karia-search)
2. On your Android device, enable **Settings > Security > Unknown Sources**
3. Open the APK file and tap **Install**
4. Launch "Jigsi Karia" from your app drawer

**Requirements:** Android 5.0 (API 21) or higher

### Android Project Structure

```
android/
├── build.gradle                          # Root: AGP 8.2.0 plugin, clean task
├── settings.gradle                       # Module registration, repo config
├── gradle.properties                     # JVM args, AndroidX flags
├── gradlew / gradlew.bat                 # Gradle wrapper scripts
├── gradle/wrapper/
│   ├── gradle-wrapper.jar                # Wrapper binary
│   └── gradle-wrapper.properties         # Gradle 8.5 distribution URL
├── .gitignore                            # Android-specific ignores
└── app/
    ├── build.gradle                      # App: compileSdk 34, dependencies
    ├── proguard-rules.pro                # ProGuard keep rules
    └── src/main/
        ├── AndroidManifest.xml           # Permissions, activity, intent filters
        ├── assets/                       # Bundled web application files
        │   ├── index.html                #   (3,277 lines — the entire app)
        │   ├── manifest.json             #   PWA manifest
        │   ├── sw.js                     #   Service Worker
        │   └── robots.txt                #   Crawl rules
        ├── java/com/jigsi/karia/
        │   └── MainActivity.java         # WebView host activity (253 lines)
        └── res/
            ├── drawable/
            │   └── ic_launcher_foreground.xml   # Lightning bolt vector icon
            ├── layout/
            │   └── activity_main.xml            # WebView + ProgressBar layout
            ├── mipmap-anydpi-v26/
            │   ├── ic_launcher.xml              # Adaptive icon
            │   └── ic_launcher_round.xml        # Round adaptive icon
            ├── values/
            │   ├── colors.xml                   # Matrix-green color palette
            │   ├── strings.xml                  # App name and labels
            │   └── themes.xml                   # Material theme (dark, no action bar)
            └── xml/
                └── backup_rules.xml             # Auto-backup rules
```

### Android Build from Source

```bash
# Prerequisites
# - Java JDK 17+
# - Android SDK (platforms;android-34, build-tools;34.0.0)
# - Set ANDROID_SDK_ROOT environment variable

# Clone and enter android directory
git clone https://github.com/rajkotpodman/jigsi-karia-search.git
cd jigsi-karia-search/android

# Make gradlew executable
chmod +x gradlew

# Build debug APK
./gradlew assembleDebug

# Build release APK (unsigned)
./gradlew assembleRelease

# Sign the release APK
apksigner sign --ks your-keystore.jks \
  --out app/build/outputs/apk/release/jigsi-karia-signed.apk \
  app/build/outputs/apk/release/app-release-unsigned.apk

# Verify
apksigner verify app/build/outputs/apk/release/jigsi-karia-signed.apk
```

**Build output:**

| Variant | Path | Size |
|---------|------|:----:|
| Debug | `app/build/outputs/apk/debug/app-debug.apk` | ~4.6 MB |
| Release (unsigned) | `app/build/outputs/apk/release/app-release-unsigned.apk` | ~4.6 MB |
| Release (signed) | `app/build/outputs/apk/release/jigsi-karia-v5.apk` | 4.6 MB |

### Android JavaScript Bridge API

The `MainActivity` exposes a `WebAppInterface` class as `window.Android` in the WebView:

```javascript
// Show native Android toast
Android.showToast("Search completed!");

// Trigger native share sheet
Android.shareContent("Jigsi Karia", "900+ OSINT tools", "https://...");

// Open URL in external browser
Android.openExternal("https://example.com");

// Get app version string
const version = Android.getAppVersion();  // "5.0.0"

// Check network connectivity
const online = Android.isOnline();
```

### Android Key Files

| File | Lines | Purpose |
|------|:-----:|---------|
| `MainActivity.java` | 253 | WebView host, JS bridge, external URL handler, lifecycle |
| `AndroidManifest.xml` | 40 | Permissions (INTERNET, NETWORK, WIFI, VIBRATE), activities, intent filters |
| `app/build.gradle` | 45 | SDK versions, dependencies (AppCompat, WebKit, Material) |
| `activity_main.xml` | 17 | LinearLayout with ProgessBar + WebView |
| `colors.xml` | 12 | Matrix-green primary palette |
| `themes.xml` | 22 | MaterialComponents.NoActionBar dark theme |

### Android Features

| Feature | Implementation |
|---------|----------------|
| Target/Compile SDK | 34 (Android 14) |
| Min SDK | 21 (Android 5.0) |
| WebView Engine | Chromium WebView with full JS/DOM/localStorage |
| URL Handling | http/https → external browser, whatsapp/tel/mailto → native app, file:// → internal |
| Fullscreen | API 30+ WindowInsetsController, API <30 SYSTEM_UI_FLAG flags |
| JavaScript Bridge | WebAppInterface with toast, share, openExternal, getAppVersion, isOnline |
| Progress Bar | Horizontal ProgressBar tinted Matrix green (#00ff00) |
| Back Navigation | WebView.goBack() for history, Activity.finish() when at root |
| Lifecycle | onPause/onResume/onDestroy properly forwarded to WebView |
| Dependencies | AppCompat 1.6.1, Core 1.12.0, WebKit 1.9.0, Material 1.11.0 |
| Gradle | AGP 8.2.0, Gradle 8.5, Java 17 |

---

## Web Deployment

### Static Hosting (Zero Config)

| Platform | Setup |
|----------|-------|
| **GitHub Pages** | Push to `main` branch, enable in Settings > Pages, set source to root |
| **Vercel** | Import repo — auto-detected static site, instant deploy |
| **Netlify** | Drag folder or connect repo — no build command needed |
| **Cloudflare Pages** | Connect repo, build command: `(none)`, output directory: `/` |
| **Surge** | `npx surge . jigsi-karia.surge.sh` |
| **Render** | Create static site, publish directory: `/` |

### PWA Verification

```bash
# Verify manifest serves correctly
curl -s https://your-domain.com/manifest.json | python3 -m json.tool

# Verify service worker is registered
curl -s https://your-domain.com/sw.js | head -3

# Audit with Lighthouse
# Open Chrome DevTools > Lighthouse > Run audit
```

The app scores high on Lighthouse PWA checks due to:
- Valid `manifest.json` with theme_color, icons, and standalone display
- Registered service worker with cache-first strategy
- Responsive viewport meta tag
- All content served over HTTPS

---

## Repository Structure

```
jigsi-karia-search/
│
├── index.html                  # Main application (3,277 lines, 213 KB)
│                               #   CSS:    540 lines  (embedded <style>)
│                               #   HTML: 1,267 lines  (30 category sections, 900+ buttons)
│                               #   JS:   1,448 lines  (engine mappings, AI fetch, auth)
│
├── jigsi-karia-v5.apk          # Signed release APK (4.6 MB) — install on Android 5.0+
│
├── manifest.json               # PWA Web App Manifest (27 lines)
├── sw.js                       # Service Worker with cache-first strategy (48 lines)
├── robots.txt                  # SEO crawl directives
├── .gitignore                  # Node modules, build artifacts, IDE files
├── README.md                   # You are here
│
└── android/                    # Full Android Studio project
    ├── build.gradle             #   Root Gradle config (AGP 8.2.0)
    ├── settings.gradle          #   Module and repository configuration
    ├── gradle.properties        #   JVM args (2048m), AndroidX flags
    ├── gradlew                  #   Gradle wrapper (Unix)
    ├── gradlew.bat              #   Gradle wrapper (Windows)
    ├── .gitignore               #   Android-specific ignores
    ├── gradle/wrapper/
    │   ├── gradle-wrapper.jar
    │   └── gradle-wrapper.properties
    └── app/
        ├── build.gradle         #   App-level: SDK 34, dependencies
        ├── proguard-rules.pro   #   ProGuard keep rules
        └── src/main/
            ├── AndroidManifest.xml
            ├── assets/          #   Bundled web files (4 files)
            ├── java/.../MainActivity.java
            └── res/             #   Resources (8 files)
```

**Total project files:** 27 source files + 1 signed APK  
**Total lines of code:** ~3,719 (web + Android combined, excluding auto-generated Gradle files)

---

## Architecture & Data Flow

```
┌─────────────────────────────────────────────────────────┐
│                      USER INPUT                          │
│         (phone, IP, domain, email, VIN, query)           │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│                 SMART SEARCH LAYER                       │
│  ┌─────────────┐  ┌──────────────┐  ┌────────────────┐  │
│  │ Autocomplete │  │ Search       │  │ Clipboard      │  │
│  │ (30 terms)   │  │ History MRU  │  │ Copy Button    │  │
│  └─────────────┘  └──────────────┘  └────────────────┘  │
└─────────────────────┬───────────────────────────────────┘
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
┌──────────────┐ ┌─────────┐ ┌──────────────────────┐
│ 900+ Engines │ │ AI Fetch│ │ Quick Access Ribbon  │
│ openEngine() │ │ Panel   │ │ (Phone/Email/IP/...) │
│ Opens query  │ │ 36 URLs │ │ One-click presets    │
│ in new tab   │ │ Stagger │ │                      │
│              │ │ launch  │ │                      │
└──────────────┘ └─────────┘ └──────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│                 STORAGE (localStorage)                   │
│  Credentials | Theme | Visit Count | Search History     │
│  (with _memStore fallback if localStorage is blocked)   │
└─────────────────────────────────────────────────────────┘
```

### Engine Resolution Flow

```
1. User enters query in search input
2. User clicks a category button (e.g., "Shodan")
3. openEngine('shodan') is called
4. Query is URI-encoded and added to search history
5. Engine mapping resolves: shodan → "https://www.shodan.io/search?query={enc}"
6. window.open(url, '_blank') launches in new tab
```

---

## Technical Specifications

### Web Application

| Attribute | Value |
|-----------|-------|
| File size | 213 KB (218,112 bytes) |
| Total lines | 3,277 |
| CSS lines | ~540 |
| HTML lines | ~1,267 |
| JavaScript lines | ~1,448 |
| External dependencies | **0** (zero) |
| CDN requests | **0** (zero) |
| Engine URL mappings | 900+ |
| CSS class variants | 40 category color classes |
| Autocomplete keywords | 30 |
| JavaScript functions | 26 named + 3 anonymous |
| AI Fetch modules | 11 (36 total endpoints) |
| Search history capacity | 10 items (MRU) |

### Android Application

| Attribute | Value |
|-----------|-------|
| APK size | 4.6 MB |
| APK type | Signed release (RSA 2048-bit) |
| compileSdk | 34 (Android 14) |
| minSdk | 21 (Android 5.0 Lollipop) |
| targetSdk | 34 |
| versionCode | 5 |
| versionName | 5.0.0 |
| Kotlin usage | 0 (pure Java) |
| Java source lines | 253 |
| Permissions | INTERNET, ACCESS_NETWORK_STATE, ACCESS_WIFI_STATE, VIBRATE |
| Gradle | 8.5 |
| AGP | 8.2.0 |
| Build time | ~3 minutes |

### Browser Compatibility

| Browser | Support |
|---------|:-------:|
| Chrome 90+ | Full |
| Firefox 90+ | Full |
| Safari 15+ | Full (minor canvas perf difference) |
| Edge 90+ | Full |
| Samsung Internet | Full |
| Opera | Full |
| Android WebView | Full (native APK target) |

---

## Color System

```
┌──────────────┬──────────┬─────────────────────────┐
│ Role         │ Hex      │ Usage                   │
├──────────────┼──────────┼─────────────────────────┤
│ Primary      │ #00ff00  │ Matrix green, borders    │
│ Secondary    │ #00bcff  │ Cyber blue, accents      │
│ Accent       │ #ff0055  │ Hot pink, highlights     │
│ Warning      │ #ffaa00  │ Amber, pro hub           │
│ Danger       │ #ff4444  │ Red, error states        │
│ Background   │ #000000  │ Page background          │
│ Surface      │ #0a0f1d  │ Card/panel backgrounds   │
│ Text         │ #cccccc  │ Secondary text           │
└──────────────┴──────────┴─────────────────────────┘
```

**Category Color Classes (40 total):**

```
Search:   #00ff00   OSINT:    #ff0055   Network:  #ffaa00   Exploit:  #aa44ff
Threat:   #ff4444   Social:   #ff88cc   AI:       #cc33ff   Crypto:   #ffaa33
Dark:     #333333   Cloud:    #66ddff   Leak:     #ff66aa   Forensic: #33aaff
Misc:     #66ccff   News:     #ff9933   Pentest:  #cc0000   Sandbox:  #009966
VPN:      #005599   Privacy:  #336699   Email:    #dd4499   Geo:      #22aa55
Paste:    #7755cc   Archive:  #aa6600   Dev:      #0077cc   Wireless: #33bbaa
IoT:      #996600   Phishing: #ff5500   Gov:      #334477   Image:    #ee44bb
Video:    #cc2244   Tire:     #ff6600   Price:    #22cc44   API:      #7744ff
Review:   #00aacc   Vehicle:  #557799   Tyre:     #cc6600   Freebie:  #ee2277
Market:   #006699   Fetch:    #ff3377   Deal:     #ffbb00   Cert:     #33aa77
```

---

## Authentication

The portal uses `localStorage`-based credential management with a `_memStore` fallback for environments where `localStorage` is unavailable (e.g., some WebView configurations).

```
Default credentials:  admin / admin
Minimum length:       2 characters
Persistence:          localStorage (survives page reload and app restart)
Fallback:             In-memory object (_memStore) if localStorage blocked
```

To reset credentials, clear localStorage or run in console:
```javascript
localStorage.removeItem('gate_user');
localStorage.removeItem('gate_pass');
```

---

## Security Notice

> **IMPORTANT:** This dashboard is structured explicitly for authorized cyber security verification, data intelligence research, and ethical OSINT investigation. Do not use this site for any illegal activities. Users must acknowledge the notice banner before accessing tools.

- No data is collected, proxied, or stored server-side
- All tools open URLs in external browser tabs pointed at legitimate third-party services
- User credentials are stored only in `localStorage` on the device
- The app requests only essential Android permissions (INTERNET, NETWORK_STATE)

---

## Contributing / Build Guide

### Web Development

```bash
# No build step required — edit index.html directly
# Test locally:
python3 -m http.server 8080

# Validate HTML (optional):
# Open in Chrome DevTools > Console for errors
```

### Adding New Tools

1. Add a button in the appropriate category section in `index.html`
2. Add the URL mapping in the `engines` object (inside `openEngine()` function)
3. Optionally add a color class if it belongs to a new category

```javascript
// Example: adding a new search engine
// In engines object:
mynewtool: `https://mynewtool.com/search?q=${encodeURIComponent(query)}`,

// In HTML:
<button class="engine-btn c-osint" onclick="openEngine('mynewtool')">My New Tool</button>
```

### Android Build Setup

```bash
# 1. Install Java 17+
# 2. Install Android SDK command-line tools
# 3. Set environment variables:
export ANDROID_SDK_ROOT=/path/to/android-sdk
export JAVA_HOME=/path/to/jdk-17

# 4. Accept licenses
yes | $ANDROID_SDK_ROOT/cmdline-tools/latest/bin/sdkmanager --licenses

# 5. Install SDK components
$ANDROID_SDK_ROOT/cmdline-tools/latest/bin/sdkmanager \
  "platforms;android-34" \
  "build-tools;34.0.0" \
  "platform-tools"

# 6. Build
cd android && ./gradlew assembleRelease
```

---

## Contact & Links

| Channel | Link |
|---------|------|
| **GitHub** | [rajkotpodman/jigsi-karia-search](https://github.com/rajkotpodman/jigsi-karia-search) |
| **WhatsApp** | [+91 98980 48483](https://wa.me/919898048483) |
| **Hub ID** | jigsi_karia |
| **Pro License** | Contact via WhatsApp |
| **Digital Store** | [WhatsApp Catalog](https://wa.me/c/919898048483) |
| **Donation** | [Google Form](https://docs.google.com/forms/d/e/1FAIpQLScJ7WjuxEXqdoSlUtxN7NQ8UeKpbEAeA9iIO-IXOmBmYzlLHQ/viewform) |

---

<p align="center">
  <b>Jigsi Karia v5.0.0</b> — Built in Gujarat, deployed globally.<br/>
  <sub>Educational and authorized research use only.</sub>
</p>
