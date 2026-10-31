# ⚡ Krea-2 Edit in Google Colab

This repository provides a streamlined Google Colab notebook designed for **Krea-2 Image Editing**. Powered by ComfyUI and the custom Krea2Edit nodes, this tool allows you to upload an image and modify it using simple text instructions. It utilizes highly optimized GGUF models so you can run it completely for free on a Google Colab T4 GPU.

**🎥 Watch the Tutorial:** [How to Use](https://www.youtube.com/watch?v=soon)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/1OPUso-UWTHyPprBVgINFncDqb0Bhs32I?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/salman02-12/Krea-2-Edit-in-Google-Colab/blob/main/Krea_2_Edit_CoinNoin.ipynb)
[![Get Pro](https://img.shields.io/badge/Get%20Pro-PayPal-blue?logo=paypal)](https://www.paypal.com/ncp/payment/96P3VY836FUUG)

---
<img src="./thumbnail.png" width="100%" />

## ✨ Features Supported in this Notebook

This notebook automates the complex setup of Krea-2 editing into 3 easy steps:

1. **⚙️ Initialize Core Environment**: Installs the ComfyUI backend, `uv` package manager, GGUF processing tools, and the essential `comfyui-krea2edit` custom nodes.
2. **📥 High-Speed Asset Downloader**: Automatically uses Aria2c to fetch the `krea2_turbo-Q6_K.gguf` UNet, Qwen3-VL FP8 text encoders, Qwen Image VAE, and a default Krea2 Identity LoRA. You can also download or upload your own custom LoRAs.
3. **🎨 Krea2Edit Image Generation**: The core editing interface. Features include:
   * **Source Image Upload**: Easily upload the original image you want to edit.
   * **Second Reference Upload**: Optionally upload a second image to use as a visual style or subject guide.
   * **Text Instructions**: Use the `EDIT_INSTRUCTION` box to tell the AI exactly what to change (e.g., "Change her outfit to a red raincoat.").
   * **Krea2Edit Settings**: Fine-tune the edit using the `REF_BOOST`, `GROUNDING_PX`, and `FIT_MODE` controls.
   * **Turbo Speeds**: Pre-configured to run efficiently with just 10 Steps and 1.0 CFG.

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure a **T4 GPU** is selected.
3. Run **Cell 1** to clone the environment and install all dependencies.
4. Run **Cell 2** to download the Krea-2 models and any optional LoRAs. 
5. Go to **Cell 3**. 
   * Ensure `UPLOAD_SOURCE_IMAGE` is checked. Check `UPLOAD_SECOND_REFERENCE` if you are providing a visual guide.
   * Type your desired change in the `EDIT_INSTRUCTION` text box.
   * Click Play. When prompted, upload your image(s).
   * The server will process the image in the background and display your newly edited image right below the cell!

## 🤝 Credits
* **Notebook Creator:** [@CoinNoin](https://www.youtube.com/@CoinNoin)
* **Krea2Edit Nodes:** [lbouaraba / comfyui-krea2edit](https://github.com/lbouaraba/comfyui-krea2edit)
* **Base Model (GGUF):** [VantageWithAI / Krea-2-Turbo-GGUF](https://huggingface.co/vantagewithai/Krea-2-Turbo-GGUF)
