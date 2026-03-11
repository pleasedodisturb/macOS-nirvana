# Mac Holy Grail — The Ultimate macOS Stack

> One opinionated pick per category. Cross-referenced from awesome-mac lists, Reddit r/macapps, Hacker News, Setapp, nikiv.dev, and 30+ curated sources. No fluff.

---

## Philosophy

1. **Keyboard-first** — every action has a hotkey
2. **Own your data** — local-first, open-source when possible
3. **One tool per job** — no overlapping apps
4. **Free > Paid > Subscription** — avoid subscriptions unless genuinely irreplaceable
5. **AI lives in the terminal** — Claude Code is the brain, everything else is the body

---

## Tier 1: Core System (install these first)

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Launcher** | **Raycast** | Free | Built-in clipboard history, snippets, window management, calculator, 1000+ extensions. Replaces 5 apps. | Alfred ($34 Powerpack, better custom workflows) |
| **Window Tiling** | **AeroSpace** | Free/OSS | i3-like tiling via TOML config. Keyboard-driven workspaces faster than native Spaces. | Rectangle (free, simple snap), Amethyst (free, auto-tile) |
| **Menu Bar** | **Ice** | Free/OSS | Hide/show/rearrange menu bar icons. Bartender replacement (Bartender has privacy concerns after acquisition). | Hidden Bar (simpler), SketchyBar (fully custom) |
| **Keyboard** | **Karabiner-Elements** | Free/OSS | Remap anything at kernel level. Caps Lock → Hyper key. Per-app mods. The foundation of nikiv's entire workflow. | Hyperkey (free, just Caps→Hyper), BetterTouchTool ($22, also trackpad) |
| **Automation** | **Keyboard Maestro** | $36 once | Automate anything: hotkey triggers, clipboard manipulation, conditionals, UI scripting. Nothing else comes close. | Shortcuts (free, built-in), Hammerspoon (free, Lua scripting) |
| **Password Manager** | **Bitwarden** | Free/OSS | Open-source, self-hostable, cross-platform, browser extension, CLI tool. No vendor lock-in. | KeePassXC (free, offline-only purist) |
| **System Monitor** | **Stats** | Free/OSS | CPU, GPU, RAM, temps, network, disk in menu bar. 95% of iStat Menus for $0. | iStat Menus ($12, prettier) |
| **Uninstaller** | **Pearcleaner** | Free/OSS | More thorough than AppCleaner, actively developed, catches files AppCleaner misses. | AppCleaner (free, simpler) |

---

## Tier 2: Development

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Terminal** | **Ghostty** | Free/OSS | Fastest GPU-rendered terminal on macOS. Native Metal, Zig-based. Already set up. | Alacritty (minimal, pairs well with tmux), WezTerm (built-in multiplexer) |
| **Shell** | **Zsh** + Oh My Zsh + Starship | Free | Autosuggestions, syntax highlighting, fuzzy history, beautiful prompt. Already set up. | Fish (friendlier defaults but different syntax) |
| **Multiplexer** | **tmux** | Free/OSS | Persistent sessions, scriptable layouts, survives crashes. Already set up. | Zellij (friendlier UI, Rust-based) |
| **Editor** | **VS Code** + **Neovim** | Free | VS Code for visual work + extensions, Neovim for terminal-native. | Zed (Rust, fast, built-in AI), Cursor (AI-first but $20/mo) |
| **AI Coding** | **Claude Code** | Subscription | The brain. Edits files, runs commands, searches code, manages git. Everything feeds into this. | — |
| **Git GUI** | **Fork** | Free eval / $50 | Fast native diffs, interactive rebase, merge conflict resolver. Free eval is forever. | Sublime Merge ($99, nikiv's pick), GitUp (free/OSS, unique undo) |
| **API Testing** | **Bruno** | Free/OSS | Collections as plain-text files in your repo (git-friendly). Offline, no account. Anti-Postman. | Insomnia (free, GraphQL), Thunder Client (VS Code extension) |
| **Database** | **TablePlus** | Free tier / $89 | Native, fast, supports Postgres/MySQL/SQLite/Redis/Mongo. | DBeaver (free/OSS, broadest support), DataGrip (free non-commercial) |
| **Docker** | **OrbStack** | Free personal | 2s startup (vs Docker Desktop 30s), 4x less power, runs Linux VMs too. | Colima (free/OSS, terminal-only), Docker Desktop (default but heavy) |
| **Dev Toolkit** | **DevUtils** | $14 once | Auto-detects clipboard (JSON, JWT, Base64, regex, UUID) → offers right tool. Offline. | Boop (free/OSS, text transforms scratchpad) |
| **HTTP Debugging** | **Proxyman** | Free tier | Modern native HTTP proxy. Intercept, inspect, modify traffic. Way nicer than Charles. | mitmproxy (free/OSS, terminal, scriptable) |
| **API Docs** | **Dash** | $30 once | Offline documentation search for 200+ APIs. Instant. Pairs with Raycast. | Zeal (free/OSS alternative) |
| **Diff/Merge** | **Kaleidoscope** | $150 | Visual diff for text, images, and folders. Beautiful. | Medio (free/OSS, lighter), opendiff (free, built-in) |
| **Version Manager** | **mise** | Free/OSS | Rust-based, manages Node/Python/Ruby/Go/etc. Faster than asdf, simpler config. | fnm (Node only), pyenv (Python only) |
| **Shell History** | **Atuin** | Free/OSS | Encrypted shell history sync across machines. SQLite-backed, fuzzy search. nikiv uses this. | fzf + Ctrl+R (simpler, already set up) |

---

## Tier 3: Productivity

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Browser** | **Firefox** + **Safari** | Free | Firefox for dev (privacy, containers, DevTools). Safari for personal (battery, Apple integration). | Zen Browser (Firefox fork, Arc-like UX) |
| **Email** | **Apple Mail** | Free | Zero setup, fast, blocks trackers. Don't pay for email if you don't live in it. | Mimestream ($50/yr, native Gmail), Thunderbird (free, PGP) |
| **Calendar** | **Fantastical** | Free tier / $5/mo | Natural language ("lunch Tuesday noon"), time zones, Zoom links. nikiv's pick too. | BusyCal ($50 once, no subscription), Notion Calendar (free) |
| **Notes** | **Obsidian** | Free | Local markdown you own forever. 1500+ plugins. Graph view. Vim keybindings. | Logseq (free/OSS, block-based), Reflect (nikiv's pick, paid) |
| **Tasks** | **Things 3** | $50 once | Most beautiful task manager on Apple. Keyboard-driven, zero subscription. nikiv uses it. | Todoist (free tier, cross-platform), TickTick (free, built-in Pomodoro) |
| **File Manager** | **ForkLift** | $20 once | Dual-pane, SFTP/S3/GDrive connections, folder sync. | Marta (free, keyboard-driven), Commander One (free, dual-pane) |
| **Quick Notes** | **SideNotes** | $15 once | Notes that slide in from screen edge. Quick capture without context-switching. | One Thing (free, single task in menu bar) |
| **Text Actions** | **PopClip** | $15 once | Select text → popup with contextual actions (search, transform, send to apps). "How did I live without this." | — |
| **Link Router** | **Velja** | Free | Click a link → choose which browser/app opens it. Essential for multi-browser setup. | Finicky (free/OSS, rule-based) |

---

## Tier 4: Media & Content

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Screenshots** | **CleanShot X** | $29 once | Scrolling capture, annotation, OCR, recording, GIF, cloud upload. Replaces 5 tools. nikiv uses it. | Shottr (free, lightweight), Xnapper ($15, beautifies screenshots) |
| **Video Player** | **IINA** | Free/OSS | Native macOS, hardware-accelerated, trackpad gestures, PiP. Feels Apple-made. nikiv uses it. | VLC (free, plays everything) |
| **Music** | **Spotify** | Subscription | Cross-platform, better discovery. Apple Music if all-in on Apple ecosystem. | Swinsian ($25, local FLAC/DSD files) |
| **PDF** | **Skim** | Free/OSS | Fast, great annotations. Preview handles 80% of cases already. | PDF Expert ($80/yr, editing/signing) |
| **Image Editing** | **Affinity Photo 2** | Free (personal) | Photoshop-class, now free for individuals. Layers, masks, RAW, batch. | Pixelmator Pro ($50, ML-powered, Mac-native) |
| **Torrents** | **qBittorrent** | Free/OSS | Built-in search, IP filtering, VPN kill-switch, RSS feeds. | Transmission (free, simpler) |
| **RSS** | **NetNewsWire** | Free/OSS | Native Swift, syncs across Apple devices. Perfect at $0. | Reeder ($10, prettier typography) |
| **Transcription** | **Aiko** | Free | On-device Whisper transcription. No cloud, no subscription. By sindresorhus. | MacWhisper (free tier), buzz (free/OSS) |

---

## Tier 5: Communication & Cloud

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Messaging** | **iMessage** + **Signal** + **Telegram** | Free | iMessage for Apple, Signal for encrypted, Telegram for communities. | Texts.com ($5/mo, aggregates all messengers) |
| **Video Calls** | **Zoom** | Free tier | The standard. Everyone has it. | Google Meet (no install), FaceTime (Apple only) |
| **Cloud Storage** | **iCloud** + **Syncthing** | $1-3/mo + Free | iCloud for ecosystem. Syncthing for P2P machine sync (no cloud). | Proton Drive (free, zero-knowledge encryption) |
| **File Sharing** | **LocalSend** | Free/OSS | Cross-platform AirDrop (works with Android/Windows/Linux). | NearDrop (free, Google Quick Share for Mac) |

---

## Tier 6: Network & Security

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **VPN (Mesh)** | **Tailscale** | Free (100 devices) | WireGuard mesh VPN. Zero-config. Your Mac Mini is one click away. nikiv uses it. | Headscale (free/OSS, self-hosted Tailscale) |
| **VPN (Privacy)** | **Mullvad** | $5.50/mo | No account (just a number), cash/crypto, audited, WireGuard. | ProtonVPN (free tier) |
| **Firewall** | **LuLu** | Free/OSS | See/control which apps connect to internet. 90% of Little Snitch for $0. Patrick Wardle / Objective-See. | Little Snitch ($59, more polished) |
| **Security Audit** | **ParetoSecurity** | Free/OSS | Menu bar app auditing your Mac: FileVault, firewall, Gatekeeper, etc. | — |
| **Webcam/Mic Guard** | **OverSight** | Free/OSS | Alerts when mic/webcam are accessed. Objective-See suite. | — |
| **Backup** | **Carbon Copy Cloner** | $40 once | Bootable clones + incremental. Does what Time Machine can't. | Time Machine (free, file-level), Backblaze ($99/yr, cloud) |
| **Encryption** | **Cryptomator** | Free/OSS | Client-side encryption for iCloud/Dropbox/any cloud folder. | — |
| **DNS** | **NextDNS** | Free tier | Cloud DNS firewall with ad/tracker blocking. Set and forget. | Pi-hole (self-hosted) |

---

## Tier 7: Quality of Life (Hidden Gems)

Small apps that punch above their weight. Install these after the essentials.

| App | Cost | What it does |
|-----|------|--------------|
| **MonitorControl** | Free/OSS | Control external monitor brightness/volume from Mac keyboard. Essential for non-Apple displays. |
| **AltTab** | Free/OSS | Windows-style Alt+Tab with full window previews. Huge upgrade over Cmd+Tab. |
| **DockDoor** | Free/OSS | Hover Dock icons to see window previews. Should be built into macOS. |
| **BoringNotch** | Free/OSS | Turns MacBook notch into music controls, file drop zone, clipboard widget. |
| **SlowQuitApps** | Free/OSS | 1-second delay on Cmd+Q. No more accidental app quits. |
| **Overkill** | Free/OSS | Stops iTunes/Music from opening when plugging headphones/iPhone. |
| **Mos** | Free/OSS | Smooth scrolling for external mice. Reverses scroll direction per-device. |
| **Mac Mouse Fix** | Free/OSS | Complete mouse customization: scroll, acceleration, buttons. Replaces vendor drivers. |
| **Keka** | Free/OSS | Archive tool. Handles every format (7z, RAR, ZIP, etc). |
| **Command X** | Free | Adds Cmd+X cut-paste to Finder. By sindresorhus. How is this not built-in? |
| **Pure Paste** | Free | Paste as plain text by default. No more pasting with formatting. By sindresorhus. |
| **MeetingBar** | Free/OSS | Next meeting in menu bar, one-click join. |
| **OnlySwitch** | Free/OSS | All-in-one toggles: dark mode, AirPods connect, hide notch, keep awake, etc. |
| **AlDente** | Free/Pro | Battery charge limiter. Keep battery at 80% when plugged in for longevity. |
| **Suspicious Package** | Free | Inspect .pkg installers before running. See every file that will be installed. |
| **Hazel** | $42 once | Automated folder rules — move, rename, tag files by conditions. Set-and-forget file organization. |
| **KeepingYouAwake** | Free/OSS | Prevent Mac from sleeping. One click in menu bar. |
| **mas** | Free/OSS | Mac App Store from the terminal. `mas install`, `mas upgrade`. |

---

## Tier 8: Quick Look Plugins

Press Space in Finder to preview these file types properly. Install via `brew install --cask`:

| Plugin | Previews |
|--------|----------|
| **QLStephen** | Plain text without extensions (Makefile, README, CHANGELOG) |
| **QLMarkdown** | Markdown rendered as HTML |
| **QLColorCode** | Source code with syntax highlighting |
| **QLImageSize** | Image dimensions + file size overlay |
| **QLVideo** | Video formats QuickTime can't handle |

---

## Sindresorhus Collection

One developer's free micro-apps that keep appearing across every list. Worth browsing [sindresorhus.com](https://sindresorhus.com). Highlights:

- **Command X** — cut-paste in Finder
- **Pure Paste** — plain text paste everywhere
- **Velja** — browser/app link router
- **Lungo** — prevent sleep
- **Aiko** — on-device transcription
- **Dato** — better menu bar clock + calendar
- **One Thing** — single focus task in menu bar
- **Folder Peek** — quick folder contents from menu bar
- **Shareful** — more sharing destinations in share sheets

---

## The Workflow

```
┌─────────────────────────────────────────────────────┐
│  Ghostty → tmux (auto-attach)                       │
│  ├── dev carcadence    → Claude Code + shell         │
│  ├── dev job-search-hq → Claude Code + shell         │
│  └── prefix+s to switch between projects             │
│                                                     │
│  VS Code (Cmd+Tab)                                  │
│  └── Visual diffs, debugging, extensions             │
│                                                     │
│  Raycast (Cmd+Space)                                │
│  ├── Launch apps, search files, clipboard history    │
│  ├── Snippets, calculator, color picker              │
│  └── Extensions: GitHub, Linear, Bitwarden           │
│                                                     │
│  Karabiner                                          │
│  ├── Caps Lock held = Hyper key (Ctrl+Alt+Cmd+Shift) │
│  ├── Hyper+T = Ghostty                               │
│  ├── Hyper+B = Firefox                               │
│  ├── Hyper+E = VS Code                               │
│  ├── Hyper+S = Spotify                               │
│  └── Hyper+N = Obsidian                              │
└─────────────────────────────────────────────────────┘
```

---

## Total Cost

### Free tier (90% of the stack):
Almost everything listed is free or open-source.

### Recommended one-time purchases (~$220):
| App | Cost |
|-----|------|
| Things 3 | $50 |
| CleanShot X | $29 |
| Carbon Copy Cloner | $40 |
| Keyboard Maestro | $36 |
| Dash | $30 |
| ForkLift | $20 |
| PopClip | $15 |
| **Total** | **~$220 once** |

### Optional subscriptions:
| App | Cost | Skip if... |
|-----|------|-----------|
| Fantastical | $57/yr | Use Apple Calendar or BusyCal ($50 once) |
| Mullvad VPN | $66/yr | Don't need privacy VPN |
| **Total** | **~$123/yr max** |

---

## What NOT to Install

| App | Why not |
|-----|---------|
| **Copilot / Cline / Continue** | Claude Code replaces all AI coding assistants |
| **Docker Desktop** | OrbStack is better in every way on Apple Silicon |
| **Bartender** | Privacy concerns after acquisition. Use Ice. |
| **Alfred** (if using Raycast) | Pick one launcher, not both |
| **1Password** | Bitwarden is open-source, free, and good enough |
| **iTerm** (as daily driver) | Keep as backup. Ghostty + tmux is faster. |
| **Wave / Warp** | tmux + Ghostty > fancy terminal apps |
| **Notion** (for personal notes) | Obsidian owns your data locally. Notion doesn't. |
| **Postman** | Bruno is git-friendly, offline, no account needed |
| **Charles Proxy** | Proxyman is native, modern, free tier |
| **Docker Desktop** | OrbStack. Seriously. |
| **Any menu bar weather/clock** | Keep menu bar clean. Use Dato if you really need it. |

---

## Nikiv-Inspired Power Moves

Things worth stealing from [nikiv.dev/workflow](https://nikiv.dev/workflow):

1. **Karabiner as OS-level orchestrator** — not just remapping but the backbone of all app-switching via custom layers. He built a generator (`kar`) for it.
2. **Dual-purpose keys** — every key does double duty (tap vs hold). Caps Lock tap = Esc, hold = Hyper.
3. **Contexts app** ($10) — window switcher bound to a hotkey for instant app jumping by typing app name.
4. **30+ parallel AI prompts** — treats coding as orchestration, not typing. Claude Code + Codex running simultaneously.
5. **Custom CLI tools** — his `flow` (Rust) manages entire project lifecycle with task tracing for AI context.
6. **Four browsers, four purposes** — Safari (daily), Chrome Canary (dev), Safari TP (testing), Arc (social feeds).
7. **SnippetsLab** ($10) + **Snippety** — code snippets + text expansion with placeholders, especially for AI prompts.
8. **Atuin** — shell history sync across machines with encryption.

---

## Install Script

```bash
# Core (brew)
brew install --cask raycast ghostty karabiner-elements obsidian \
  visual-studio-code firefox bitwarden iina skim \
  cleanshot fork bruno tableplus orbstack \
  stats ice forklift the-unarchiver \
  monitorcontrol alt-tab meetingbar

# CLI tools
brew install tmux starship fzf bat neovim mise atuin mas httpie

# Free apps from App Store (use mas)
mas install 1480068668  # Messenger (Signal)
mas install 497799835   # Xcode
mas install 1176895641  # Spark
mas install 1529448980  # Reeder 5

# Quick Look plugins
brew install --cask qlstephen qlmarkdown qlcolorcode qlimagesize qlvideo

# Security
brew install --cask lulu oversight cryptomator suspicious-package

# Quality of life
brew install --cask keepingyouawake keka slowquitapps
```

*Note: Some apps (CleanShot X, Keyboard Maestro, Things 3, ForkLift, PopClip, Hazel, Dash) are purchased from their websites or the App Store directly.*
