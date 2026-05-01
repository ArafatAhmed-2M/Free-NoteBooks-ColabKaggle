<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0055FF&height=180&section=header&text=2M%20AI%20Suite&fontSize=56&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=The%20Ultimate%20Cloud-Based%20AI%20Creative%20Toolkit&descAlignY=58&descColor=CCE5FF" width="100%"/>

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-ArafatAhmed--2M-0055FF?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArafatAhmed-2M)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@ArafatAhmedMubin)
[![Colab](https://img.shields.io/badge/Google%20Colab-Ready-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com)
[![Kaggle](https://img.shields.io/badge/Kaggle-Ready-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://kaggle.com)

<br/>

> **Production-grade AI notebooks optimised for T4 GPUs — No crashes, No limits.**  
> Uses `device_map="auto"` to spread models across **GPU VRAM + RAM + CPU** automatically.

</div>

---

## ✨ What's Inside

<div align="center">

| &nbsp; | Notebook | Model | Key Features |
|:---:|:---|:---|:---|
| 🎬 | [**Cloud Video Generator**](./Cloud_Video_Generator.ipynb) | Wan 2.1-T2V / I2V-1.3B | Text-to-Video · Image-to-Video · Frame Slider · Xformers |
| 🎨 | [**FLUX Image Studio**](./AI_Image_Generator_FLUX.ipynb) | FLUX.1-schnell | 4-bit NF4 Quant · Up to 1360 px · PNG Download |
| 🎵 | [**Advanced AI Music Studio**](./Advanced_AI_Music_Studio.ipynb) | Stable Audio + MusicGen + HTDemucs | 3-min Tracks · Remix · 4-Stem Split |
| 🎙️ | [**Advanced AI Voice Studio**](./Advanced_AI_Voice_Studio.ipynb) | F5-TTS + Whisper | Zero-Shot Cloning · Speech-to-Speech · WAV Download |
| 🏗️ | [**3D Asset Factory**](./3D_Asset_Factory.ipynb) | FLUX + TripoSR | Text-to-3D · Image-to-3D · GLB Export · Mesh Optimizer |
| 🤖 | [**AI Agent Builder**](./AI_Agent_Builder.ipynb) | OpenRouter (5 Free LLMs) | Persona Designer · Export Config · Live Chat |
| 🌐 | [**AI Browser Agent**](./colab_agent.ipynb) | Qwen 2.5 Coder 7B (4-bit) | LLM-driven Playwright Web Automation |

</div>

---

## 🔥 Key Technical Highlights

<table>
<tr>
<td width="50%" valign="top">

### 🧠 Memory — No More Crashes
- **`device_map="auto"`** distributes layers across VRAM → RAM → CPU
- **4-bit NF4 Quantization** via `bitsandbytes` fits 7B+ models on 16 GB T4
- **`gc.collect()` + `torch.cuda.empty_cache()`** after every generation
- **Attention Slicing + Xformers** cut peak VRAM during diffusion

</td>
<td width="50%" valign="top">

### 🌍 Smart Environment Detection
```python
try:
    import google.colab
    ENV = "Colab"
except ImportError:
    ENV = "Kaggle" if os.environ.get(
        "KAGGLE_KERNEL_RUN_TYPE") else "Local"
```
Auto-detects **Colab / Kaggle / Local** on every run.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📦 Always Up-to-Date Packages
All install cells use the **`-U` upgrade flag**, so you always get the latest:
`diffusers` · `transformers` · `accelerate` · `bitsandbytes` · `gradio`

</td>
<td width="50%" valign="top">

### 🎛️ Full Gradio Web UIs
Every notebook includes a polished **multi-tab Gradio dashboard** with:
- 📊 Real-time progress tracking
- 💬 Status text feedback
- 📥 One-click download buttons

</td>
</tr>
</table>

---

## 🚀 Quick Start

```
1. Open any notebook link above in Google Colab or Kaggle
2. Enable GPU  →  T4 GPU (Colab: Runtime menu | Kaggle: Settings panel)
3. Run All Cells  →  environment auto-detected, all packages installed
4. Open the Gradio link  →  use the interactive web UI to generate!
```

> 💡 **Kaggle users:** Make sure **Internet** is turned ON in the right-side Settings panel before running.

---

## 📺 Connect

<div align="center">

[![YouTube](https://img.shields.io/badge/YouTube-%40ArafatAhmedMubin-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@ArafatAhmedMubin)
[![GitHub](https://img.shields.io/badge/GitHub-ArafatAhmed--2M-0055FF?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArafatAhmed-2M)

Subscribe on YouTube for tutorials, live demos, and 2M Suite updates!

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0055FF&height=100&section=footer&fontColor=FFFFFF" width="100%"/>

**© 2026 2M · All Rights Reserved**  
*Crafted with ❤️ by Arafat Ahmed Mubin*

</div>
