# H3 Video Generation Benchmark Data

Interactive benchmark matrix comparing generation times and visual quality across resolutions (0.1MP – 1.0MP) and durations (1s – 15s).

🔗 **Live Interactive Grid:** [View Web App](https://desktop4070.github.io/Optimized-H3-Gen-Times-V1/)

---

### ⚙️ Benchmark & Workflow Settings

| Category | Specification |
| :--- | :--- |
| **OS** | Windows 11 25H2 |
| **CPU** | Intel Core i9-12900K |
| **GPU** | NVIDIA GeForce RTX 5070 Ti 16GB (`sm_120`) |
| **Driver** | `610.74` |
| **System RAM** | 64GB DDR5 @ 5400 MT/s|
| **Pagefile.sys** | 65536 MB |
| **Software Environment** | PyTorch `2.13.0+cu130` · CUDA `13.0` |
| **ComfyUI Launch Flags** | `--windows-standalone-build --reserve-vram 2` |
| **Diffusion Model** | [`minimax_h3_fl2va_pruned_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/blob/main/diffusion_models/minimax_h3_fl2va_pruned_int8_convrot.safetensors) |
| **Text Encoder** | [`qwen3vl_32b_minimax_h3_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/blob/main/text_encoders/qwen3vl_32b_minimax_h3_int8_convrot.safetensors) |
| **Attention Node** | Comfy Kitchen Attention |
| **Turbo LoRA** | larryvrh's [`minimax_h3_turbo_v4_step600_ema.safetensors`](https://huggingface.co/larryvrh/MiniMax-H3-Turbo-Lora/blob/main/minimax_h3_turbo_v4_step600_ema.safetensors) @ 1.00 strength |
| **Sampler / Scheduler** | `er_sde` / `sgm_uniform` |
| **Steps** | 8 |

---

### Prompt

```yaml
integrated_multimodal_description: 
[Shot 1] Anime. Fantasy. A dense, sun-dappled forest clearing with towering, mossy trees. The young man in peasant clothing (S2) stands near an ancient tree trunk, looking disinterested as he rummages through a worn leather satchel. The young woman in a dirty and torn royal dress (S1) stands close by, gesturing out into the forest with animated frustration and pleading with him to pay attention, but he refuses to make eye contact. The camera pans slowly, tracking the vast wilderness of the forest and the friction between their postures. [Shot 2] The shot cuts to a close-up of the woman (S1). Her face is flushed with indignation, her eyebrows knit tightly, and her mouth forms an expression of sharp, wordless protest as her frustration reaches a breaking point. [Shot 3] The shot cuts to a close-up of a unique looking artifact that was pulled from the satchel, a GeForce RTX 5070 Ti; it visibly shines against his rough glove. [Shot 4] The shot transitions to a wider framing of the pair. The woman (S1) steps forward, clutching the fabric of her dress in an outburst of intense, visible emotion, while the man (S2) replies in a smug manner, snaps his satchel shut, and turns his back to walk away, leaving her standing alone as she watches him go.

overall_soundscape:
Quiet forest ambience. No other voices are heard.

non_diegetic_music:
N/A
