# Claw-Dev-Modified
A local-first AI coding agent inspired by Claude Code, powered by Ollama (Gemma/Mistral) with zero API cost.
# ⚡ Claw Dev (Local Claude Code Clone)

A local-first AI coding agent inspired by Claude Code, built to run entirely on your machine using Ollama.

No API. No cost. Full control.

---

## 🚀 Features

- 🧠 Local LLM support (Gemma, Mistral, etc.)
- 💻 Terminal-based coding assistant
- 🛠 Built-in tool system for file interaction
- 🔁 Interactive REPL mode
- ⚡ Zero API dependency (runs fully offline)
- 🧩 Modular provider system (Anthropic, Gemini, Ollama)

---

## 🧠 How It Works
User Input → Agent → Provider → Local Model (Ollama) → Response


The project replaces cloud-based AI providers with a local model backend, enabling a fully offline AI agent experience.

---

## 📦 Tech Stack

- Node.js + TypeScript
- Ollama (local LLM runtime)
- Gemma / Mistral models
- CLI interface (tsx)

---

## ⚙️ Setup

### 1. Install dependencies

```bash
npm install

2. Install Ollama

Download: https://ollama.com

Run:

ollama pull gemma:27b
ollama serve

3. Configure environment

Create .env:

LLM_PROVIDER=ollama
OLLAMA_MODEL=gemma:27b
OLLAMA_BASE_URL=http://127.0.0.1:11434

4. Run the project
npm run dev -- --provider ollama

⚠️ Notes
Performance depends on your hardware
Large models (e.g. Gemma 27B) may be slow on low VRAM systems
Tool-calling is basic and can be extended
🔥 Future Improvements
Smarter tool usage
Memory + task planning
Multi-model switching
GUI interface
