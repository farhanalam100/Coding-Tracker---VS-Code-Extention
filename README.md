# Coding-Tracker---VS-Code-Extention
Track how many hours you spend coding on your HCTG project. Live timer in the status bar + a beautiful weekly dashboard.
# ⏱ Coding Tracker — VS Code Extension

Track how many hours you spend coding on your HCTG project.  
Live timer in the status bar + a beautiful weekly dashboard.

---

## Features

- **Status bar timer** — shows `⏱ 2h 34m today` live while you code
- **Auto start/stop** — tracks time only when VS Code is in focus
- **Weekly dashboard** — click the status bar to open a bar chart of your last 7 days
- **Persistent storage** — your logs survive restarts

---

## Getting Started

### 1. Clone & install dependencies
```bash
git clone https://github.com/YOUR_USERNAME/coding-tracker
cd coding-tracker
npm install
```

### 2. Compile TypeScript
```bash
npm run compile
```

### 3. Run in VS Code
- Open the folder in VS Code
- Press `F5` to launch the Extension Development Host
- You'll see `⏱ 0s today` in the bottom status bar!

### 4. Open the Dashboard
- Click the status bar timer, OR
- Open Command Palette (`Ctrl+Shift+P`) → `Coding Tracker: Show Dashboard`

---

## How it works

| Event | Action |
|-------|--------|
| VS Code gains focus | Timer starts |
| VS Code loses focus | Timer pauses |
| Every second | +1 second added to today's log |
| Click status bar | Opens dashboard webview |

---

## HCTG Submission Info

**Title:** Coding Tracker  
**Description:** A VS Code extension that tracks how many hours you spend coding. Shows a live timer in the status bar and a weekly dashboard — perfect for logging your HCTG project hours.  
**Demo:** Record a short GIF using [ScreenToGif](https://www.screentogif.com/) showing the status bar + dashboard.

---

## Tech Stack
- TypeScript
- VS Code Extension API
- Local JSON storage (no internet required)
