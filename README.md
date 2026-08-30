# Optimized H3 Video Generation Benchmark

Interactive benchmark matrix comparing generation times and visual quality across resolutions (0.1MP – 1.0MP) and durations (1s – 15s).

🔗 **Live Interactive Grid:** [View Web App](https://desktop4070.github.io/Optimized-H3-Gen-Times-V1/)

---

### ⚙️ Benchmark & Workflow Settings

| Category | Specification |
| :--- | :--- |
| **Driver / OS** | Driver `610.74` / Windows 11 |
| **GPU** | NVIDIA GeForce RTX 5070 Ti 16GB, `sm_120`) |
| **System RAM** | 64GB DDR5 |
| **Software Stack** | ComfyUI · PyTorch `2.13.0+cu130` · CUDA `13.0` |
| **Diffusion Model** | MiniMax H3 (`minimax_h3_fl2va_pruned_int8_convrot.safetensors`) |
| **Text Encoder** | Qwen3-VL 32B (`qwen3vl_32b_minimax_h3_int8_convrot.safetensors`) |
| **Attention** | Comfy Kitchen Attention |
| **Turbo LoRA** | larryvrh's `minimax_h3_turbo_4step_ema.safetensors` @ 1.00 |
| **Sampler / Scheduler** | `er_sde` / `sgm_uniform` |
| **Steps** | 8 |
