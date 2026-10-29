## Hi, I'm Namratha 👋

**ML inference engineer**: I make deep learning models fast and small enough to deploy.
4+ years across autonomous driving (Volvo Cars) and edge AI, focused on **quantization (INT8 / FP8 /
mixed precision), TensorRT, and LLM serving with vLLM**.

- 🎓 MS Computer Science & Engineering (High-Performance Computer Systems), Chalmers University of Technology
- 🚗 Previously: Software Engineer at **Volvo Cars** (fleet-wide multi-sensor logging, NVIDIA Drive AGX Orin) and **KPIT Technologies** (AUTOSAR, ADAS ECUs)
- 🏁 Chalmers Formula Student Driverless: YOLO cone detection + Kalman tracking, bare-metal ECU firmware

### Selected work

| Project | What it shows | Result |
|---|---|---|
| [**Qwen2.5-7B in FP8: serving & cost**](https://github.com/namrathasanjay/qwen2.5-7b-fp8-serving) | FP8 quantization, perplexity, async load testing (TTFT / ITL / p99) of vLLM's OpenAI API on an L4, cost model | +1% perplexity, 36% faster decode, 28% cheaper chat serving; gain falls to 10% on long prompts |
| [**Phi-2: FP8, INT4 & mixed precision on H100**](https://github.com/namrathasanjay/phi2-fp8-quantization-vllm) | GPTQ W4A16 vs FP8 vs mixed precision in vLLM, per-layer sensitivity analysis, OpenAI-compatible serving | FP8 fastest (1,579 tok/s); keeping 3 sensitive layers in BF16 costs 3% |
| [**ViT-Base token pruning**](https://github.com/namrathasanjay/vit-token-pruning) | Training-free CLS-attention pruning, profiling, interleaved A/B benchmarking | 1.14× at −0.33 pts top-1; linear layers are 84% of GPU time |
| [**TensorRT INT8: semantic segmentation**](https://github.com/namrathasanjay/TensorRT-Quantization-SemanticSegmentation) | PTQ vs QAT on FCN-ResNet18 / Cityscapes | QAT keeps FP32 mIoU (62.5%) at 2.2× FP32 speed; PTQ loses 10.6 pts |
| [**TensorRT INT8: image classification**](https://github.com/namrathasanjay/TensorRT-Quantization-ImageClassification) | FP32/FP16/INT8 engines, layer sensitivity analysis | 3.5× lower latency, 3× smaller engine, −0.75 pts top-1 |

### Toolbox

**ML & inference:** PyTorch · TensorRT · ONNX · vLLM · HuggingFace Transformers · llmcompressor · GPTQ · timm · peft (LoRA) · torch.profiler · CUDA
**MLOps:** Docker · Kubeflow · GCP · AWS · CI/CD · Prometheus · Grafana
**Systems:** Python · C++ · Linux · CAN / Ethernet / AUTOSAR

### Contact

[LinkedIn](https://www.linkedin.com/in/namrathasanjay/)
