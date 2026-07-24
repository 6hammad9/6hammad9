<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║   RAJA HAMMAD NASEER  ·  AI/ML + FULL-STACK ENGINEER     ║
║   Building systems that actually ship                    ║
╚══════════════════════════════════════════════════════════╝
```

[![Portfolio](https://img.shields.io/badge/Portfolio-rajahammadnaseer.com-0A66C2?style=flat-square&logo=safari&logoColor=white)](https://www.rajahammadnaseer.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/6hammad9)
[![Hugging Face](https://img.shields.io/badge/🤗_HuggingFace-Models-FFD21E?style=flat-square)](https://huggingface.co/HammadNaseer)
[![Location](https://img.shields.io/badge/📍_Ilmenau-Germany-black?style=flat-square)](https://maps.app.goo.gl/ilmenau)

</div>

---

## `$ whoami`

ML Research Intern @ **Fraunhofer IOSB** · M.Sc. Computer & Systems Engineering @ **TU Ilmenau** · 2+ years shipping production AI and full-stack systems.

Not tutorials. Not demos. **Systems that run in the real world.**

- 🧠 Fine-tuned LLMs on consumer hardware → published on Hugging Face
- 🔍 Built a fully air-gapped semantic search engine for regulated industries
- 📷 Deployed multi-camera computer vision platforms across live installations
- 🌐 Shipped full-stack web products with zero downtime

---

## `$ cat projects.txt`

<table>
<tr>
<td width="50%" valign="top">

### 🔒 Air-Gapped Semantic Search
**The problem:** A regulated client needed AI-powered document search. No external APIs. No cloud. Compliance-first.

**The build:** 3 microservices via Docker Compose — Node.js orchestration + FastAPI ONNX embedding service (3× faster than PyTorch CPU) + cross-encoder reranker. HNSW vector search in Redis Stack.

```
Recall  → top-30 in ~10ms   (Redis HNSW)
Rerank  → top-10 precision  (cross-encoder)
E2E     → ~2s on CPU
Outbound API calls → 0
```

`Node.js` `FastAPI` `sentence-transformers` `ONNX` `Redis`

</td>
<td width="50%" valign="top">

### 🧬 MediChat-AI — LLM Fine-Tuning
**The constraint:** 4 GB GPU. 1.1B parameter model. Production-quality output.

**The build:** Fine-tuned TinyLlama with QLoRA (4-bit, 1.13% trainable weights, ~3 GB VRAM). Found template memorisation at 87% token accuracy — fixed the dataset, not the metric. Deployed via Ollama + ChromaDB RAG.

```
Training VRAM → ~3 GB
Quantised size → 1.17 GB (GGUF q8_0)
Dataset → 28k WebMD Q&A pairs (restructured)
```

[![Model](https://img.shields.io/badge/🤗_Model_on-HuggingFace-FFD21E?style=flat-square)](https://huggingface.co/HammadNaseer/medichat-tinyllama-q8)

`PyTorch` `QLoRA` `Hugging Face` `ChromaDB` `FastAPI`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📷 EMACS — Multi-Camera CV Platform
**The build:** Face recognition access control system across live camera installations. Owned the full ML pipeline: Roboflow labelling → YOLOv8 training → hyperparameter tuning → ONNX inference optimisation → React dashboard.

`YOLOv8` `ONNX Runtime` `React` `Node.js` `Docker`

</td>
<td width="50%" valign="top">

### 🚁 Drone MOT Research — TU Ilmenau
**The build:** Real-time multi-object tracking benchmark on simulated UAV footage. ByteTrack vs Norfair on MOTA, ID-switch rate, and FPS — quantifying accuracy/latency trade-offs for onboard inference.

`YOLOv11` `ByteTrack` `Norfair` `Microsoft AirSim` `Python`

</td>
</tr>
</table>

---

## `$ pip list` + `$ npm list`

```python
ML_STACK = {
    "fine_tuning":   ["PyTorch", "QLoRA", "LoRA", "bitsandbytes", "TRL", "Hugging Face Transformers"],
    "deployment":    ["Ollama", "llama.cpp", "GGUF", "ONNX Runtime", "FastAPI"],
    "retrieval":     ["LangChain", "ChromaDB", "Redis Stack", "sentence-transformers", "RAG"],
    "vision":        ["YOLOv8/v11", "ByteTrack", "OpenCV", "ONNX", "Roboflow"],
    "data":          ["NumPy", "Pandas", "SciPy", "Matplotlib"],
}

WEB_STACK = {
    "frontend":      ["React", "Next.js", "TypeScript", "Tailwind CSS"],
    "backend":       ["Node.js", "Express", "FastAPI", "REST APIs"],
    "databases":     ["MongoDB", "PostgreSQL", "Redis", "ChromaDB"],
    "devops":        ["Docker", "GitHub Actions", "CI/CD", "Linux"],
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
Currently  →  M.Sc. @ TU Ilmenau, Germany
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
