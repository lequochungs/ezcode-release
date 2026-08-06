<div align="center">

# 🧠 EzCode

### A professional AI coding assistant for your desktop

**Chat • Steer • Auto-update • macOS & Windows**

[![macOS](https://img.shields.io/badge/platform-macOS-333333?logo=apple&logoColor=white)](#downloads)
[![Windows](https://img.shields.io/badge/platform-Windows-0078D6?logo=windows&logoColor=white)](#downloads)

**Download the latest release** → [Get EzCode](https://github.com/lequochungs/ezcode-release/releases/latest)

</div>

---

## 🚀 What is EzCode?

EzCode is a **professional AI coding assistant** that turns natural language into real work. Built on a modern React + Rsbuild interface, it wraps a powerful agent runtime so you can chat, plan, steer, and execute coding tasks right from your desktop — without leaving your workflow.

- 💬 **Chat naturally** — send prompts with file & image attachments
- ⚡ **Stream live** — see responses as they happen over WebSocket
- 🧠 **Steer the agent** — guide it mid-task, queue follow-ups, or stop instantly
- 📚 **Context-aware** — injection of project instructions (global + per-workspace)
- 🌐 **Multi-provider** — plug in the LLM providers you already use
- 🗂️ **Sessions** — every conversation is saved, easy to switch & resume
- 🎨 **Dark / Light mode** — comfortable in any environment

> **Auto-update included.** EzCode checks for new versions and installs them
> silently in the background — you always run the latest, most polished build.

---

## ✨ Feature Highlights

### 💬 Chat & Stream
- Send text prompts with drag-and-drop / paste / file picker attachments
- Real-time streaming responses over a persistent WebSocket
- Markdown rendering with syntax-highlighted code blocks
- Expandable tool calls so you can inspect what the agent is doing

### 🎛️ STEER — take control in real time
Real agents don't just answer — they *work*. While a task is running you can:

| Action | What it does |
|---|---|
| **Steer** | Send guidance mid-run (queued, applies after the current step) |
| **Follow-Up** | Queue input for after the agent finishes all its work |
| **Cancel Steer/Follow-Up** | Clear the pending queue |
| **Abort (Stop)** | Halt execution immediately |

### 📁 Workspaces
- Add any local folder / repo as a workspace
- Each workspace keeps its own agent context and settings

### 🧠 Prompt Injection (context rules)
- Two layers, stored as plain files you can edit from the UI:
  - **Global** — `~/.ezcode/AGENTS.md`, applies to every session
  - **Workspace** — `{workspace}/.ezcode/AGENTS.md`, applies to that repo
- Edit directly: **Settings → Prompt Injection → Edit → Save**

### 🗂️ Sessions & History
- Sessions are auto-saved to a local SQLite database
- Full session list in the sidebar — switch / resume / start new anytime

### ⚙️ Settings
- Provider management — add / remove your API keys
- Model selection + thinking level
- Prompt injection editor (global + workspace)
- Dark / Light theme toggle

### 🪵 App Logs
- Structured logging (debug / info / warn / error)
- Convenient log viewer right in the panel + bottom bar

---

## ⬇️ Downloads

Grab the installer for your platform from the [latest release](https://github.com/lequochungs/ezcode-release/releases/latest):

| Platform | File | Notes |
|---|---|---|
| **Windows** | `EzCode-<version>-setup.exe` | NSIS installer. Installs to the current user's apps folder; **auto-updates itself**. |
| **macOS (Apple Silicon / Intel)** | `EzCode-<version>-mac.dmg` | Drag EzCode into `Applications`. |
| **macOS (zip)** | `EzCode-<version>-mac.zip` | Also used by the built-in auto-updater for smooth delta updates. |

> 💡 **SmartScreen / Gatekeeper note:** binaries are not yet signed with an
> Apple Developer ID or a (EV) Windows certificate. On Windows choose
> **More info → Run anyway**; on macOS you may need to right-click → **Open**
> the first time. We're working on official code signing — once it's ready,
> future builds will install without these prompts.

---

## 🛠️ Getting Started

### Windows
1. Download **`EzCode-<version>-setup.exe`**
2. Run it — EzCode installs and launches automatically
3. Open **Settings**, add your API provider keys, and start chatting

### macOS
1. Download **`EzCode-<version>-mac.dmg`**
2. Open the DMG and drag **EzCode** into your `Applications` folder
3. First launch: right-click **EzCode** → **Open** (one-time Gatekeeper step)
4. Add your API keys in **Settings** and go

---

## 📖 Quick User Manual

### Starting a conversation
1. Launch EzCode from Start Menu / Applications.
2. Pick or create a **Workspace** (a folder you want to work in).
3. Type a prompt in the chat box and press **Enter** — the agent begins responding.

### Sending files & images
- **Drag & drop** a file/image into the chat, or
- **Click the attach button** (paperclip) / **paste** from clipboard.

### Steering a running task
- While the agent is working, use the **Steer** box to interject with new
  direction, or press **Stop** to abort immediately.
- Your **Follow-Up** messages are queued and sent automatically once the agent
  finishes the current turn.

### Managing sessions
- Sessions are saved automatically — close and reopen EzCode, everything's there.
- Use the **sidebar** to switch sessions, rename, or start a new one.

### Project-wide instructions
- Set global rules in **Settings → Prompt Injection → Global**.
- Set per-repo rules by adding a `.ezcode/AGENTS.md` file in your project.

### Updating
- EzCode checks for updates automatically on launch.
- When an update is available, you'll be prompted — choose **Download**, then
  **Restart now** when it's ready. It installs itself with no manual steps.

### Where your data lives
| Data | Location |
|---|---|
| Settings & prompts | `~/.ezcode/` |
| Sessions / database | `~/.ezcode/` (SQLite) |
| Workspace context | `.ezcode/AGENTS.md` inside each project |

---

## 🔒 Privacy

- Your API keys stay in your local settings — we never see them.
- Sessions and chat history are stored **locally** on your machine.
- The app talks directly to the LLM provider(s) you configure; no intermediary
  cloud that reads your conversations.

---

<div align="center">

**EzCode — your AI pair programmer, one click away.**

Questions, feedback, or issues? Open a GitHub Issue on this repository.

</div>
