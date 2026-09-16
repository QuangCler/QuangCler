<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,45:1f6feb,100:8957e5&height=230&section=header&text=Tran%20Ngoc%20Quang&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=AI%20Engineer%20%E2%80%A2%20Computer%20Vision%20%E2%80%A2%203D%20Reconstruction%20%E2%80%A2%20LLM%20Systems&descAlignY=56&descSize=18" />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3200&pause=900&color=58A6FF&center=true&vCenter=true&width=780&lines=Pre-training+vision+models+at+ImageNet+scale;Making+them+fast+with+TensorRT+%E2%9A%A1;3D+Gaussian+Splatting+%E2%80%94+Viettel+AI+Race+2026+Finalist;Building+production+LLM+systems+at+TSC" alt="Typing SVG" />

<br/>

<a href="https://www.linkedin.com/in/quangcler/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://www.kaggle.com/quangcler"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" /></a>
<a href="mailto:quang.aidev@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://quangcler.github.io/ghostconvmae-face-demo/"><img src="https://img.shields.io/badge/Live_Demo_Page-181717?style=for-the-badge&logo=githubpages&logoColor=white" /></a>

</div>

<br/>

## 👋 hey, I'm Quang

I train vision models, make them fast, and ship them.

Most of my time goes into the unglamorous half of AI — taking a model from a paper to something that actually runs on real hardware. Multi-day pre-training runs, TensorRT engines that refuse to build, CUDA kernels that overflow once the images get big enough. Lately that has meant 3D Gaussian Splatting for **Viettel AI Race 2026** (made the final), inference-efficient ConvMAE backbones for my capstone, and LLM products with my team at **TSC**.

## ⚙️ What I actually do

<table>
  <tr>
    <td width="30%"><b>🧠 Train vision models</b></td>
    <td>Self-supervised / MAE pre-training at ImageNet scale, multi-GPU DDP, mixed precision, and ablations designed so the comparison is actually fair.</td>
  </tr>
  <tr>
    <td><b>⚡ Make them fast</b></td>
    <td>PyTorch → ONNX → TensorRT, FP16 vs FP32 profiling, measuring latency, throughput and VRAM per pipeline instead of trusting parameter counts.</td>
  </tr>
  <tr>
    <td><b>🛰️ Rebuild the world in 3D</b></td>
    <td>Gaussian Splatting with gsplat — sharded training across GPUs, ensemble fusion, camera-model plumbing, and patching the rasterizer when it breaks.</td>
  </tr>
  <tr>
    <td><b>🤖 Ship LLM products</b></td>
    <td>Agent backends with live CRM context, vision-LLM content pipelines, retries and circuit breakers, APIs that survive real traffic.</td>
  </tr>
  <tr>
    <td><b>🧱 Build the plumbing</b></td>
    <td>TypeScript / Express and Python services, PostgreSQL, Redis, S3 / MinIO, Docker — whatever the model needs to live in production.</td>
  </tr>
</table>

## 🔭 Featured projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>⚡ <a href="https://github.com/QuangCler/inference-efficient-convmae">Inference-Efficient ConvMAE</a></h3>
      Four hybrid backbones (Ghost · Transformer · Mamba-2 · Bi-Mamba), each MAE-pre-trained 300 epochs on ImageNet-1K and benchmarked under one fair protocol — PyTorch vs ONNX/TensorRT.
      <br/><br/>
      🎯 <b>Faster <i>and</i> lighter</b> than ConvMAE-Base under TensorRT, on-par face-ID accuracy
      <br/><br/>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
      <img src="https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white" />
      <img src="https://img.shields.io/badge/Mamba-6E40C9?style=flat-square" />
      <img src="https://img.shields.io/badge/DDP-555?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>🧑‍🚀 <a href="https://github.com/QuangCler/ghostconvmae-face-demo">GhostConvMAE Face Demo</a></h3>
      Two backbones × five tasks with a live <b>PyTorch ⇄ TensorRT</b> switch on a 4 GB GTX 1650 — per-forward latency, peak-VRAM accounting and an automated self-test harness.
      <br/><br/>
      🎯 <b>30 / 30</b> task × model × backend combos pass
      <br/><br/>
      <img src="https://img.shields.io/badge/Gradio-F97316?style=flat-square" />
      <img src="https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white" />
      <img src="https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🛰️ BTS Digital Twin — Viettel AI Race 2026</h3>
      Multi-backbone <b>3D Gaussian Splatting</b> for drone-captured telecom towers with SELECT-median ensemble fusion; final-round stack on H200.
      <br/><br/>
      🎯 <b>#5 in Round 1</b> (76.25) ➜ advanced to the <b>Final</b>
      <br/><br/>
      <img src="https://img.shields.io/badge/gsplat-111?style=flat-square" />
      <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" />
      <img src="https://img.shields.io/badge/4×A5000_→_H200-333?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>🚘 <a href="https://github.com/QuangCler/QuangCler-Vietnamese-License-Plate-Recognition-Benchmark">Vietnamese LPR Benchmark</a></h3>
      YOLOv5 / v8 / v11 × three OCR pipelines on real RTSP traffic-camera data (8.2k detection + 3.7k OCR images).
      <br/><br/>
      🎯 <b>98.9%</b> plate accuracy · mAP@0.5 <b>0.994</b>
      <br/><br/>
      <img src="https://img.shields.io/badge/YOLOv11-00FFFF?style=flat-square&logoColor=black" />
      <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
      <img src="https://img.shields.io/badge/CTC_OCR-555?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🙂 <a href="https://github.com/QuangCler/Face-Aware-MAE-Landmark-Guided-Face-Pretraining">Face-Aware MAE</a></h3>
      Landmark-guided masking that points MAE pre-training at identity-critical facial regions — controlled against random and block-wise masking.
      <br/><br/>
      🎯 <b>−17.5%</b> identity-critical reconstruction error
    </td>
    <td width="50%" valign="top">
      <h3>🎵 <a href="https://github.com/QuangCler/Audio-BE">GenBGM API</a> · 🤖 <a href="https://github.com/QuangCler/Telegram_AITalentBot_v2">AI Talent Bot</a></h3>
      Dockerized MusicGen service that scores chat conversations with background music on 4 GB VRAM · Gemini-powered bot that parses CVs and ranks them against a job description.
    </td>
  </tr>
</table>

## 🛠️ Production work · <a href="https://github.com/TSC-teamsolocode">TSC — Team Solo Code</a>

<table>
  <tr>
    <td width="50%" valign="top">
      <b>🎓 AI consulting console</b> <sub>for an education provider</sub><br/>
      LLM agents with real-time CRM context, background suggestion &amp; lead-summary pipeline, Redis cache, retry + circuit breaker, scoped partner APIs.
      <br/><sub>TypeScript · Express · React · PostgreSQL · Redis</sub>
    </td>
    <td width="50%" valign="top">
      <b>🎬 Automated short-video pipeline</b><br/>
      MinIO asset indexing → ffmpeg frame sampling → vision-LLM tagging into SQLite FTS5, ETag-incremental so an unchanged library costs zero API calls. 86 tests.
      <br/><sub>Python · ffmpeg · S3 · Vision LLM · Docker</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b>🧊 3DGS competition infrastructure</b><br/>
      Sharded gsplat MCMC training on 4×A5000, CUDA projection patch for int32 overflow at 21 MP, reproducible H200 build; final-round recipe <b>+3.38</b> points.
      <br/><sub>gsplat · CUDA · Docker · SCUNet</sub>
    </td>
    <td width="50%" valign="top">
      <b>🔐 License control plane</b><br/>
      Ed25519-signed licenses and signed revocation lists with an offline grace period — CLI plus admin web UI for delivered software.
      <br/><sub>Node.js · Ed25519 · JWT · SPA</sub>
    </td>
  </tr>
</table>

## 🧰 Tech stack

<div align="center">

**Modeling & training**<br/>
<img src="https://skillicons.dev/icons?i=python,pytorch,opencv,sklearn&theme=dark" /><br/>
<img src="https://img.shields.io/badge/TensorRT-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
<img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
<img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white" />
<img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
<img src="https://img.shields.io/badge/YOLO-111F68?style=for-the-badge" />
<img src="https://img.shields.io/badge/gsplat-222?style=for-the-badge" />
<br/><br/>
**Backend, data & infra**<br/>
<img src="https://skillicons.dev/icons?i=ts,nodejs,express,react,django,postgres,redis,sqlite,docker,linux,git&theme=dark" />

</div>

## 📜 Certifications

<table>
  <tr>
    <td>🧠 <a href="https://www.coursera.org/account/accomplishments/specialization/YS7JV6ONIOL4"><b>TensorFlow Developer Professional Certificate</b></a></td>
    <td><sub>DeepLearning.AI</sub></td>
  </tr>
  <tr>
    <td>🏭 <a href="https://www.coursera.org/account/accomplishments/specialization/FYJ40YBBNGUZ"><b>AI Enterprise Workflow Specialization</b></a> — model deployment &amp; AI in production</td>
    <td><sub>IBM</sub></td>
  </tr>
  <tr>
    <td>💬 <b>NLP</b> — <a href="https://www.coursera.org/account/accomplishments/records/UVXRJ8OY5JJL">Attention Models</a> · <a href="https://www.coursera.org/account/accomplishments/records/PPT9U5A79N1Q">Sequence Models</a></td>
    <td><sub>DeepLearning.AI</sub></td>
  </tr>
  <tr>
    <td>📊 <a href="https://www.coursera.org/account/accomplishments/records/Z3QTSMA0F6RD"><b>Machine Learning With Big Data</b></a></td>
    <td><sub>UC San Diego</sub></td>
  </tr>
  <tr>
    <td>🐳 <a href="https://www.coursera.org/account/accomplishments/records/PCINXA4G9T71"><b>Containers: Docker, Kubernetes &amp; OpenShift</b></a> · <a href="https://www.coursera.org/account/accomplishments/records/6GHP6W2NVZP3">Microservices &amp; Serverless</a></td>
    <td><sub>IBM</sub></td>
  </tr>
</table>

## 📄 Writing

- 📘 **Inference-Efficient ConvMAE for Universal Visual Recognition Tasks** — capstone report, FPT University, 2026
- 📗 **Identity-Aware Masked Autoencoding for Face Representation Pretraining** — a controlled comparison of region-based masking strategies
- 📙 **A Comparative Benchmark Study for Vietnamese License Plate Recognition**, 2026

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:8957e5,55:1f6feb,100:0d1117&height=120&section=footer" />
