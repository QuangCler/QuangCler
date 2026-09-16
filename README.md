<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=24&pause=1200&color=58A6FF&center=true&vCenter=true&width=760&lines=AI+Engineer+%E2%80%94+Computer+Vision+%26+3D;Self-supervised+pre-training+at+ImageNet+scale;Viettel+AI+Race+2026+%E2%80%94+%235+Round+1+%E2%86%92+Final;Shipping+fast+models+with+TensorRT+%E2%9A%A1" alt="Typing SVG" />

# Tran Ngoc Quang

**AI Engineer · Computer Vision · 3D Reconstruction · Efficient Inference · LLM Systems**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-quangcler-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/quangcler/)
[![Kaggle](https://img.shields.io/badge/Kaggle-quangcler-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/quangcler)
[![Email](https://img.shields.io/badge/Email-quang.aidev%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:quang.aidev@gmail.com)
![Location](https://img.shields.io/badge/Ho_Chi_Minh_City-Vietnam-DA251D?style=flat-square)

</div>

---

### ⚡ What I do

- **Train** vision models from scratch — MAE / self-supervised pre-training on ImageNet-1K, multi-GPU, mixed precision, strictly controlled ablations.
- **Ship** them fast — ONNX → TensorRT, latency / throughput / VRAM measured per pipeline, running on anything from an RTX A5000 to a 4 GB laptop GPU.
- **Reconstruct** the 3D world — Gaussian Splatting pipelines at competition scale, with 14M+ Gaussians per scene and custom patches to the CUDA rasterizer.
- **Build** LLM products — agent backends with real-time CRM context, vision-LLM content pipelines, production-grade APIs.

### 🏆 Highlights

| | |
|---|---|
| 🥇 **Viettel AI Race 2026** | **#5 in Round 1** (BTS Digital Twin NVS, 76.25) → advanced to the **Final round** (large-scale urban NVS on H200) |
| 🚀 **+27% throughput** | Ghost + ConvMAE backbone: **1,331 img/s** TensorRT FP16 vs 1,046 for ConvMAE-Base, fewer params, on-par CASIA-WebFace accuracy |
| 🧪 **4 × 300-epoch** | ImageNet-1K MAE pre-training runs in one fair-comparison protocol (Ghost / Transformer / Mamba-2 / Bi-Mamba) |
| 🎯 **98.9%** | End-to-end Vietnamese license plate accuracy (YOLOv11 + CNN-BiLSTM-CTC, mAP@0.5 0.994) |

### 🔭 Research & open-source

| Project | What I built | Result |
|---|---|---|
| [**Inference-Efficient ConvMAE**](https://github.com/QuangCler/inference-efficient-convmae) | 4-arm controlled study of hybrid Conv/Transformer/Mamba backbones: MAE pre-training → linear probe → face fine-tuning (3 seeds) → ONNX/TensorRT benchmarking with bias control | Showed parameter count does **not** predict real throughput; selected backbone is faster *and* lighter under TensorRT at FP16 and FP32 |
| [**GhostConvMAE Face Demo**](https://github.com/QuangCler/ghostconvmae-face-demo) | Gradio app: 2 backbones × 5 tasks with live PyTorch ⇄ TensorRT switching on a 4 GB GTX 1650, per-forward latency & peak-VRAM accounting, automated self-test harness | 30/30 task × model × backend combos pass; TensorRT matches PyTorch top-1 everywhere |
| [**Face-Aware MAE**](https://github.com/QuangCler/Face-Aware-MAE-Landmark-Guided-Face-Pretraining) | Landmark-guided masking policy for face MAE pre-training (paper) | **−17.5%** identity-critical reconstruction error vs block-wise masking |
| [**Vietnamese LPR Benchmark**](https://github.com/QuangCler/QuangCler-Vietnamese-License-Plate-Recognition-Benchmark) | YOLOv5/v8/v11 × 3 OCR pipelines on real RTSP traffic data (8.2k + 3.7k images) | **98.9%** plate accuracy |
| [**GenBGM API**](https://github.com/QuangCler/Audio-BE) | Dockerized GPU service generating background music from chat context (MusicGen) | Runs on 4 GB VRAM |
| [**AI Talent Bot**](https://github.com/QuangCler/Telegram_AITalentBot_v2) | Telegram bot parsing PDF/DOCX CVs and scoring them against a JD with Gemini | — |

### 🛠 Production work — [TSC · Team Solo Code](https://github.com/TSC-teamsolocode)

- **3D Gaussian Splatting competition stack** — gsplat MCMC training sharded across 4×A5000 with shard merging; final-round recipe (multi-view gradient accumulation + regularization + fine-tuned SCUNet restoration) lifted the proxy score **+3.38**; audited and patched gsplat's CUDA projection against int32 intersection overflow at 21 MP full-res; reproducible Docker build for H200 (Hopper).
- **AI consulting console for an education provider** — Express/TypeScript + React; LLM agents with real-time CRM context injection, background suggestion & lead-summary pipeline cached in Redis, retry + circuit breaker on every upstream, scoped API keys and rate limiting.
- **Automated short-video pipeline** — MinIO asset indexing, ffmpeg frame sampling, vision-LLM tagging into SQLite FTS5, ETag-based incremental indexing (zero API calls on an unchanged library), 86 tests.
- **License control plane** — Ed25519-signed licenses and signed revocation lists with offline grace period, CLI + admin web UI.

### 🧰 Stack

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,opencv,docker,linux,ts,nodejs,express,react,redis,postgres,sqlite&perline=12" alt="stack" />
</p>

**Modeling** PyTorch · timm · Transformers · Mamba-SSM · gsplat · Ultralytics YOLO<br>
**Training** DDP · FP16/BF16 · MAE / self-supervised pre-training · linear probe & fine-tune protocols<br>
**Deployment** TensorRT · ONNX · CUDA · Docker · Gradio<br>
**LLM** Coze agents · Gemini · OpenAI-compatible vision models · prompt/persona pipelines<br>
**Backend** Python · TypeScript · Express · NestJS · Django · PostgreSQL · Redis · MinIO/S3

### 📄 Writing

- *Inference-Efficient ConvMAE for Universal Visual Recognition Tasks* — capstone report, FPT University, 2026
- *Identity-Aware Masked Autoencoding for Face Representation Pretraining: A Controlled Comparison of Region-Based Masking Strategies*
- *A Comparative Benchmark Study for Vietnamese License Plate Recognition*, 2026
