# Jigsi Karia - Cyber OSINT Gateway & Hacker Scanner

**Version 5.0** | **900+ Tools** | **30 Categories** | **70+ API Fetchers**

A single-file, zero-dependency cyber intelligence dashboard aggregating 900+ search engines, OSINT tools, exploit databases, API fetchers, dark web scanners, and AI-powered intelligence modules — all accessible through one terminal-themed interface.

---

## Table of Contents

- [Features](#features)
- [Live Preview](#live-preview)
- [Category Index](#category-index)
- [AI Intelligence Fetcher](#ai-intelligence-fetcher)
- [Quick Start](#quick-start)
- [Deployment](#deployment)
- [File Structure](#file-structure)
- [Tech Stack](#tech-stack)
- [Color System](#color-system)
- [Authentication](#authentication)
- [PWA Support](#pwa-support)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Security Notice](#security-notice)
- [License](#license)

---

## Features

| Feature | Description |
|---------|-------------|
| Matrix Canvas | Full-screen digital rain animation at 35ms frame rate |
| Smart Search | Autocomplete with 30 keyword suggestions, search history (MRU 10) |
| AI Fetch Engine | 12 configurable intelligence modules launching 3 endpoints each |
| Dark/Light Mode | Persisted theme toggle with full CSS overrides |
| Category Navigation | Quick toolbar with 10 jump points and smooth scroll |
| Clipboard Copy | One-click target copy with visual flash feedback |
| PWA Ready | Installable web app with offline service worker |
| WhatsApp Integration | Floating chat button with direct message link |
| Pro Action Hub | Buy Pro, Donation, and Official Store CTAs |
| Visitor Analytics | Persistent portal visit counter |

---

## Category Index

| # | Category | Buttons | Highlight |
|:--:|----------|:-------:|-----------|
| 1 | Mega Search Engines | 56 | Google, Bing, Yandex, Baidu, SearX, Brave AI |
| 2 | OSINT & Intelligence | 96 | Shodan, Maltego, HaveIBeenPwned, IntelX, Censys |
| 3 | Network & Domain Tools | 55 | DNSDumpster, MXToolBox, BGPView, SecurityTrails |
| 4 | Exploit & Vulnerability DB | 47 | Exploit-DB, NVD, CVE Details, Metasploit, VulHub |
| 5 | Threat Intelligence & Malware | 38 | VirusTotal, MalwareBazaar, MISP, YARA, CrowdStrike |
| 6 | Social & People Search | 48 | LinkedIn, Pipl, Spokeo, WhatsMyName, UserSearch |
| 7 | Advanced AI Suites | 30 | ChatGPT, Claude, Gemini, DeepSeek, Hugging Face |
| 8 | Cryptocurrency & Blockchain | 30 | Blockchair, Etherscan, DeBank, CoinGecko, Glassnode |
| 9 | Dark Web & TOR | 23 | Ahmia, DarkSearch, Tor Project, OnionShare, I2P |
| 10 | Cloud & DevOps OSINT | 28 | AWS, Azure, GCP, Kubernetes, Docker Hub, Vercel |
| 11 | Forensic & Data Leak | 36 | Autopsy, Volatility, BreachDirectory, DeHashed |
| 12 | Misc Hacker Tools | 47 | CyberChef, Hash Killer, JWT.io, CodePen, Regex101 |
| 13 | Cyber Security News | 20 | Krebs, TheHackerNews, BleepingComputer, DarkReading |
| 14 | Pentest, CTF & Lab Tools | 25 | HackTheBox, TryHackMe, HackerOne, Bugcrowd |
| 15 | Sandbox & File Analysis | 20 | Cuckoo, CAPE, Joe Sandbox, Intezer, FileScan.io |
| 16 | Privacy, VPN & Anonymity | 20 | NordVPN, Mullvad, ProtonVPN, PrivacyTools, Tails OS |
| 17 | Email Intel & Spam Check | 19 | MXToolBox, EmailRep, Mail-Tester, NeverBounce |
| 18 | Geo, Map & Location | 20 | Google Maps, OpenStreetMap, Sentinel Hub, GeoNames |
| 19 | Paste & Archive Sites | 14 | Pastebin, Rentry, PrivateBin, Wayback Machine |
| 20 | Developer Tools | 20 | NPM, PyPI, MDN, LeetCode, CodeWars, StackOverflow |
| 21 | Wireless & IoT | 15 | WiGLE, CellMapper, Shodan IoT, RouterPwn, Insecam |
| 22 | Phishing Detection | 15 | Google SafeBrowse, PhishTank, CheckPhish, ScamAdviser |
| 23 | Government & Cert DB | 15 | CERT/CC, CISA, NIST, FBI IC3, INTERPOL, NCSC UK |
| 24 | Image, Video & Media | 15 | TinEye, PimEyes, Forensically, EXIF Viewer |
| 25 | Extra Bonus Tools | 22 | Nmap, SQLMap, FFUF, Nuclei, GAU, Amass, Masscan |
| 26 | Free Tire Search & Price | 35 | TireRack, Discount Tire, eBay, Walmart, Freecycle |
| 27 | Real-Time API Fetchers | 40 | ipapi.co, OpenWeatherMap, GitHub API, CoinGecko |
| 28 | Vehicle Database & Specs | 25 | NHTSA VIN, Kelley Blue Book, Carfax, Edmunds, CarMax |
| 29 | Price Comparison & Deals | 20 | Google Shopping, CamelCamelCamel, Slickdeals, Rakuten |
| 30 | Web Fetchers & Scrapers | 30 | SerpAPI, Diffbot, ScrapingBee, Apify, Common Crawl |

---

## AI Intelligence Fetcher

The AI Fetch Panel provides one-click multi-tab intelligence gathering across 12 domains:

```
osint_full_scan  -> IP Geo + WHOIS + Shodan
ip_geo           -> ipapi.co + ipinfo.io + AbuseIPDB
domain_whois     -> DomainTools + crt.sh SSL + DNSDumpster
email_breach     -> Have I Been Pwned + DeHashed + LeakCheck
phone_lookup     -> TrueCaller + PhoneInfoga + Numverify
tire_search      -> TireRack + Discount Tire + SimpleTire
social_scan      -> WhatsMyName + UserSearch + Social Searcher
crypto_trace     -> Blockchair + Etherscan + BSCScan
dns_enum         -> DNSDumpster + SecurityTrails + ViewDNS
malware_check    -> VirusTotal + HybridAnalysis + URLScan
image_reverse    -> TinEye + Google Images + Yandex Images
darkweb_monitor  -> Ahmia + DarkSearch + Tor Project
```

Each module opens 3 URLs in new tabs with a 400ms stagger delay, logs output to the inline result panel, and displays a toast notification.

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/rajkotpodman/jigsi-karia-search.git

# Navigate to project
cd jigsi-karia-search

# Start local server (Python 3)
python3 -m http.server 8080 --bind 0.0.0.0

# Or with Node.js
npx serve .
```

Open `http://localhost:8080` in your browser.

**Default credentials:** `admin` / `admin`

---

## Deployment

### Static Hosting (Zero Config)

Drop the files onto any static host:

| Platform | Setup |
|----------|-------|
| GitHub Pages | Push to `main` branch, enable in Settings > Pages |
| Vercel | Import repo — auto-detected, no config needed |
| Netlify | Drag folder or connect repo — instant deploy |
| Cloudflare Pages | Connect repo, set build command to `(none)`, output to `/` |
| Surge | `npx surge . jigsi-karia.surge.sh` |

### PWA Verification

After deployment, verify PWA readiness:

```bash
# Check manifest loads
curl -s https://your-domain.com/manifest.json | python3 -m json.tool

# Verify service worker
curl -s https://your-domain.com/sw.js | head -1
```

---

## File Structure

```
jigsi-karia-search/
├── index.html          # Main application (3,277 lines, 213 KB)
│                       #   - 540 lines CSS (embedded)
│                       #   - 1,267 lines HTML (30 categories)
│                       #   - 1,448 lines JavaScript
├── manifest.json       # PWA manifest (installable web app)
├── sw.js               # Service Worker (offline caching)
├── robots.txt          # Search engine crawl rules
└── .gitignore          # Excluded files and directories
```

**Zero dependencies** — no `node_modules`, no CDN imports, no build step.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 single-file |
| Styling | CSS3 (Custom Properties, Grid, Flexbox, Animations) |
| Scripting | Vanilla JavaScript (ES6+) |
| Canvas | Canvas 2D API (Matrix rain) |
| Storage | Web Storage API (localStorage + sessionStorage) |
| Clipboard | Async Clipboard API + execCommand fallback |
| PWA | Service Worker + Web App Manifest |
| Font | Courier New monospace (system font, zero latency) |

---

## Color System

The interface uses a cyber/terminal aesthetic with 40 distinct category color classes:

```
Primary:    #00ff00 (Matrix Green)    Secondary:  #00bcff (Cyber Blue)
Accent:     #ff0055 (Hot Pink)        Warning:    #ffaa00 (Amber)
Danger:     #ff4444 (Red)             Dark BG:    #0a0f1d (Deep Navy)
```

**Category Color Map:**

```
OSINT: #ff0055    Network: #ffaa00    Exploit: #aa44ff    Threat: #ff4444
Social: #ff88cc   AI:      #cc33ff    Crypto:  #ffaa33    Dark:    #333333
Cloud:  #66ddff   Leak:    #ff66aa    VPN:     #005599    Email:   #dd4499
Tire:   #ff6600   Price:   #22cc44    API:     #7744ff    Vehicle: #557799
Fetch:  #ff3377   Deal:    #ffbb00    Freebie: #ee2277    Market:  #006699
```

---

## Authentication

The portal uses localStorage-based credential management:

```
Default Login:  admin / admin
Register:       Create custom username/password (min 2 chars each)
```

Credentials persist across sessions via `localStorage` with a memory-based fallback if storage is blocked.

**UI is in Gujarati language** for the primary target audience.

---

## PWA Support

The app is installable as a Progressive Web App:

- **Installable** — Add to home screen on Android/iOS/Desktop
- **Offline Ready** — Service Worker caches `index.html` and `manifest.json`
- **Standalone Mode** — Launches without browser chrome
- **Theme Color** — System status bar matches Matrix green (`#00ff00`)

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Enter` in search | Triggered via button click (prevented on input) |
| `Tab` | Navigate between interactive elements |
| Click outside search | Closes history/suggestion dropdowns |

---

## Security Notice

> **IMPORTANT:** This dashboard is structured explicitly for authorized cyber security verification, data intelligence research, and ethical OSINT investigation. Do not use this site for any illegal activities. Users must acknowledge the notice banner before accessing tools.

All tools open in external tabs pointed to legitimate third-party services. No data is collected, proxied, or stored server-side beyond the user's own `localStorage`.

---

## License

This project is provided for educational and authorized security research purposes only. Unauthorized use may violate applicable laws.

---

**Maintained by** [rajkotpodman](https://github.com/rajkotpodman)  
**Hub:** jigsi_karia  
**Contact:** [WhatsApp](https://wa.me/919898048483)
