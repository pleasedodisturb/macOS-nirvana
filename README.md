# macOS Nirvana

**The opinionated guide to a perfect Mac setup.**

One pick per category. No "top 10" listicles. No affiliate links. Just the best tool for each job, cross-referenced from 30+ sources, battle-tested by actual daily use.

---

## The Problem

Every "awesome Mac apps" list gives you 200 options and zero decisions. You spend more time researching tools than using them. You install 15 apps that overlap, your menu bar looks like a Christmas tree, and you still can't remember the hotkey for anything.

This guide is different. It makes the decisions for you.

## The Idea

Your Mac should work like an instrument — every key has a purpose, every app has a role, nothing overlaps, nothing is wasted. The goal isn't to install the most apps. It's to install the *right* apps, wire them together, and build muscle memory that makes you fast.

The philosophy:

1. **Keyboard-first** — if you're reaching for the mouse, something is wrong
2. **Own your data** — local files, open-source tools, no vendor lock-in
3. **One tool per job** — pick it, learn it, master it
4. **Free > Paid > Subscription** — your wallet has limits, your taste doesn't
5. **AI lives in the terminal** — [Claude Code](https://claude.com/claude-code) is the brain, everything else is the body

## What's Inside

**[`MAC-HOLY-GRAIL.md`](./MAC-HOLY-GRAIL.md)** — the full stack, organized in 8 tiers:

| Tier | What | Examples |
|------|------|---------|
| 1. Core System | The foundation you install first | Raycast, Karabiner, AeroSpace, Bitwarden, Ice |
| 2. Development | Terminal, editors, dev tools | Ghostty + tmux, VS Code, Claude Code, OrbStack, Bruno |
| 3. Productivity | Daily drivers | Firefox + Safari, Obsidian, Things 3, Fantastical |
| 4. Media | Content consumption & creation | IINA, CleanShot X, Affinity Photo 2, qBittorrent |
| 5. Communication | Messaging, calls, cloud | Signal, Telegram, Zoom, Syncthing, LocalSend |
| 6. Security | Network, privacy, backup | LuLu, Tailscale, Mullvad, Carbon Copy Cloner |
| 7. Hidden Gems | Small apps, big impact | DockDoor, Command X, Pure Paste, BoringNotch |
| 8. Quick Look | Finder preview plugins | Markdown, source code, images, video |

Plus: a "What NOT to Install" blacklist, nikiv-inspired power moves, a Sindresorhus micro-app collection, cost breakdown, and a one-command install script.

## The Setup at a Glance

```
Ghostty (terminal)
  └── tmux (sessions)
        ├── Claude Code (AI brain)
        └── zsh + starship + fzf (shell)

Raycast .............. launcher, clipboard, snippets, calculator
Karabiner ............ Caps Lock = Hyper key, app hotkeys
AeroSpace ............ i3-style tiling window manager
VS Code .............. visual editor (Neovim for terminal)
Obsidian ............. knowledge base (local markdown)
Bitwarden ............ passwords (open-source, self-hostable)
OrbStack ............. Docker (fast, lightweight)
Firefox + Safari ..... dev browser + personal browser
```

## Cost

| | Amount |
|---|---|
| **Free/OSS** | 90% of the stack |
| **One-time purchases** | ~$220 (Things 3, CleanShot X, Keyboard Maestro, Dash, ForkLift, PopClip, Carbon Copy Cloner) |
| **Subscriptions** | ~$123/yr max (Fantastical + Mullvad — both optional) |

You can run the entire setup for **$0** using only the free tiers and open-source alternatives listed for every category.

## Quick Start

```bash
# Install Homebrew (if you haven't)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Core apps
brew install --cask raycast ghostty karabiner-elements obsidian \
  visual-studio-code firefox bitwarden iina cleanshot \
  fork bruno tableplus orbstack stats ice

# CLI tools
brew install tmux starship fzf bat neovim mise atuin httpie mas

# Security
brew install --cask lulu oversight cryptomator

# Quality of life
brew install --cask monitorcontrol alt-tab keepingyouawake keka slowquitapps

# Quick Look plugins
brew install --cask qlstephen qlmarkdown qlcolorcode qlimagesize qlvideo
```

Then read [`MAC-HOLY-GRAIL.md`](./MAC-HOLY-GRAIL.md) for the full breakdown, rationale, and workflow wiring.

## Standing on the Shoulders of Giants

This guide wouldn't exist without the incredible work of these people and projects:

### Curated Lists
- **[awesome-mac](https://github.com/jaywcjlove/awesome-mac)** by jaywcjlove — the most comprehensive macOS app list on GitHub (70k+ stars)
- **[awesome-macos](https://github.com/phmullins/awesome-macos)** by Patrick Mullins — beautifully curated macOS resources
- **[open-source-mac-os-apps](https://github.com/serhii-londar/open-source-mac-os-apps)** by Serhii Londar — the definitive open-source Mac app catalog
- **[awesome-macOS](https://github.com/iCHAIT/awesome-macOS)** by iCHAIT — another essential curated list
- **[my-mac-os](https://github.com/nikitavoloboev/my-mac-os)** by Nikita Voloboev — the original "here's my entire Mac setup" repo that inspired thousands

### Individuals
- **[Nikita Voloboev](https://nikiv.dev)** — the original inspiration. His [workflow](https://nikiv.dev/workflow), [wiki](https://wiki.nikiv.dev), and keyboard-driven philosophy shaped this guide's DNA. His approach to Karabiner layers, AI-assisted development, and tool unification is years ahead.
- **[Sindre Sorhus](https://sindresorhus.com)** — prolific creator of dozens of free, beautifully crafted Mac utilities (Command X, Pure Paste, Velja, Aiko, and many more). If a small Mac app "just works," there's a good chance he made it.
- **[Patrick Wardle](https://objective-see.org)** — security researcher behind the Objective-See suite (LuLu, OverSight, BlockBlock, KnockKnock). Free, open-source macOS security tools that should be on every Mac.
- **[Mitchell Hashimoto](https://mitchellh.com)** — creator of Ghostty, Vagrant, Terraform. Proof that one person can build tools that millions depend on.

### Communities
- **[r/macapps](https://reddit.com/r/macapps)** — the best subreddit for discovering Mac apps, with genuinely helpful discussions
- **[r/mac](https://reddit.com/r/mac)** — broader Mac community with regular "what apps do you use?" threads
- **[Hacker News](https://news.ycombinator.com)** — developer-heavy discussions that surface tools you won't find in mainstream articles
- **[Mac Power Users](https://talk.macpowerusers.com)** — forum of power users sharing detailed workflows and app recommendations

### Research & Articles
- [Builder.io — Best VS Code Extensions 2026](https://www.builder.io/blog/best-vs-code-extensions-2026)
- [Setapp — Must-Try Mac Tools 2026](https://setapp.com/app-reviews/must-try-mac-tools)
- [MacRumors — 10 Mac Apps Worth Trying 2026](https://www.macrumors.com/2025/12/24/10-mac-apps-worth-trying-in-2026/)
- [Mac Automation Tips — 20 Favorite macOS Apps 2025](https://macautomationtips.com/my-20-favorite-apps-2025/)
- [Wix Engineering — Must-Have Mac Apps + Reddit's Hidden Gems](https://medium.com/wix-engineering/must-have-mac-apps-in-2025-my-picks-reddits-hidden-gems-6add3883c09a)
- [TheSweetBits — The macOS Power Stack](https://thesweetbits.com/macos-power-stack-small-lifetime-apps-remove-big-friction/)

## How This Was Made

This guide was built in a single session using [Claude Code](https://claude.com/claude-code) — Anthropic's AI coding assistant running in the terminal. Claude researched 30+ sources, cross-referenced 4 major awesome-mac GitHub lists, analyzed Reddit and Hacker News threads, studied nikiv's complete setup, and distilled it all into opinionated picks.

The human provided the taste. The AI provided the throughput.

## Contributing

Found a better app for a category? Think something's wrong? Open an issue or PR. The rules:

1. **One pick per category** — if you're suggesting a replacement, explain why it's *better*, not just *different*
2. **Include cost** — free/OSS preferred
3. **Personal experience > hype** — "I've used this daily for 6 months" beats "this just launched and looks cool"
4. **No affiliate links** — ever

## License

[MIT](./LICENSE) — do whatever you want with this.

---

*"Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away."* — Antoine de Saint-Exupery
