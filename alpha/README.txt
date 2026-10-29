ReshalaAI Terminal — Alpha Build
=================================

How to run:
1. Double-click ReshalaAI.Console.exe (or run from terminal).
2. Windows will ask for Administrator rights — click "Yes".
3. The TUI interface will open automatically.

Requirements:
- Windows 10/11 (x64)
- Ollama installed (https://ollama.com) with at least one model pulled:
  ollama pull qwen2.5-coder:7b

Cloud (optional):
- Edit .env file and add your API key:
  OPENROUTER_API_KEY=sk-or-...
- Or use /provider wizard inside the app.

Commands (TUI):
  /cloud          — list cloud models from providers
  /cloud set 2    — apply model #2 to planner and chat
  /local          — list Ollama models
  /local set 3    — apply Ollama model #3
  /language en    — switch UI to English
  /language ru    — switch UI to Russian
  /admin          — switch to admin console mode
  /exit           — quit

Files:
  ReshalaAI.Console.exe  — main application (self-contained, no .NET needed)
  models.json            — configuration (models, cloud providers, tiers)
  .env                   — API keys (optional, for cloud features)
  Resources/             — embedded prompts and skills

Notes:
- All data (database, chat history) is stored in %LOCALAPPDATA%\ReshalaAI\
- If Ollama is not running, AI features will not work.
- The app requests Administrator rights for SendInput and GDI+ (mouse/keyboard control).