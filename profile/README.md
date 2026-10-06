# 🚀 GPU-Heater: Private, All-in-One Local AI Workstation

Turn your local GPU into a unified, privacy-first AI workspace. GPU-Heater consolidates text, deep reasoning, code generation, media synthesis, and local RAG into a single offline interface—powered directly by local engines like Ollama and ComfyUI, keeping your data strictly on-premise.

### Why GPU-Heater?
Running modern local AI typically means juggling disconnected browser tabs, brittle CLI scripts, and tangled ComfyUI node graphs. GPU-Heater unifies these disparate tools into a single coherent workstation, backed by an automated resource lock that intelligently schedules VRAM to prevent Out-of-Memory (OOM) crashes on consumer hardware.

### ✨ Core Capabilities

* 🧠 **Specialized Model Profiles:** Seamlessly switch between daily orchestration (`qwen3.8:27b`), deep chain-of-thought analysis (`qwq:32b`), and repository-scale coding (`qwen2.5-coder:32b`).
* 🎨 **Headless Multimodal Studio:** Execute pre-configured pipelines for Text-to-Image, Video (LTX-2), Outpainting, Audio/TTS, and 3D mesh reconstruction directly from chat—no manual node routing required.
* 📚 **Offline Knowledge & RAG:** Local document indexing (PDF, DOCX, XLSX, codebase) backed by ChromaDB, with zero external data telemetry.
* 💻 **Developer Tooling:** Native integrations for VSCode, JetBrains, and Neovim, featuring architectural blueprint mapping and inline refactoring.
* 🛡️ **Strictly Local Loopback:** Binds exclusively to `127.0.0.1:2004`—your prompts, source code, and media assets never leave your machine.

---

> ⚠️ **The "Heater" Reality:**  
> Running multimodal pipelines and heavy reasoning models on a single consumer GPU creates substantial compute load. GPU-Heater uses sequential VRAM offloading to keep workloads stable, but operations take minutes, not seconds. A fast NVMe swap/pagefile (32GB+) is strongly recommended.