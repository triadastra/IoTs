# AI/ML in IoT: Edge Intelligence and TinyML

## Overview

The convergence of artificial intelligence and IoT — sometimes called **AIoT** — is
the defining trend of the mid-2020s. Rather than shipping raw sensor data to the
cloud, modern IoT systems increasingly run machine-learning inference **on or near
the device**. This shift is driven by demands for ultra-low latency, energy
efficiency, privacy, and offline operation.

The most influential development is **TinyML**: running ML models directly on
microcontrollers with kilobytes of RAM and milliwatt power budgets. Reflecting how
far the field has expanded, the **TinyML Foundation rebranded to the
[Edge AI Foundation](https://www.edgeaifoundation.org/) in late 2024**, signaling a
move from "tiny models on MCUs" to ML across the full spectrum of edge devices.

## Key Concepts

### The Inference Spectrum
- **TinyML** — Models on microcontrollers (e.g., Cortex-M, ESP32); KB of memory
- **Edge AI** — Models on capable edge SoCs and gateways (NPUs, edge GPUs)
- **Cloud AI** — Large models trained and served centrally; used for training and
  heavy analytics

### Core Techniques
- **Quantization** — Reduce model precision (e.g., FP32 → INT8) to shrink size/compute
- **Pruning** — Remove redundant weights/connections
- **Knowledge distillation** — Train a small "student" model from a large "teacher"
- **Federated learning** — Train across many devices without centralizing raw data,
  preserving privacy

### Common Toolchains
- **TensorFlow Lite for Microcontrollers**, **ONNX Runtime**, **Edge Impulse**,
  **STM32Cube.AI**, vendor NPU SDKs (Qualcomm, Nordic, NXP, ST)

## Current Status (2026)

### Market & Momentum
- The TinyML market was **~$1.53B in 2025**, projected to reach **~$9.65B by 2035**
  (20.2% CAGR) — [DataM Intelligence](https://www.datamintelligence.com/research-report/tinyml-market).
- **Silicon vendors are absorbing the ML tooling layer**: Qualcomm acquired
  **Edge Impulse** (2025) and Nordic acquired **Neuton.AI** (2025), making edge AI
  "part of the platform" — [Shawn Hymel](https://shawnhymel.com/3125/state-of-edge-ai-on-microcontrollers-in-2026/).
- **Ultra-low-power MCUs with on-device AI inference** became a baseline expectation
  in 2026, with dedicated NPU blocks appearing in mainstream microcontrollers —
  [Promwad](https://promwad.com/news/ultra-low-power-mcus-in-2026-ai-tinyml).

### Where Generative AI Fits
Large language models remain largely cloud-side, but **small language models (SLMs)**
and quantized models are pushing toward gateways and high-end edge devices for
natural-language interfaces, anomaly explanation, and local agents. The practical
2026 pattern is hybrid: tiny discriminative models on-device, larger generative
models in the cloud or at the regional edge.

## Use Cases

| Domain | On-device ML task |
|--------|-------------------|
| Predictive maintenance | Vibration/acoustic anomaly detection on the motor |
| Smart home | Keyword spotting, presence detection, no cloud round-trip |
| Healthcare | Arrhythmia detection on a wearable patch |
| Agriculture | Pest/disease image classification on solar sensors |
| Manufacturing | Visual defect detection at line speed |

## Benefits & Trade-offs

### Benefits
- **Latency** — Millisecond decisions, no network round-trip
- **Privacy** — Raw data (audio, video, biometrics) never leaves the device
- **Bandwidth/cost** — Only events/inferences are transmitted, not raw streams
- **Resilience** — Works offline / with intermittent connectivity

### Trade-offs
- Constrained accuracy vs. cloud models
- Model-update logistics across a deployed fleet (MLOps at the edge)
- Vendor lock-in as toolchains optimize for the owning company's silicon
- Debugging and observability are harder on distributed devices

## References & Citations

1. Edge AI Foundation (formerly TinyML Foundation) — [edgeaifoundation.org](https://www.edgeaifoundation.org/)
2. "From Tiny Machine Learning to Tiny Deep Learning: A Survey" (2025) — [arXiv 2506.18927](https://arxiv.org/pdf/2506.18927)
3. "Tiny Machine Learning (TinyML): Research trends and future application opportunities" (2025) — [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2590005625003017)
4. DataM Intelligence (2025). "TinyML Market Size & Forecast 2035" — [datamintelligence.com](https://www.datamintelligence.com/research-report/tinyml-market)
5. Shawn Hymel (2026). "State of Edge AI on Microcontrollers in 2026" — [shawnhymel.com](https://shawnhymel.com/3125/state-of-edge-ai-on-microcontrollers-in-2026/)

## Related Topics

- [Edge Computing](../applications/edge-computing.md)
- [Industrial IoT](../applications/industrial-iot.md)
- [Sustainability](./sustainability.md)
- [Data Management](../architecture/data-management.md)
- [Key Facts & Figures](../key-facts.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
