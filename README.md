# Pinn

> AI that stays out of sight.

**Why go to ChatGPT and copy-paste when you can just take a screenshot?**

Switching apps, copying text, pasting it in, waiting, copying the answer back — that is too much work. With Pinn you hit one shortcut, drag over anything on your screen, and the answer appears instantly. No switching apps. No copy-pasting. No back and forth. Just there on your desktop, any time you need it.

→ **[pinn.homes](https://pinn.homes)**

---

## about

Pinn is a desktop AI assistant that lives completely out of sight. There is no icon, no dock entry, no taskbar, no trace of it anywhere — until you need it. Hit a shortcut from any app and a dark glass chat window slides in. Ask a question, take a screenshot of anything on your screen, or drop in a file. Pinn reads it and answers immediately. Then dismiss it and it disappears completely.

It works over everything — video calls, games, fullscreen apps, even inside Lockdown Browser. No screen recorder on earth can capture it. Nobody on your Zoom call will ever know it is there.

Built by **Drex** as a faster, less disruptive alternative to browser-based AI. The idea is simple: the AI should come to you, not the other way around.

---

## what pinn can do

- **screenshot AI** — drag-select any part of your screen, Pinn reads it and helps instantly. No typing needed.
- **ask anything** — type a question from any app without switching windows
- **drop a file** — drag in an image or PDF and ask about it
- **invisible to recorders** — hidden from Zoom, Teams, Meet, OBS, and every screen capture tool
- **works in Lockdown Browser** — fully hidden, zero detection
- **chat history** — sessions saved locally, pick up where you left off
- **copy answer** — one click to copy any response
- **auto start** — launches silently on login
- **no account, no telemetry, free forever**

---

## download

| platform | file |
|---|---|
| macOS (Apple Silicon + Intel) | [Pinn-14-universal-mac.zip](https://github.com/DrexSkills/Pinn/releases/download/v1.0.14/Pinn-14-universal-mac.zip) |
| Windows 10/11 | [Pinn-14-Windows.exe](https://github.com/DrexSkills/Pinn/releases/download/v1.0.14/Pinn-14-Windows.exe) |

---

## how to use

### 1. install

**mac**
1. download `Pinn-14-universal-mac.zip` and unzip it
2. find `Pinn.app` in Finder
3. right-click it → Open (do this once to get past Gatekeeper)
4. click Open again when the popup asks

**windows**
1. download `Pinn-14-Windows.exe` and run it
2. click **More info** → **Run anyway** if Windows SmartScreen appears
3. Pinn starts silently — look for the icon in your system tray (bottom right)

---

### 2. summon pinn

Press `Cmd+Shift+P` on Mac or `Ctrl+Shift+P` on Windows from any app — fullscreen, video call, game, anything. The Pinn window appears. Press it again or hit `Esc` to dismiss.

---

### 3. ask a question

Type anything and press `Enter`. Pinn answers immediately. That is it.

---

### 4. screenshot anything

Hit the screenshot button or press `Space` while idle. Pinn hides itself, you drag-select any area of your screen, and Pinn comes back with an answer. Works on questions, code, errors, documents, spreadsheets — whatever is on your screen.

---

### 5. drop a file

Drag any image or PDF directly onto the Pinn window and ask about it.

---

## shortcuts

| key | action |
|---|---|
| `Cmd/Ctrl + Shift + P` | show / hide Pinn |
| `Space` (when idle) | instant screenshot |
| `Enter` | send message |
| `Shift + Enter` | new line |
| `Esc` | dismiss |

---

## how it stays hidden

- no dock icon or taskbar entry at the OS level
- `setContentProtection(true)` makes it invisible to all screen capture software
- process runs under a neutral system name — not listed as "Pinn" or "Electron"
- window passes through mouse events when idle
- on macOS: excluded from Mission Control, Cmd+Tab, and Spaces

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

Requires Node.js and npm.

---

## stack

- [Electron](https://www.electronjs.org/) — desktop shell
- [Groq API](https://groq.com/) — fast AI inference
- vanilla HTML / CSS / JS — zero frameworks

---

## version history

| version | notes |
|---|---|
| v1.0.14 | Pinn 14 — smarter screenshot AI, improved context awareness |
| v1.0.12 | dark glass UI, tray icon on Windows, copy button, Lockdown Browser support |
| v1.0.9 | screenshot + AI, sessions, settings panel |
| v1.0.6 | hotkey customisation, theme switcher |
| v1.0.3 | persistent chat history |
| v1.0.1 | first release |

---

built by Drex
