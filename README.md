# H3 Video Generation Benchmark Data

Interactive benchmark matrix comparing generation times and visual quality across resolutions (0.1MP – 1.0MP) and durations (1s – 15s).

🔗 **Live Interactive Grid:** [View Web App](https://desktop4070.github.io/Optimized-H3-Gen-Times-V1/)

---

### ⚙️ Benchmark & Workflow Settings

| Category | Specification |
| :--- | :--- |
| **Driver / OS** | Driver `610.74` / Windows 11 |
| **GPU** | NVIDIA GeForce RTX 5070 Ti 16GB (`sm_120`) |
| **System RAM** | 64GB DDR5 @ 5400 MT/s|
| **Pagefile.sys** | 65536 MB |
| **Software Stack** | ComfyUI · PyTorch `2.13.0+cu130` · CUDA `13.0` |
| **ComfyUI Launch Flags** | `--windows-standalone-build --reserve-vram 2` |
| **Diffusion Model** | [`minimax_h3_fl2va_pruned_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/blob/main/diffusion_models/minimax_h3_fl2va_pruned_int8_convrot.safetensors) |
| **Text Encoder** | [`qwen3vl_32b_minimax_h3_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/blob/main/text_encoders/qwen3vl_32b_minimax_h3_int8_convrot.safetensors) |
| **Attention** | Comfy Kitchen Attention |
| **Turbo LoRA** | larryvrh's [`minimax_h3_turbo_v4_step600_ema.safetensors`](https://huggingface.co/larryvrh/MiniMax-H3-Turbo-Lora/blob/main/minimax_h3_turbo_v4_step600_ema.safetensors) @ 1.00 strength |
| **Sampler / Scheduler** | `er_sde` / `sgm_uniform` |
| **Steps** | 8 |
