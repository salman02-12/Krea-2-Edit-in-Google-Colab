# ⚡ Krea-2 Edit in Google Colab

This repository provides an easy-to-use Google Colab notebook to run the **Krea-2 Turbo Q6_K GGUF** model for AI image editing. Built on a ComfyUI backend, this tool utilizes the `comfyui-krea2edit` and GGUF nodes to allow lightning-fast, high-quality image modifications using text instructions and reference images on a free T4 GPU.

**🎥 Watch the Tutorial:** [How to Use](https://www.youtube.com/watch?v=soon)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/1XrSZDPq6OI7oL4EsC9V_UfCz2cXb9_oo?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/salman02-12/Krea-2-Edit-in-Google-Colab/blob/main/Krea_2_Edit_CoinNoin.ipynb)
[![Get Pro](https://img.shields.io/badge/Get%20Pro-PayPal-blue?logo=paypal)](https://www.paypal.com/ncp/payment/96P3VY836FUUG)

---
<img src="./thumbnail.png" width="100%" />

## ✨ Features Supported in this Notebook

The notebook is fully automated and organized into 3 simple steps:

1. **⚙️ Initialize Core Environment**: Installs ComfyUI, the `uv` package manager, and the custom `comfyui-krea2edit` and GGUF processing nodes.
2. **📥 High-Speed Asset Downloader & LoRA Setup**: Automatically uses Aria2c to fetch the heavily optimized `krea2_turbo-Q6_K.gguf` UNet, Qwen3-VL FP8 text encoder, Qwen VAE, and the default Krea2 Identity Edit LoRA. It also supports downloading or uploading extra `.safetensors` LoRAs.
3. **🎨 Krea2Edit Image Generation**: The core editing interface. Features include:
   * **Dual Image Uploads**: Upload a 'Source Image' to edit, and an optional 'Second Reference' image to guide the edit (like a specific face or outfit).
   * **Text Instructions**: Simply type what you want to change (e.g., "Change her outfit to a red raincoat").
   * **Krea2Edit Advanced Settings**: Fine-tune the `REF_BOOST`, `GROUNDING_PX`, and choose between `fit` or `crop` modes.
   * **Customizable Parameters**: Adjust Width, Height, Steps, CFG, Samplers (e.g., `euler`, `dpmpp_2m`), and Schedulers.
   * **Auto-download**: Automatically save the edited masterpiece to your computer.

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure a **T4 GPU** is selected.
3. Run **Cell 1** to initialize the ComfyUI core environment.
4. Run **Cell 2**. Select your `LORA_SOURCE` (None, Download from URL, or Upload from Computer), and hit Play to download all required models.
5. Go to **Cell 3**. 
   * Ensure `UPLOAD_SOURCE_IMAGE` is checked. If you have a reference image, check `UPLOAD_SECOND_REFERENCE`.
   * Type your editing instruction in the `EDIT_INSTRUCTION` box.
   * Adjust your resolution (Width/Height) and click Play.
   * When prompted, upload your image(s).
   * The ComfyUI server will process the edit in the background, and your new image will appear directly below the cell!

## 🤝 Credits
* **Notebook Creator:** [@CoinNoin](https://www.youtube.com/@CoinNoin)
* **Krea2Edit Node:** [lbouaraba / comfyui-krea2edit](https://github.com/lbouaraba/comfyui-krea2edit)
* **Base Model (GGUF):** [VantageWithAI / Krea-2-Turbo-GGUF](https://huggingface.co/vantagewithai/Krea-2-Turbo-GGUF)
