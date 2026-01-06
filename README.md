# PRODIGY_GA
Fine-tune GPT-2 on custom text data using Hugging Face Transformers and PyTorch, with a modern, deprecated-free training pipeline.

1️⃣ GPT-2 Fine-Tuning

Fine-tune GPT-2 on custom text data and generate text.

Libraries: transformers, datasets, torch

Usage:

python gpt2_finetune.py


Creates train_data.txt automatically if missing.

Saves fine-tuned model and tokenizer in ./results.

Generates text from a user-defined prompt.

Tips:

Use larger datasets and more epochs for meaningful results.

Adjust block_size and per_device_train_batch_size for memory management.

2️⃣ Markov Chain Text Generator

Generate random text using a Markov chain from a text file.

Libraries: python (no extra libraries required)

Usage:

python markov_text.py


Uses alice.txt as the default source.

Generates 50-word random text (adjustable in script).

Tips:

Larger source text → more coherent results.

Can experiment with n-gram variations.

3️⃣ Stable Diffusion Image Generation

Generate images from text prompts using Stable Diffusion.

Libraries: torch, diffusers, transformers, Pillow

Usage:

python stable_diffusion.py


Saves images in generated_images/.

Works on CPU or GPU. GPU recommended for speed.

Can edit the prompt in the script to generate custom images.

Tips:

Enable Hugging Face authentication to access private models (optional).

Use smaller images if VRAM is limited.

4️⃣ Neural Style Transfer

Apply style from one image onto another using VGG19.

Libraries: torch, torchvision, Pillow, matplotlib, requests

Usage:

python neural_style_transfer.py


Input images can be URLs or local files.

Saves the stylized image as stylized_output.jpg.

Displays the output in Colab.

Notes:

GPU is recommended for faster optimization.

Image size affects runtime (smaller = faster).

Normalization improves quality: VGG19 expects mean/std
