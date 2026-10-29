# Reshal (Alpha) — Your Local AI Terminal Agent

Hey! You are holding an early alpha version of **Reshal** — an AI agent that understands natural language and executes tasks directly on your operating system.

**What it can do right now:**
*   Create folders, write files, and manage your file system.
*   Execute complex command chains (e.g., `git init` -> create file -> commit).
*   Run fully locally via **Ollama** or connect to cloud APIs (**OpenRouter**, **OpenCode**).
*   It has memory and a brain-inspired architecture (Frontal Lobe plans, Parietal Lobe executes).

This is an **Alpha version**. The core engine works (200 automated tests passed!), but the user interface (TUI) is still a bit buggy and may lag.

---

## 🚀 How to Run (Tester Guide)

1. **Unpack** the `alpha` folder to any location.
2. **Install Ollama** (if you haven't already): https://ollama.com
   *   Open your terminal (cmd/PowerShell) and pull the model:
       `ollama pull qwen2.5-coder:7b`
3. **Run `ReshalaAI.Console.exe`** (Running as Administrator is recommended to avoid permission issues).
   *   *If Windows SmartScreen blocks it with a blue window, click "More info" -> "Run anyway". This is normal for new unsigned apps.*
4. The TUI interface will open.

---

## 🕹️ Usage (Commands & Tips)

Because the **TUI interface is currently unstable** (you might experience input lag or rendering bugs), I highly recommend using **Admin Mode** for stable testing.

**How to enter the stable mode:**
Type `/admin` and press Enter. You will drop into a classic, rock-solid CLI environment.

**Core Commands (work in both TUI and Admin):**
*   `/cloud` — list available cloud models.
*   `/cloud set <number>` — select a cloud model (e.g., `/cloud set 2`).
*   `/local` — list local models.
*   `/local set <number>` — select a local model (e.g., `/local set 3`).
*   `/language en` (or `ru`) — switch interface language.
*   `/admin` — switch to pure terminal mode (most stable).
*   `/exit` — quit the app.

**How to give tasks:**
Just type in plain English (or Russian). Example:
> *"Create a folder named my_project on my desktop, navigate into it, and create a main.py file"*

---

## 🐛 What we are looking for (Your Feedback)
Your job is to break it.
Let me know via the feedback form if:
*   The app hangs or crashes.
*   The TUI glitches out (overlapping text, messed up borders).
*   The agent does something completely wrong.
*   You have architectural ideas for improvement.

Thanks for testing! Together we'll make it perfect.