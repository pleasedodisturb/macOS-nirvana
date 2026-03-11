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
| **Launcher** | **[Raycast](https://raycast.com/)** | Free | Built-in clipboard history, snippets, window management, calculator, 1000+ extensions. Replaces 5 apps. | [Alfred](https://www.alfredapp.com/) ($34 Powerpack, better custom workflows) |
| **Window Tiling** | **[AeroSpace](https://github.com/nikitabobko/AeroSpace)** | Free/OSS | i3-like tiling via TOML config. Keyboard-driven workspaces faster than native Spaces. | [Rectangle](https://rectangleapp.com/) (free, simple snap), [Amethyst](https://ianyh.com/amethyst/) (free, auto-tile) |
| **Menu Bar** | **[Ice](https://github.com/jordanbaird/Ice)** | Free/OSS | Hide/show/rearrange menu bar icons. Bartender replacement (Bartender has privacy concerns after acquisition). | [Hidden Bar](https://github.com/dwarvesf/hidden) (simpler), [SketchyBar](https://github.com/FelixKratz/SketchyBar) (fully custom) |
| **Keyboard** | **[Karabiner-Elements](https://karabiner-elements.pqrs.org/)** | Free/OSS | Remap anything at kernel level. Caps Lock → Hyper key. Per-app mods. The foundation of nikiv's entire workflow. | [Hyperkey](https://hyperkey.app/) (free, just Caps→Hyper), [BetterTouchTool](https://folivora.ai/) ($22, also trackpad) |
| **Automation** | **[Keyboard Maestro](https://www.keyboardmaestro.com/)** | $36 once | Automate anything: hotkey triggers, clipboard manipulation, conditionals, UI scripting. Nothing else comes close. | [Shortcuts](https://support.apple.com/shortcuts) (free, built-in), [Hammerspoon](https://www.hammerspoon.org/) (free, Lua scripting) |
| **Password Manager** | **[Bitwarden](https://bitwarden.com/)** | Free/OSS | Open-source, self-hostable, cross-platform, browser extension, CLI tool. No vendor lock-in. | [KeePassXC](https://keepassxc.org/) (free, offline-only purist) |
| **System Monitor** | **[Stats](https://github.com/exelban/stats)** | Free/OSS | CPU, GPU, RAM, temps, network, disk in menu bar. 95% of iStat Menus for $0. | [iStat Menus](https://bjango.com/mac/istatmenus/) ($12, prettier) |
| **Uninstaller** | **[Pearcleaner](https://github.com/alienator88/Pearcleaner)** | Free/OSS | More thorough than AppCleaner, actively developed, catches files AppCleaner misses. | [AppCleaner](https://freemacsoft.net/appcleaner/) (free, simpler) |

---

## Tier 2: Development

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Terminal** | **[Ghostty](https://ghostty.org/)** | Free/OSS | Fastest GPU-rendered terminal on macOS. Native Metal, Zig-based. | [Alacritty](https://alacritty.org/) (minimal, pairs well with tmux), [WezTerm](https://wezfurlong.org/wezterm/) (built-in multiplexer) |
| **Shell** | **[Zsh](https://www.zsh.org/)** + [Oh My Zsh](https://ohmyz.sh/) + [Starship](https://starship.rs/) | Free | Autosuggestions, syntax highlighting, fuzzy history, beautiful prompt. | [Fish](https://fishshell.com/) (friendlier defaults but different syntax) |
| **Multiplexer** | **[tmux](https://github.com/tmux/tmux)** | Free/OSS | Persistent sessions, scriptable layouts, survives crashes. | [Zellij](https://zellij.dev/) (friendlier UI, Rust-based) |
| **Editor** | **[VS Code](https://code.visualstudio.com/)** + **[Neovim](https://neovim.io/)** | Free | VS Code for visual work + extensions, Neovim for terminal-native. | [Zed](https://zed.dev/) (Rust, fast, built-in AI), [Cursor](https://cursor.sh/) (AI-first but $20/mo) |
| **AI Coding** | **[Claude Code](https://claude.com/claude-code)** | Subscription | The brain. Edits files, runs commands, searches code, manages git. Everything feeds into this. | — |
| **Git GUI** | **[Fork](https://git-fork.com/)** | Free eval / $50 | Fast native diffs, interactive rebase, merge conflict resolver. Free eval is forever. | [Sublime Merge](https://www.sublimemerge.com/) ($99, nikiv's pick), [GitUp](https://gitup.co/) (free/OSS, unique undo) |
| **API Testing** | **[Bruno](https://www.usebruno.com/)** | Free/OSS | Collections as plain-text files in your repo (git-friendly). Offline, no account. Anti-Postman. | [Insomnia](https://insomnia.rest/) (free, GraphQL), [Thunder Client](https://www.thunderclient.com/) (VS Code extension) |
| **Database** | **[TablePlus](https://tableplus.com/)** | Free tier / $89 | Native, fast, supports Postgres/MySQL/SQLite/Redis/Mongo. | [DBeaver](https://dbeaver.io/) (free/OSS, broadest support), [DataGrip](https://www.jetbrains.com/datagrip/) (free non-commercial) |
| **Docker** | **[OrbStack](https://orbstack.dev/)** | Free personal | 2s startup (vs Docker Desktop 30s), 4x less power, runs Linux VMs too. | [Colima](https://github.com/abiosoft/colima) (free/OSS, terminal-only), [Docker Desktop](https://www.docker.com/products/docker-desktop/) (default but heavy) |
| **Dev Toolkit** | **[DevUtils](https://devutils.com/)** | $14 once | Auto-detects clipboard (JSON, JWT, Base64, regex, UUID) → offers right tool. Offline. | [Boop](https://boop.okat.best/) (free/OSS, text transforms scratchpad) |
| **HTTP Debugging** | **[Proxyman](https://proxyman.io/)** | Free tier | Modern native HTTP proxy. Intercept, inspect, modify traffic. Way nicer than Charles. | [mitmproxy](https://mitmproxy.org/) (free/OSS, terminal, scriptable) |
| **API Docs** | **[Dash](https://kapeli.com/dash)** | $30 once | Offline documentation search for 200+ APIs. Instant. Pairs with Raycast. | [Zeal](https://zealdocs.org/) (free/OSS alternative) |
| **Diff/Merge** | **[Kaleidoscope](https://kaleidoscope.app/)** | $150 | Visual diff for text, images, and folders. Beautiful. | [Medio](https://medio.app/) (free/OSS, lighter), opendiff (free, built-in) |
| **Version Manager** | **[mise](https://mise.jdx.dev/)** | Free/OSS | Rust-based, manages Node/Python/Ruby/Go/etc. Faster than asdf, simpler config. | [fnm](https://github.com/Schniz/fnm) (Node only), [pyenv](https://github.com/pyenv/pyenv) (Python only) |
| **Shell History** | **[Atuin](https://atuin.sh/)** | Free/OSS | Encrypted shell history sync across machines. SQLite-backed, fuzzy search. nikiv uses this. | [fzf](https://github.com/junegunn/fzf) + Ctrl+R (simpler, already set up) |

---

## Tier 3: Productivity

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Browser** | **[Brave](https://brave.com/)** or **[Vivaldi](https://vivaldi.com/)** | Free | Brave: Chromium-based, built-in ad/tracker blocking, privacy-first, fast. Vivaldi: EU-based, insane customizability, tab stacking, built-in mail/calendar, respects privacy. Both have full Chrome DevTools. | [Firefox](https://www.mozilla.org/firefox/) (OSS, containers), [Safari](https://www.apple.com/safari/) (battery life), [Zen](https://zen-browser.app/) (Arc-like UX) |
| **Email** | **[Apple Mail](https://support.apple.com/mail)** | Free | Zero setup, fast, blocks trackers. Don't pay for email if you don't live in it. | [Mimestream](https://mimestream.com/) ($50/yr, native Gmail), [Thunderbird](https://www.thunderbird.net/) (free, PGP) |
| **Calendar** | **[Fantastical](https://flexibits.com/fantastical)** | Free tier / $5/mo | Natural language ("lunch Tuesday noon"), time zones, Zoom links. nikiv's pick too. | [BusyCal](https://www.busymac.com/busycal/) ($50 once, no subscription), [Notion Calendar](https://www.notion.so/product/calendar) (free) |
| **Notes** | **[Obsidian](https://obsidian.md/)** | Free | Local markdown you own forever. 1500+ plugins. Graph view. Vim keybindings. | [Logseq](https://logseq.com/) (free/OSS, block-based), [Reflect](https://reflect.app/) (nikiv's pick, paid) |
| **Tasks** | **[TickTick](https://ticktick.com/)** | Free / $36/yr | Does everything — tasks, habits, Pomodoro timer, calendar view, Eisenhower matrix, Kanban — all in one app. Cross-platform. The Swiss army knife of productivity. | [Things 3](https://culturedcode.com/things/) ($50 once, prettier but Apple-only), [Todoist](https://todoist.com/) (free tier, simpler) |
| **File Manager** | **[ForkLift](https://binarynights.com/)** | $20 once | Dual-pane, SFTP/S3/GDrive connections, folder sync. | [Marta](https://marta.sh/) (free, keyboard-driven), [Commander One](https://mac.eltima.com/file-manager.html) (free, dual-pane) |
| **Quick Notes** | **[SideNotes](https://www.apptorium.com/sidenotes)** | $15 once | Notes that slide in from screen edge. Quick capture without context-switching. | [One Thing](https://sindresorhus.com/one-thing) (free, single task in menu bar) |
| **Text Actions** | **[PopClip](https://www.popclip.app/)** | $15 once | Select text → popup with contextual actions (search, transform, send to apps). "How did I live without this." | — |
| **Link Router** | **[Velja](https://sindresorhus.com/velja)** | Free | Click a link → choose which browser/app opens it. Essential for multi-browser setup. | [Finicky](https://github.com/johnste/finicky) (free/OSS, rule-based) |

---

## Tier 4: Media & Content

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Screenshots** | **[CleanShot X](https://cleanshot.com/)** | $29 once | Scrolling capture, annotation, OCR, recording, GIF, cloud upload. Replaces 5 tools. nikiv uses it. | [Shottr](https://shottr.cc/) (free, lightweight), [Xnapper](https://xnapper.com/) ($15, beautifies screenshots) |
| **Video Player** | **[IINA](https://iina.io/)** | Free/OSS | Native macOS, hardware-accelerated, trackpad gestures, PiP. Feels Apple-made. nikiv uses it. | [VLC](https://www.videolan.org/vlc/) (free, plays everything) |
| **Music** | **[Spotify](https://www.spotify.com/)** | Subscription | Cross-platform, better discovery. Apple Music if all-in on Apple ecosystem. | [Swinsian](https://swinsian.com/) ($25, local FLAC/DSD files) |
| **PDF** | **[Skim](https://skim-app.sourceforge.io/)** | Free/OSS | Fast, great annotations. Preview handles 80% of cases already. | [PDF Expert](https://pdfexpert.com/) ($80/yr, editing/signing) |
| **Image Editing** | **[Affinity Photo 2](https://affinity.serif.com/photo/)** | Free (personal) | Photoshop-class, now free for individuals. Layers, masks, RAW, batch. | [Pixelmator Pro](https://www.pixelmator.com/pro/) ($50, ML-powered, Mac-native) |
| **Torrents** | **[qBittorrent](https://www.qbittorrent.org/)** | Free/OSS | Built-in search, IP filtering, VPN kill-switch, RSS feeds. | [Transmission](https://transmissionbt.com/) (free, simpler) |
| **RSS** | **[NetNewsWire](https://netnewswire.com/)** | Free/OSS | Native Swift, syncs across Apple devices. Perfect at $0. | [Reeder](https://reederapp.com/) ($10, prettier typography) |
| **Dictation** | **[Superwhisper](https://superwhisper.com/)** | Free / $8/mo | Voice-to-text anywhere on your Mac — the dictation interface you'll actually use. Local Whisper models, works in any app, natural speech. Life-changing for long-form input. | [Aiko](https://sindresorhus.com/aiko) (free, file transcription), [MacWhisper](https://goodsnooze.gumroad.com/l/macwhisper) (free tier) |
| **Screen Memory** | **[Screenpi.pe](https://screenpi.pe/)** | Free/OSS | Rewind.ai done right — local, private, open-source. Records your screen 24/7, search anything you've seen. All on-device, nothing leaves your Mac. Mesmerizing and life-changing. | [Rewind](https://www.rewind.ai/) (paid, cloud concerns) |

---

## Tier 5: Communication & Cloud

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **Messaging** | **iMessage** + **[Signal](https://signal.org/)** + **[Telegram](https://telegram.org/)** | Free | iMessage for Apple, Signal for encrypted, Telegram for communities. | [Texts.com](https://texts.com/) ($5/mo, aggregates all messengers) |
| **Video Calls** | **[Zoom](https://zoom.us/)** | Free tier | The standard. Everyone has it. | [Google Meet](https://meet.google.com/) (no install), FaceTime (Apple only) |
| **Cloud Storage** | **[iCloud](https://www.icloud.com/)** + **[Syncthing](https://syncthing.net/)** | $1-3/mo + Free | iCloud for ecosystem. Syncthing for P2P machine sync (no cloud). | [Proton Drive](https://proton.me/drive) (free, zero-knowledge encryption) |
| **File Sharing** | **[LocalSend](https://localsend.org/)** | Free/OSS | Cross-platform AirDrop (works with Android/Windows/Linux). | [NearDrop](https://github.com/grishka/NearDrop) (free, Google Quick Share for Mac) |

---

## Tier 6: Network & Security

| Category | Pick | Cost | Why it wins | Alternatives |
|----------|------|------|-------------|-------------|
| **VPN (Mesh)** | **[Tailscale](https://tailscale.com/)** | Free (100 devices) | WireGuard mesh VPN. Zero-config. Your Mac Mini is one click away. nikiv uses it. | [Headscale](https://github.com/juanfont/headscale) (free/OSS, self-hosted Tailscale) |
| **VPN (Privacy)** | **[Mullvad](https://mullvad.net/)** | $5.50/mo | No account (just a number), cash/crypto, audited, WireGuard. | [ProtonVPN](https://protonvpn.com/) (free tier) |
| **Firewall** | **[LuLu](https://objective-see.org/products/lulu.html)** | Free/OSS | See/control which apps connect to internet. 90% of Little Snitch for $0. Patrick Wardle / Objective-See. | [Little Snitch](https://www.obdev.at/products/littlesnitch/) ($59, more polished) |
| **Security Audit** | **[ParetoSecurity](https://paretosecurity.com/)** | Free/OSS | Menu bar app auditing your Mac: FileVault, firewall, Gatekeeper, etc. | — |
| **Webcam/Mic Guard** | **[OverSight](https://objective-see.org/products/oversight.html)** | Free/OSS | Alerts when mic/webcam are accessed. Objective-See suite. | — |
| **Backup** | **[Carbon Copy Cloner](https://bombich.com/)** | $40 once | Bootable clones + incremental. Does what Time Machine can't. | Time Machine (free, file-level), [Backblaze](https://www.backblaze.com/) ($99/yr, cloud) |
| **Encryption** | **[Cryptomator](https://cryptomator.org/)** | Free/OSS | Client-side encryption for iCloud/Dropbox/any cloud folder. | — |
| **DNS** | **[NextDNS](https://nextdns.io/)** | Free tier | Cloud DNS firewall with ad/tracker blocking. Set and forget. | [Pi-hole](https://pi-hole.net/) (self-hosted) |

---

## Tier 7: Quality of Life (Hidden Gems)

Small apps that punch above their weight. Install these after the essentials.

| App | Cost | What it does |
|-----|------|--------------|
| **[MonitorControl](https://github.com/MonitorControl/MonitorControl)** | Free/OSS | Control external monitor brightness/volume from Mac keyboard. Essential for non-Apple displays. |
| **[AltTab](https://alt-tab-macos.netlify.app/)** | Free/OSS | Windows-style Alt+Tab with full window previews. Huge upgrade over Cmd+Tab. |
| **[DockDoor](https://github.com/ejbills/DockDoor)** | Free/OSS | Hover Dock icons to see window previews. Should be built into macOS. |
| **[BoringNotch](https://github.com/TheBoringWorker/BoringNotch)** | Free/OSS | Turns MacBook notch into music controls, file drop zone, clipboard widget. |
| **[SlowQuitApps](https://github.com/dteoh/SlowQuitApps)** | Free/OSS | 1-second delay on Cmd+Q. No more accidental app quits. |
| **[Overkill](https://github.com/KrauseFx/overkill-for-mac)** | Free/OSS | Stops iTunes/Music from opening when plugging headphones/iPhone. |
| **[Mos](https://mos.caldis.me/)** | Free/OSS | Smooth scrolling for external mice. Reverses scroll direction per-device. |
| **[Mac Mouse Fix](https://macmousefix.com/)** | Free/OSS | Complete mouse customization: scroll, acceleration, buttons. Replaces vendor drivers. |
| **[Keka](https://www.keka.io/)** | Free/OSS | Archive tool. Handles every format (7z, RAR, ZIP, etc). |
| **[Command X](https://sindresorhus.com/command-x)** | Free | Adds Cmd+X cut-paste to Finder. By sindresorhus. How is this not built-in? |
| **[Pure Paste](https://sindresorhus.com/pure-paste)** | Free | Paste as plain text by default. No more pasting with formatting. By sindresorhus. |
| **[MeetingBar](https://github.com/leits/MeetingBar)** | Free/OSS | Next meeting in menu bar, one-click join. |
| **[OnlySwitch](https://github.com/jacklandrin/OnlySwitch)** | Free/OSS | All-in-one toggles: dark mode, AirPods connect, hide notch, keep awake, etc. |
| **[AlDente](https://apphousekitchen.com/)** | Free/Pro | Battery charge limiter. Keep battery at 80% when plugged in for longevity. |
| **[Suspicious Package](https://mothersruin.com/software/SuspiciousPackage/)** | Free | Inspect .pkg installers before running. See every file that will be installed. |
| **[Hazel](https://www.noodlesoft.com/)** | $42 once | Automated folder rules — move, rename, tag files by conditions. Set-and-forget file organization. |
| **[KeepingYouAwake](https://keepingyouawake.app/)** | Free/OSS | Prevent Mac from sleeping. One click in menu bar. |
| **[mas](https://github.com/mas-cli/mas)** | Free/OSS | Mac App Store from the terminal. `mas install`, `mas upgrade`. |

---

## Tier 8: Quick Look Plugins

Press Space in Finder to preview these file types properly. Install via `brew install --cask`:

| Plugin | Previews |
|--------|----------|
| **[QLStephen](https://github.com/whomwah/qlstephen)** | Plain text without extensions (Makefile, README, CHANGELOG) |
| **[QLMarkdown](https://github.com/sbarex/QLMarkdown)** | Markdown rendered as HTML |
| **[QLColorCode](https://github.com/anthonygelibert/QLColorCode)** | Source code with syntax highlighting |
| **[QLImageSize](https://github.com/Nyx0uf/qlImageSize)** | Image dimensions + file size overlay |
| **[QLVideo](https://github.com/Marginal/QLVideo)** | Video formats QuickTime can't handle |

---

## Sindresorhus Collection

One developer's free micro-apps that keep appearing across every list. Worth browsing [sindresorhus.com](https://sindresorhus.com). Highlights:

- **[Command X](https://sindresorhus.com/command-x)** — cut-paste in Finder
- **[Pure Paste](https://sindresorhus.com/pure-paste)** — plain text paste everywhere
- **[Velja](https://sindresorhus.com/velja)** — browser/app link router
- **[Lungo](https://sindresorhus.com/lungo)** — prevent sleep
- **[Aiko](https://sindresorhus.com/aiko)** — on-device transcription
- **[Dato](https://sindresorhus.com/dato)** — better menu bar clock + calendar
- **[One Thing](https://sindresorhus.com/one-thing)** — single focus task in menu bar
- **[Folder Peek](https://sindresorhus.com/folder-peek)** — quick folder contents from menu bar
- **[Shareful](https://sindresorhus.com/shareful)** — more sharing destinations in share sheets

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
| [CleanShot X](https://cleanshot.com/) | $29 |
| [Carbon Copy Cloner](https://bombich.com/) | $40 |
| [Keyboard Maestro](https://www.keyboardmaestro.com/) | $36 |
| [Dash](https://kapeli.com/dash) | $30 |
| [ForkLift](https://binarynights.com/) | $20 |
| [PopClip](https://www.popclip.app/) | $15 |
| **Total** | **~$170 once** |

### Optional subscriptions:
| App | Cost | Skip if... |
|-----|------|-----------|
| [Fantastical](https://flexibits.com/fantastical) | $57/yr | Use Apple Calendar or [BusyCal](https://www.busymac.com/busycal/) ($50 once) |
| [Mullvad VPN](https://mullvad.net/) | $66/yr | Don't need privacy VPN |
| **Total** | **~$123/yr max** |

---

## What NOT to Install

| App | Why not |
|-----|---------|
| **Copilot / Cline / Continue** | Claude Code replaces all AI coding assistants |
| **[Docker Desktop](https://www.docker.com/products/docker-desktop/)** | OrbStack is better in every way on Apple Silicon |
| **[Bartender](https://www.macbartender.com/)** | Privacy concerns after acquisition. Use Ice. |
| **[Alfred](https://www.alfredapp.com/)** (if using Raycast) | Pick one launcher, not both |
| **[1Password](https://1password.com/)** | Bitwarden is open-source, free, and good enough |
| **[iTerm](https://iterm2.com/)** (as daily driver) | Keep as backup. Ghostty + tmux is faster. |
| **Wave / Warp** | tmux + Ghostty > fancy terminal apps |
| **[Notion](https://www.notion.so/)** (for personal notes) | Obsidian owns your data locally. Notion doesn't. |
| **[Postman](https://www.postman.com/)** | Bruno is git-friendly, offline, no account needed |
| **[Charles Proxy](https://www.charlesproxy.com/)** | Proxyman is native, modern, free tier |
| **Any menu bar weather/clock** | Keep menu bar clean. Use [Dato](https://sindresorhus.com/dato) if you really need it. |

---

## Nikiv-Inspired Power Moves

Things worth stealing from [nikiv.dev/workflow](https://nikiv.dev/workflow):

1. **[Karabiner](https://karabiner-elements.pqrs.org/) as OS-level orchestrator** — not just remapping but the backbone of all app-switching via custom layers. He built a generator ([kar](https://github.com/nikivdev/kar)) for it.
2. **Dual-purpose keys** — every key does double duty (tap vs hold). Caps Lock tap = Esc, hold = Hyper.
3. **[Contexts](https://contexts.co/)** ($10) — window switcher bound to a hotkey for instant app jumping by typing app name.
4. **30+ parallel AI prompts** — treats coding as orchestration, not typing. [Claude Code](https://claude.com/claude-code) + Codex running simultaneously.
5. **Custom CLI tools** — his [flow](https://github.com/nikivdev/flow) (Rust) manages entire project lifecycle with task tracing for AI context.
6. **Four browsers, four purposes** — Safari (daily), Chrome Canary (dev), Safari TP (testing), Arc (social feeds).
7. **[SnippetsLab](https://www.renfei.org/snippets-lab/)** ($10) + **Snippety** — code snippets + text expansion with placeholders, especially for AI prompts.
8. **[Atuin](https://atuin.sh/)** — shell history sync across machines with encryption.

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

*Note: Some apps ([CleanShot X](https://cleanshot.com/), [Keyboard Maestro](https://www.keyboardmaestro.com/), [Things 3](https://culturedcode.com/things/), [ForkLift](https://binarynights.com/), [PopClip](https://www.popclip.app/), [Hazel](https://www.noodlesoft.com/), [Dash](https://kapeli.com/dash)) are purchased from their websites or the App Store directly.*
