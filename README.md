# comfyui-workflows
### Production-Ready Generative AI Pipelines

A collection of specialized ComfyUI workflows optimized for high-end VFX tasks, including camera synchronization, cinematic relighting, and 4K upscaling.

## 📁 Workflow Categories

### 🎥 Camera Control & Motion
* **SCAIL Motion Transfer:** Image-to-Video generation using **Wan 2.1 SCAIL** for precise pose and camera matching via driving video.
![GGVFX_Cam_SCAIL_Match](images/GGVFX_Cam_SCAIL_Match_01.png)(images/GGVFX_Cam_SCAIL_Match_02.png)
* **Spatial Re-projection:** Image-to-Image multi-angle generation.
    * Features a **Camera Angle Gizmo** for intuitive perspective control.
    * Powered by **Qwen Image Edit 2511**.

### 💡 Cinematic Relighting
* **Lighting Transfer:** Source-to-Target lighting plate transfer for consistent shot integration.
* **Dynamic Relighting:** Multi-angle lighting control via **Lighting Gizmo** nodes.
    * Utilizes **Qwen Image Edit 2509** for high-fidelity shadow and highlight reconstruction.

### 🛠 VFX Pipeline Utilities
* **4K Video Upscaling:** High-bandwidth video-to-video upscaling.
    * Uses **Nvidia RTX Video Super Resolution (VSR)**. *(Note: See documentation for essential post node install fix).*
* **Photorealistic Refinement:** Advanced Image-to-Image filtering using **Z-image Turbo** to enhance texture detail and material response.
* **VFX ControlNet Generation:** Video-to-video multi-control generation (Masks, Canny, Depth, and Normal).

---
*Note: These workflows are designed for professional VFX environments and have been tested on 24GB VRAM configurations.*