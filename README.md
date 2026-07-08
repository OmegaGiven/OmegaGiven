# ABOUTME

I love open source. I love homelabing. I love self sustainability.

## OG-toolkit — rebuilding my whole desktop UX from scratch (WIP)

Not just a window manager config — a real toolkit. Every app that makes up
my desktop shares the same config, the same theming engine, and the same
low-level Wayland plumbing, instead of being five unrelated scripts glued
together. Change a color once, every app updates.

**[OG-toolkit](https://github.com/OmegaGiven/OG-toolkit)** — the shared
crates everything else is built on:
- `og-config` — one config schema, one source of truth, no per-app copies drifting out of sync
- `og-theme` — deterministic per-app color variance (adjacent windows tint slightly differently so you can tell them apart at a glance, without breaking the shared palette), gradient theming, instant propagation when you change a color anywhere
- `og-wayland` — a from-scratch cross-application drag-and-drop implementation (iced/winit ship *zero* Wayland DnD support — this opens a second raw protocol connection to make dragging a file out of the file manager into a browser actually work), plus a reusable layer-shell overlay bootstrap for effects like the notification popup

**The apps**, each its own repo, each themeable from one place:
- [og-settings](https://github.com/OmegaGiven/sway-settings-manager) — the whole suite's control panel
- [og-apps](https://github.com/OmegaGiven/linux-packages) — pacman/AUR/Flatpak store
- [og-files](https://github.com/OmegaGiven/OG-file-manager) — file manager with real cross-app drag-and-drop and a preview pane that doesn't rearrange the UI every time you click something
- [og-search](https://github.com/OmegaGiven/OG-system-search) — app launcher / instant `go/<alias>` shortcuts
- [og-notify](https://github.com/OmegaGiven/OG-notify) — themed notification effects (rain, glow, wind, sparkle) on a transparent full-screen overlay
- [og-links](https://github.com/OmegaGiven/OG-links) — the local `go/` redirect service backing og-search's shortcuts

**Next up: [og-bar](https://github.com/OmegaGiven/OG-bar)** — replacing waybar
with something built the same way, fixing the one thing waybar genuinely
can't do (actually centering bar content, on any screen edge) and fully
customizable live from a popout menu — no config file required.

Desktop: Sway · OS: Arch Linux

## My specific object 3d modeler (LIVE)
website: https://omegagiven.github.io/OG-3dmodeler/ 
- https://github.com/OmegaGiven/OG-3dmodeler

## Where I write my stories and such as I love writing Fantasy short stories (LIVE)
website: https://omegagiven.github.io/omega-stories/
- https://github.com/OmegaGiven/omega-stories

## CRM tool for small businesses (BETA Testing stage)
- https://github.com/OmegaGiven/OG-fulfillment

## Trying to build a suite to replace googles suite of software (WIP)
- v1: https://github.com/OmegaGiven/home-suite-home
- v2: https://github.com/OmegaGiven/OG-suite

## Go alias service (LIVE)
- https://github.com/OmegaGiven/go-alias-rust

## DB manager / api requester / inspector (WIP)
- https://github.com/OmegaGiven/OG-TestDesk
