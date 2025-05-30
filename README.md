# FaceDiffuser

Fine-tuning Stable Diffusion for photorealistic human face synthesis with LoRA

---

## Overview
This project fine-tunes a pretrained diffusion model—**Stable Diffusion**—to specialize in generating **high-fidelity human faces**. While Stable Diffusion is a powerful general-purpose model, its facial outputs often suffer from unrealistic structure, poor detail, and identity artifacts.

By using **LoRA (Low-Rank Adaptation)** and a subset of high-quality face images, we significantly enhance the model's ability to generate photorealistic and anatomically plausible faces.

---

## Technology Stack

- **PyTorch** – Core deep learning framework
- **Stable Diffusion v1.5** – Pretrained text-to-image base model
- **LoRA** – Lightweight fine-tuning approach with low memory overhead
- **FFHQ Dataset** – 7,000 high-resolution face images used for training

> 📌 *Note: Only a subset of 7,000 images from FFHQ was used. We expect further improvements with larger datasets and longer training schedules.*

---

## Results

**Comparison (FID ↓ is better):**

| Comparison            | FID Score |
|-----------------------|-----------|
| Real vs. Base         | 150.7     |
| Real vs. Fine-tuned   | 108.5     |
| Base vs. Fine-tuned   | 83.6      |

The fine-tuned model shows noticeable improvements in facial structure, sharpness, and coherence.

---

## Potential Downstream Applications

- 🎨 Avatar & character design for gaming, AR/VR, and social apps  
- 🖼️ Photographic restoration and upscaling  
- 💄 Virtual try-on (makeup, glasses, hairstyles)  
- 🧪 Data augmentation for facial recognition or landmark detection  
- 📚 Concept art and visual storytelling  
- 🧠 NPC generation in interactive fiction and virtual worlds
