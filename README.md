<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║   RAJA HAMMAD NASEER  ·  AI/ML + FULL-STACK ENGINEER     ║
║   Building systems that actually ship                    ║
╚══════════════════════════════════════════════════════════╝
```

[![Portfolio](https://img.shields.io/badge/Portfolio-rajahammadnaseer.com-0A66C2?style=flat-square&logo=safari&logoColor=white)](https://www.rajahammadnaseer.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/6hammad9)
[![Hugging Face](https://img.shields.io/badge/🤗_HuggingFace-7_models-FFD21E?style=flat-square)](https://huggingface.co/HammadNaseer)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-Publications-00CCBB?style=flat-square&logo=researchgate&logoColor=white)](https://www.researchgate.net/profile/Raja-Hammad-Naseer)
[![Location](https://img.shields.io/badge/📍_Ilmenau-Germany-black?style=flat-square)](https://maps.app.goo.gl/ilmenau)

</div>

---

## `$ whoami`

**Machine Learning Intern @ Fraunhofer IOSB** · M.Sc. Computer & Systems Engineering @ **TU Ilmenau** · 2+ years shipping production AI, computer vision, and full-stack systems.

Not tutorials. Not demos. **Systems that run in the real world.**

- 🔋 Extending Amazon's Chronos foundation model for energy time-series forecasting @ Fraunhofer IOSB
- 🧠 Fine-tuned LLMs on consumer hardware → 7 models published on Hugging Face
- 🔍 Built a fully air-gapped semantic search engine for regulated industries
- 📷 Deployed multi-camera computer vision platforms across live installations
- 🚗 Built and raced a self-driving 1/10-scale car — autonomous overtaking, 1–4 cm tracking error
- 🌐 Shipped full-stack web products with Docker CI/CD owned solo, end to end

---

## `$ cat projects.txt`

<table>
<tr>
<td width="50%" valign="top">

### 🔋 Chronos for Energy Forecasting
**Fraunhofer IOSB — current role.** Profiling Amazon's Chronos, a transformer-based time-series foundation model, on energy-economic data: load, generation, electricity prices, weather. Measuring accuracy, robustness, and runtime, then designing architecture extensions adapted to how energy markets actually behave.

`PyTorch` `Time series` `Foundation models` `Python`

</td>
<td width="50%" valign="top">

### 🚗 QCar Autonomous Overtaking
**TU Ilmenau.** A self-driving 1/10-scale vehicle on a physical indoor track. Cartographer localisation, a CasADi/IPOPT model-predictive controller at 12.5 Hz on a Jetson, and RPLidar-based detection driving a behaviour state machine that overtakes a moving ROSbot 2 and returns to the reference line.

```
Tracking error → 1–4 cm over continuous laps
Control rate   → 12.5 Hz
```

`ROS2 Humble` `CasADi` `IPOPT` `Cartographer SLAM` `Nav2` `C++`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔒 Air-Gapped Semantic Search
**The problem:** A regulated client needed AI-powered document search. No external APIs. No cloud. Compliance-first.

**The build:** ONNX embedding service (3× faster than PyTorch CPU) + HNSW vector search in Redis Stack + cross-encoder reranker.

```
Recall  → top-30 in ~10ms   (Redis HNSW)
Rerank  → top-10 precision  (cross-encoder)
E2E     → ~2s on CPU
Outbound API calls → 0
```

`Python` `FastAPI` `sentence-transformers` `ONNX` `Redis`

</td>
<td width="50%" valign="top">

### 🧬 MediChat-AI — LLM Fine-Tuning
**The constraint:** 4 GB GPU. 1.1B parameter model. Production-quality output.

**The build:** Fine-tuned TinyLlama with QLoRA (4-bit NF4, 12.6M trainable params — 1.13% of the model). Grounded with a ChromaDB index of 19,725 WebMD Q&As so answers don't rely on what a 1B model happens to remember. Most-downloaded model I've published.

```
Training VRAM  → ~3 GB (fits an RTX 3050)
Quantised size → 1.17 GB (GGUF q8_0)
Training data  → 7,664 examples, 3,832 conditions
```

[![Model](https://img.shields.io/badge/🤗_Model_on-HuggingFace-FFD21E?style=flat-square)](https://huggingface.co/HammadNaseer/medichat-tinyllama-q8)

`PyTorch` `QLoRA` `bitsandbytes` `GGUF` `Ollama` `ChromaDB` `LangChain`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📷 EMACS — Multi-Camera Access Control
**Live across multiple sites.** Face recognition and whitelist-based access control. Owned the full pipeline: Roboflow labelling → YOLOv8 training → ONNX inference optimisation → concurrent backend handling several video feeds → React dashboard. Proof of concept to production.

`YOLOv8` `ONNX Runtime` `React` `Node.js` `Express` `MongoDB` `Docker`

</td>
<td width="50%" valign="top">

### 🚁 Drone MOT Research — TU Ilmenau
**Published, CCSE2026.** Real-time multi-object tracking benchmark on simulated UAV footage. ByteTrack vs Norfair on MOTA, ID-switch rate, and FPS, with the benchmark dataset published alongside it so the numbers can be checked, not just believed.

`YOLOv8` `ByteTrack` `Norfair` `Microsoft AirSim` `Python`

</td>
</tr>
</table>

<details>
<summary><b>More projects</b> — agents, PULAO vision models, web, data</summary>

<br>

**🤖 AI Debate Agent** — Dynamic tool use: live web-search grounding, chain-of-thought reasoning, structured argument/counter-argument output with citation tracking. `LangChain` `Gemini API` `Web Search API`

**📝 CoverCare** — Analyses a CV against a job posting and generates a tailored cover letter as PDF. Dual engine: Gemini 2.5 in the cloud, or Llama 3.2 locally via Ollama. `React` `Flask` `Gemini 2.5` `Llama 3.2`

**🎓 Campus Marketplace** — Student marketplace for TU Ilmenau: listings, search, filtering, admin panel, validated through real user interviews. [Live ↗](https://unimarket-xi.vercel.app) `React` `Node.js` `MongoDB`

**🛂 PULAO — Event Access Control Vision Stack** — Five ONNX models published for a person-detection → tracking → face-recognition access-control pipeline: YOLOv5m person detector, a lightweight face detector, ArcFace glintr100 embeddings, plus PPE compliance detection with GDPR-compliant anonymisation for factory floors.

**🌡️ TEC Cooling Control** — Published research. Modelled a thermoelectric cooling system as PT2 plus dead time, tuned a PID controller with anti-windup on Arduino. Steady-state error under 0.3 °C. [Paper ↗](https://www.researchgate.net/publication/405075772_Modeling_and_Temperature_Control_of_a_Peltier-Based_Cooling_Chamber)

**🔥 CertiRoute** — Heat-aware shift-timing tool for outdoor crews: reads street-level heat data, predicts how it moves through the day, and returns one recommended start time per site. [Live ↗](https://certiroute.streamlit.app/) `Python` `Streamlit` `Forecasting`

**🏭 WorkAI** — Real-time industrial monitoring dashboard; pose-estimation and face-recognition pipelines exposed as their own services rather than bolted into the app. `React` `Node.js` `MongoDB` `Docker`

</details>

---

## `$ pip list` + `$ npm list`

```python
ML_STACK = {
    "fine_tuning":   ["PyTorch", "QLoRA", "LoRA", "bitsandbytes", "TRL", "Hugging Face Transformers"],
    "deployment":    ["Ollama", "llama.cpp", "GGUF", "ONNX Runtime", "FastAPI"],
    "retrieval":     ["LangChain", "ChromaDB", "Redis Stack", "sentence-transformers", "RAG"],
    "vision":        ["YOLOv8", "ByteTrack", "ArcFace", "OpenCV", "ONNX", "Roboflow"],
    "autonomy":      ["ROS2", "Gazebo Sim", "Cartographer SLAM", "Nav2", "CasADi/IPOPT"],
    "data":          ["NumPy", "Pandas", "SciPy", "Matplotlib"],
}

WEB_STACK = {
    "frontend":      ["React", "Next.js", "TypeScript", "Tailwind CSS"],
    "backend":       ["Node.js", "Express", "FastAPI", "REST APIs", "WebSockets"],
    "databases":     ["MongoDB", "PostgreSQL", "Redis", "ChromaDB"],
    "devops":        ["Docker", "GitHub Actions", "GitLab CI/CD", "Linux"],
}
```

---

## `$ git log --oneline`

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=6hammad9&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e&icon_color=58a6ff)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=6hammad9&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e)

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=6hammad9&theme=github-compact&bg_color=0d1117&color=58a6ff&line=58a6ff&point=ffffff&hide_border=true)

</div>

---

## `$ cat status.txt`

```
Currently  →  ML Intern @ Fraunhofer IOSB · M.Sc. @ TU Ilmenau, Germany
Open to    →  Werkstudent / Internship (AI · ML · Full-Stack)
Languages  →  English C1  ·  German B1  ·  Urdu (native)
Available  →  Immediately
```

---

<div align="center">

**If you build things that matter, let's talk.**

[![Email](https://img.shields.io/badge/hammadnaseer2230@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:hammadnaseer2230@gmail.com)
[![Portfolio](https://img.shields.io/badge/rajahammadnaseer.com-0A66C2?style=flat-square&logo=safari&logoColor=white)](https://www.rajahammadnaseer.com/)

</div>
