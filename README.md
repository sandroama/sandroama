<!-- Profile README for github.com/sandroama/sandroama. Numbers verified 2026-07-20
     against each project's committed docs/results/ artifacts — do not add a number
     here without a committed artifact behind it. -->

# Hi, I'm Sandro 👋

**I build efficient, grounded, multimodal AI systems** — models that are cheap to run, cite their
evidence, and are measured honestly. MS in Computer Science, Stony Brook University, 2026.

- 🔭 **Focus:** LLM efficiency (quantization, LoRA/DPO, distillation) · retrieval & citation grounding · on-device CV · causal inference
- 🧪 **How I work:** pre-register the question, measure on committed artifacts, report the result even when it's negative
- 📫 Reach me: lashaama@chamamama.com

---

## Featured projects

> Every headline traces to a committed measurement file in that project's `docs/results/`.
> Evidence labels are explicit: **real-data** = public benchmark, **synthetic** = seeded protocol proof, **CPU-measured** = real numbers, no GPU required.

| Project | What it is | Measured headline |
|---|---|---|
| **[finops-agent](https://github.com/sandroama/finops-agent)** | RAG + LoRA + DPO + quantization over SEC filings | **47.5% memory cut** from dynamic int8 (0.989 hidden-state overlap); **192× smaller FAISS index** at recall@10 parity — *CPU-measured* |
| **[graphrag-citations](https://github.com/sandroama/graphrag-citations)** | Entity-graph RAG with verifier-grounded citations | **+30.0pp citation precision** vs flat RAG on HotpotQA n=500 (95% CI [+26.4, +33.7]) — with the honest costs named: −8.8pp accuracy, −30pp recall — *real-data* |
| **[sceneiq](https://github.com/sandroama/sceneiq)** | Detection + tracking + depth + VLM QA on video | Tracking is the **+69pp accuracy win** (0.12 → 0.81, hand-labeled n=32) — *synthetic protocol proof; real-video corpus pending* |
| **[pricing-lab](https://github.com/sandroama/pricing-lab)** | Causal-first dynamic pricing (switchback vs naive A/B) | Under heavy spillover, naive A/B bias hits **82.5%**; a clustered Hájek switchback design holds it at **3.9%** — *synthetic DGP, seeded* |
| **[edge-vision](https://github.com/sandroama/edge-vision)** | RT-DETR + MobileSAM + INT8/TensorRT deployment | **−72.5% INT8 model size**; structured pruning **−78.8% size at 0.545× latency** — *CPU lane measured; GPU latency/power Pareto pending* |

*Master's thesis — **adaptive KV-cache quantization** (per-token bit allocation atop TurboQuant):
**−68.8% importance-weighted MSE** vs uniform at matched bits (95% CI, n=30 seeds, synthetic);
heavy-tail sweep goes **28 win / 2 tie / 0 loss** across token-count × tail × budget cells; real-model phase in progress.*

---

## What I can prove I can do

`PyTorch` · `Transformers` · `LoRA / DPO` · `Quantization (int8 / vector / scalar)` ·
`RAG (BM25 + dense + graph)` · `Citation grounding & verification` · `Detection / tracking / depth` ·
`Causal inference (ATE, SUTVA, switchback)` · `ONNX / TensorRT` · `FastAPI` · `Streamlit` ·
`pytest / CI` · `Pareto / cost-quality analysis`
