# 2M AI Suite: The Ultimate Cloud-Based Creative Toolkit 🚀
### 🛠️ Developed by: **[Arafat Ahmed Mubin](https://github.com/ArafatAhmedMubin)**
### 🌐 Brand: **2M**
---

## 🌟 Introduction
Welcome to the **2M AI Suite** — a complete collection of production-grade Jupyter Notebooks (`.ipynb`) fully optimised for **Google Colab T4** and **Kaggle T4 GPUs**.

Every notebook in this suite uses `device_map="auto"` (via HuggingFace `accelerate`) to intelligently distribute model layers across **GPU VRAM → System RAM → CPU**, eliminating out-of-memory crashes. All dependencies are pinned to the **latest versions** and installed automatically.

---

## 📂 The 2M Creative Directory

| Notebook | Primary Model | Key Features | Open |
| :--- | :--- | :--- | :--- |
| **🎬 Cloud Video Generator** | Wan 2.1-T2V/I2V-1.3B | Text-to-Video, Image-to-Video, Xformers, Frame Slider | [Open](./Cloud_Video_Generator.ipynb) |
| **🎨 FLUX Image Studio** | FLUX.1-schnell | 4-bit NF4 Quant, 1360px, Download Helper | [Open](./AI_Image_Generator_FLUX.ipynb) |
| **🎵 Advanced AI Music Studio** | Stable Audio Open + MusicGen + HTDemucs | 3-min tracks, Remix, 4-Stem Split | [Open](./Advanced_AI_Music_Studio.ipynb) |
| **🎙️ Advanced AI Voice Studio** | F5-TTS + Whisper | Zero-Shot Cloning, Speech-to-Speech, Download | [Open](./Advanced_AI_Voice_Studio.ipynb) |
| **🏗️ 3D Asset Factory** | FLUX + TripoSR | Text-to-3D, Image-to-3D, .GLB Export, Mesh Optimizer | [Open](./3D_Asset_Factory.ipynb) |
| **🤖 AI Agent Builder** | OpenRouter (5 Free Models) | Persona Designer, Multi-Model, Export Config | [Open](./AI_Agent_Builder.ipynb) |
| **🌐 AI Browser Agent** | Qwen 2.5 Coder 7B (4-bit) | LLM-driven Playwright Web Automation | [Open](./colab_agent.ipynb) |

---

## 🔥 Key Technical Highlights

### 🧠 Memory Optimization (No More Crashes!)
- **`device_map="auto"`** — Automatically distributes model layers across GPU VRAM, System RAM, and CPU.
- **4-bit NF4 Quantization** (`bitsandbytes`) — Compresses large models to fit on 16GB T4 VRAM.
- **`gc.collect()` + `torch.cuda.empty_cache()`** — Proactive memory cleanup after every generation.
- **Attention Slicing + Xformers** — Reduces peak VRAM usage during diffusion steps.

### 🌍 Environment Intelligence
Every notebook auto-detects whether it is running on **Colab**, **Kaggle**, or **Local** and prints a confirmation. Kaggle-specific notes (Internet toggle) are shown where relevant.

### 📦 Always Up to Date
All `pip install` commands use the `-U` (upgrade) flag, ensuring the latest stable versions of `diffusers`, `transformers`, `accelerate`, `bitsandbytes`, and `gradio` are always used.

### 🎛️ Gradio Web UIs
Every notebook ships a **multi-tab Gradio interface** with:
- Progress tracking (`gr.Progress(track_tqdm=True)`)
- Status text boxes for real-time feedback
- Download buttons (`gr.File`) for every output

---

## 🚀 Quick Start

1. **Open** any notebook in Google Colab or Kaggle.
2. **Enable GPU** — Runtime → Change runtime type → T4 GPU (Colab) or Settings → Accelerator → GPU (Kaggle).
3. **Run All Cells** — The first cell auto-detects your environment and installs all dependencies.
4. **Use the Gradio UI** — Click the generated public link to open the web interface.

---

## 🔗 Connect with the 2M Ecosystem
- 📖 **[2M Business Blogs](https://2mbusinessblogs.com)** — AI insights for the corporate world.
- 🔬 **[2M Future Facts](https://2mfuturefacts.com)** — Exploring the next frontier of technology.
- 💻 **[2M Dev's](https://2mdevs.com)** — Engineering resources and tutorials.

---
**© 2026 2M | All Rights Reserved**  
*Crafted with Passion by Arafat Ahmed Mubin*
