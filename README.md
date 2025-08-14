# Stable Diffusion Pipelines

This project is **Stable Diffusion** in `img2img`.  

## 🖼️ txt2img Pipeline

```mermaid
flowchart LR
    A2["Input Image<br/>(Encoded to Latent)"] --> B2["Add Partial Noise<br/>(strength parameter)"]
    B2 --> C2["U-Net Denoising<br/>+ Cross-Attention"]
    C2 --> D2["Decoder<br/>(Latent → Image)"]
