# comfyui-workflows
### Production-Ready Generative AI Pipelines

A collection of specialized ComfyUI workflows optimized for high-end VFX tasks, including camera synchronization, cinematic relighting, 4K upscaling, and production shot work integrating Foundry Nuke, Unreal Engine, and generative AI.

[ComfyUI Workflows demo video](https://vimeo.com/manage/videos/1180167988)
*(Covers March 2026 workflows — production shot work added April/May 2026 not yet included)*

---

## 🆕 What's New — April/May 2026

- **Shot Paint Outs & Replacements** — Wan VACE + Foundry Nuke + Beeble AI pipeline for production-grade clean plating and set element replacement
- **Background Replacement** — Unreal Engine grey box driving plates + ControlNet + Wan VACE, tested against Seedance 2; full comp in Nuke with bluescreen FG elements
- *(WIP)* **Long Establishing Shots** — Iterative generation beyond standard clip length using Unreal grey box plates, targeting Seedance 2.0
- *(WIP)* **Interactive Hologram Compositing** — Translucent, actor-reactive holographic elements via Nuke + ComfyUI

---

## 📁 Workflow Categories

### 🎬 Production Shot Work *(Added April/May 2026)*

* **Shot Paint Outs & Set Element Replacement**
  A production workflow for video clean plating, paint outs, and replacement of set elements using **Wan VACE** within ComfyUI, with final compositing in **Foundry Nuke**. 

*Developed and successfully tested in active VFX production*

![GGVFX_Pwf_Replace_01](images/GGVFX_Pwf_Replace_01.png)
![GGVFX_Pwf_Replace_02](images/GGVFX_Pwf_Replace_02.png)
![GGVFX_Pwf_Replace_03](images/GGVFX_Pwf_Replace_03.png)
![GGVFX_Pwf_Replace_04](images/GGVFX_Pwf_Replace_04.png)

* **Background Replacement with Unreal Engine Grey Box Driving Plates**
  End-to-end video background replacement pipeline using **Wan VACE**:
  * **Unreal Engine** for a grey box driving plate from a tracked bluescreen shot
  * Grey box plate drives **ControlNets** (used with generated first frame and reference set concepts, matte paintings, and GenAI reference frames)
  * Tested with grey box alone and with a pre-keyed FG plate over the grey box for tighter ControlNet guidance
  * Composited in **Foundry Nuke** with bluescreen FG elements, color correct and fixes
  * Tests include occluded geometry — handling views and surfaces not present in the first frame reference image, as revealed by camera movement
  * Results benchmarked against **Seedance 2** generations using same driving plate and reference images

*Developed in active VFX production, testing ongoing.*

![GGVFX_Pwf_BGGen_01](images/GGVFX_Pwf_BGGen_01.png)
![GGVFX_Pwf_BGGen_02](images/GGVFX_Pwf_BGGen_02.png)
![GGVFX_Pwf_BGGen_03](images/GGVFX_Pwf_BGGen_03.png)
![GGVFX_Pwf_BGGen_04](images/GGVFX_Pwf_BGGen_04.png)
![GGVFX_Pwf_BGGen_05](images/GGVFX_Pwf_BGGen_05.png)

* **Long Establishing Shots via Iterative Generation** *(WIP)*
  A workflow for generating video shots that exceed standard clip generation lengths. Uses Unreal Engine grey box driving plates, breaking a long shot into sequential iterations where each generation references previously generated frames. Final sections are comped together with cinematic and action elements added in post.

* **Interactive Hologram Compositing** *(WIP)*
  A video compositing workflow for translucent, interactive story elements — for example, in-world holograms that respond to actor performances. Combines **Foundry Nuke** compositing with **ComfyUI** generation passes to achieve physically plausible interactive light and translucency.

---

### 🎥 Camera Control & Motion

* **SCAIL Motion Transfer:** Image-to-Video generation using **Wan 2.1 SCAIL** for precise pose and camera matching via driving video.
![GGVFX_Cam_SCAIL_Match_01](images/GGVFX_Cam_SCAIL_Match_01.png)
![GGVFX_Cam_SCAIL_Match_02](images/GGVFX_Cam_SCAIL_Match_02.jpg)

* **Spatial Re-projection:** Image-to-Image multi-angle generation.
  * Features a **Camera Angle Gizmo** for intuitive perspective control.
  * Powered by **Qwen Image Edit 2511**.
![GGVFX_Cam_Multiangle_01](images/GGVFX_Cam_Multiangle_01.png)
![GGVFX_Cam_Multiangle_02](images/GGVFX_Cam_Multiangle_02.png)

---

### 💡 Cinematic Relighting

* **Lighting Transfer:** Source-to-Target lighting plate transfer for consistent shot integration.
![GGVFX_Lite_Transfer](images/GGVFX_Lite_Transfer.png)

* **Dynamic Relighting:** Multi-angle lighting control via **Lighting Gizmo** nodes.
  * Utilizes **Qwen Image Edit 2509** for high-fidelity shadow and highlight reconstruction.
![GGVFX_Lite_Relight_01](images/GGVFX_Lite_Relight_01.png)
![GGVFX_Lite_Relight_02](images/GGVFX_Lite_Relight_02.png)

---

### 🛠 VFX Pipeline Utilities

* **4K Video Upscaling:** High-bandwidth video-to-video upscaling.
  * Uses **Nvidia RTX Video Super Resolution (VSR)**. *(Note: See documentation for essential post node install fix.)*
![GGVFX_Util_Upscale4k](images/GGVFX_Util_Upscale4k.png)

* **Photorealistic Refinement:** Advanced Image-to-Image filtering using **Z-image Turbo** to enhance texture detail and material response.
![GGVFX_Util_Photoreal](images/GGVFX_Util_Photoreal.png)

* **VFX ControlNet Generation:** Video-to-video multi-control generation (Masks, Canny, Depth, and Normal).
![GGVFX_Util_ControlNets_01](images/GGVFX_Util_ControlNets_01.png)
![GGVFX_Util_ControlNets_02](images/GGVFX_Util_ControlNets_02.png)

---

## Changelog

| Date | Update |
|------|--------|
| April/May 2026 | Added Production Shot Work section: paint outs, BG replacement, and two WIP workflows |
| March 2026 | Initial release — camera control, relighting, upscaling, and utility workflows |

---

*Note: These workflows are designed for professional VFX environments and have been tested on 24GB VRAM configurations.*
> 📋 All reference images and footage used in these workflows are original, non-IP material used for testing only.