# .pinn

**Invisible AI for your desktop. Press a shortcut, get an answer, disappear.**

No icon. No dock. No taskbar. No trace. Works over any app — video calls, games, fullscreen, even inside Lockdown Browser. Nobody knows it's there.

→ **[pinn.homes](https://pinn.homes)**

---

## what it does

Pinn lives silently on your desktop. Hit a shortcut from anywhere and a dark glass chat window appears — ask anything, get an instant AI answer, then dismiss it. It vanishes completely. No screen recorder can capture it. No one on your Zoom call can see it.

- runs hidden — no dock icon, no taskbar, no app switcher
- invisible to Zoom, Teams, Meet, OBS and every screen recorder
- works inside Lockdown Browser — fully hidden, no detection
- screenshot mode — drag select any part of your screen, ask AI about it
- copy answer in one click
- persistent chat sessions saved locally
- auto starts on login
- no account, no telemetry, free forever

---

## download

| platform | file |
|---|---|
| macOS (Apple Silicon + Intel) | [Pinn-1.0.12-universal-mac.zip](https://github.com/DrexSkills/Pinn/releases/download/v1.0.12/Pinn-1.0.12-universal-mac.zip) |
| Windows 10/11 | [Pinn-1.0.12-Windows.exe](https://github.com/DrexSkills/Pinn/releases/download/v1.0.12/Pinn-1.0.12-Windows.exe) |

---

## how to open

**mac**
1. unzip → find `Pinn.app` in Finder
2. right-click → Open
3. popup asks if you're sure → click Open again
4. press `Cmd+Shift+P` to summon it

**windows**
1. double click the `.exe`
2. click More info → Run anyway
3. Pinn icon appears in your system tray (bottom right)
4. press `Ctrl+Shift+P` to summon it

---

## shortcuts

| key | action |
|---|---|
| `Cmd/Ctrl + Shift + P` | show / hide Pinn |
| `Esc` | dismiss |
| `Enter` | send message |
| `Shift + Enter` | new line |

---

## how it stays hidden

- no dock icon or taskbar entry at the OS level
- `setContentProtection` prevents it from appearing in any screen capture
- process runs under a neutral name — not visible as "Pinn" or "Electron"
- window is set to ignore mouse events when idle — completely click-through
- on macOS: excluded from Mission Control, Cmd+Tab, and all workspace views

---

## build from source

```bash
git clone https://github.com/DrexSkills/Pinn.git
cd Pinn
npm install

# run in dev
npm start

# build for mac
npm run build:mac

# build for windows
npm run build:win
```

requires Node.js and npm.

---

## stack

- [Electron](https://www.electronjs.org/) — desktop shell
- [Groq API](https://groq.com/) — fast AI inference
- vanilla HTML/CSS/JS — zero frameworks

---

## version history

| version | what changed |
|---|---|
| v1.0.12 | removed onboarding, dark glass UI, tray icon on Windows, copy answer button, lockdown browser support |
| v1.0.9 | screenshot + AI, sessions, settings panel |
| v1.0.6 | hotkey customisation, theme switcher |
| v1.0.3 | persistent chat history |
| v1.0.1 | first release |

---

built by Drex
