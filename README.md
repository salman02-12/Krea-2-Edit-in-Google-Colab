# ⚡ Krea-2 Edit in Google Colab

This repository contains a streamlined, easy-to-use Google Colab notebook designed to run the **Krea-2 Turbo Q6_K GGUF** model for AI image editing. Powered by ComfyUI, this tool allows you to upload an existing image, provide text instructions, and seamlessly edit it. It even supports uploading a second reference image to guide the edit, all running for free on a Google Colab T4 GPU.

**🎥 Watch the Tutorial:** [How to Use](https://www.youtube.com/watch?v=soon)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/1XrSZDPq6OI7oL4EsC9V_UfCz2cXb9_oo?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salman02-12/Krea-2-Edit-in-Google-Colab/blob/main/Krea_2_Edit_CoinNoin.ipynb)
[![Get Pro](https://img.shields.io/badge/Get%20Pro-PayPal-blue?logo=paypal)](https://www.paypal.com/ncp/payment/96P3VY836FUUG)

---
<img src="./thumbnail.png" width="100%" />

## ✨ Features Supported in this Notebook

This notebook simplifies the complex setup of Krea-2 Edit into 3 automated cells:

1. **⚙️ Initialize Core Environment**: Installs the ComfyUI backend and the custom GGUF and Krea2Edit integration nodes required to run the architecture.
2. **📥 High-Speed Asset Downloader & LoRA Setup**: Automatically downloads the highly compressed `krea2_turbo-Q6_K.gguf` UNet, Qwen3-VL FP8 text encoder, and VAE using Aria2c for rapid fetching. It also downloads the default Krea2 Identity LoRA and allows you to upload custom LoRAs.
3. **🎨 Krea2Edit Image Generation**: The core editing engine featuring:
   * **Source Image Upload**: Upload the primary image you wish to edit.
   * **Second Reference Image (Optional)**: Upload a secondary image to guide the AI (e.g., matching a specific outfit or style).
   * **Text Instructions**: Use natural language to tell the AI what to change (e.g., "Change her outfit to a red raincoat").
   * **Krea2Edit Advanced Settings**: Fine-tune the edit with `REF_BOOST`, `GROUNDING_PX`, and `FIT_MODE` controls.
   * **Turbo Generation**: Generates edits rapidly using low step counts (e.g., 10 Steps, CFG 1.0).
   * **Auto-download**: Seamlessly save the final masterpiece directly to your device.

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure a **T4 GPU** is selected in your Colab menu.
3. Run **Cell 1** to initialize the ComfyUI core environment.
4. Go to **Cell 2** and run it to download all required models. You can also upload a custom LoRA here if desired.
5. Go to **Cell 3**:
   * Ensure `UPLOAD_SOURCE_IMAGE` is checked.
   * Check `UPLOAD_SECOND_REFERENCE` if you have a second image to guide the edit.
   * Type your edit command in the `EDIT_INSTRUCTION` box.
   * Hit the Play button and upload your image(s) when prompted.
   * The server will process the edit in the background, and your new image will appear below the cell!

## 🤝 Credits
* **Notebook Creator:** [@CoinNoin](https://www.youtube.com/@CoinNoin)
* **Base Model (GGUF):** [VantageWithAI / Krea-2-Turbo-GGUF](https://huggingface.co/vantagewithai/Krea-2-Turbo-GGUF)
* **Krea2Edit Nodes:** [lbouaraba / comfyui-krea2edit](https://github.com/lbouaraba/comfyui-krea2edit)
