# comfyui-workflows
### Production-Ready Generative AI Pipelines

A collection of specialized ComfyUI workflows optimized for high-end VFX tasks, including camera synchronization, cinematic relighting, and 4K upscaling.

[ComfyUI Workflows demo video] https://vimeo.com/manage/videos/1180167988

## 📁 Workflow Categories

### 🎥 Camera Control & Motion
* **SCAIL Motion Transfer:** Image-to-Video generation using **Wan 2.1 SCAIL** for precise pose and camera matching via driving video.
![GGVFX_Cam_SCAIL_Match_01](images/GGVFX_Cam_SCAIL_Match_01.png)
![GGVFX_Cam_SCAIL_Match_02](images/GGVFX_Cam_SCAIL_Match_02.jpg)

* **Spatial Re-projection:** Image-to-Image multi-angle generation.
  * Features a **Camera Angle Gizmo** for intuitive perspective control.
  * Powered by **Qwen Image Edit 2511**.
![GGVFX_Cam_Multiangle_01](images/GGVFX_Cam_Multiangle_01.png)
![GGVFX_Cam_Multiangle_02](images/GGVFX_Cam_Multiangle_02.png)

### 💡 Cinematic Relighting
* **Lighting Transfer:** Source-to-Target lighting plate transfer for consistent shot integration.
![GGVFX_Lite_Transfer](images/GGVFX_Lite_Transfer.png)

* **Dynamic Relighting:** Multi-angle lighting control via **Lighting Gizmo** nodes.
  * Utilizes **Qwen Image Edit 2509** for high-fidelity shadow and highlight reconstruction.
![GGVFX_Lite_Relight_01](images/GGVFX_Lite_Relight_01.png)
![GGVFX_Lite_Relight_02](images/GGVFX_Lite_Relight_02.png)

### 🛠 VFX Pipeline Utilities
* **4K Video Upscaling:** High-bandwidth video-to-video upscaling.
  * Uses **Nvidia RTX Video Super Resolution (VSR)**. *(Note: See documentation for essential post node install fix).*
![GGVFX_Util_Upscale4k](images/GGVFX_Util_Upscale4k.png)

* **Photorealistic Refinement:** Advanced Image-to-Image filtering using **Z-image Turbo** to enhance texture detail and material response.
![GGVFX_Util_Photoreal](images/GGVFX_Util_Photoreal.png)

* **VFX ControlNet Generation:** Video-to-video multi-control generation (Masks, Canny, Depth, and Normal).
![GGVFX_Util_ControlNets_01](images/GGVFX_Util_ControlNets_01.png)
![GGVFX_Util_ControlNets_02](images/GGVFX_Util_ControlNets_02.png)

---
*Note: These workflows are designed for professional VFX environments and have been tested on 24GB VRAM configurations.*