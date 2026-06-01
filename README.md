# 🎨 AI Image Generation with Stable Diffusion

Generate stunning images from text prompts using the Stable Diffusion v1.5 model via Hugging Face Diffusers.

## 📸 Sample Output

> Prompt: *"A futuristic city at sunset"*

![Futuristic City](futuristic_city.png)

---

## 🛠️ Tech Stack

- Python
- Hugging Face Diffusers
- Stable Diffusion v1.5 (`runwayml/stable-diffusion-v1-5`)
- PyTorch
- Google Colab

---

## 🚀 How to Run

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/stable-diffusion-image-gen.git
cd stable-diffusion-image-gen
```

### 2. Install dependencies
```bash
pip install diffusers transformers accelerate torch huggingface_hub
```

### 3. Add your Hugging Face token
Get your token from [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens) and add it:
```python
from huggingface_hub import login
login(token="your_hf_token_here")
```

### 4. Run the notebook
Open `stable_diffusion.ipynb` and run all cells.

---

## 💡 How It Works

1. Loads the Stable Diffusion v1.5 pipeline from Hugging Face
2. Takes a text prompt as input
3. Runs the diffusion process to generate an image
4. Displays and saves the output as a PNG file

---

## 🔁 Try Your Own Prompts

Change the prompt in the notebook to generate anything:
```python
prompt = "A dragon flying over a mountain at night"
image = pipe(prompt).images[0]
image.save("output.png")
```

---

## 👤 Author

Built by GIFT — Cybersecurity & AI/ML Engineering Student, Torilo Academy (NEST Program)
