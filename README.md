# 🩺 WoundAid AI

WoundAid AI is an open-source AI assistant that analyzes images of wounds and provides first aid suggestions. It uses a vision-language model (BLIP-2) to describe the injury and a large language model (Falcon-7B-Instruct) to suggest first aid — all completely free and runnable on Google Colab.

---

## 🔍 Features

- 📸 Upload wound or injury image
- 🤖 Auto-describe the wound using BLIP-2
- 💬 Get natural first aid suggestions from Falcon-7B-Instruct
- 🌐 100% free, open-source, and no paid API keys required
- 🚀 Easy to run on Google Colab with GPU support

---

## 📊 Architecture


---

## 🧠 Models Used

### 1. **BLIP-2 (Salesforce/blip2-opt-2.7b)**
- Role: Image captioning — converts uploaded image into wound description
- Link: [https://huggingface.co/Salesforce/blip2-opt-2.7b](https://huggingface.co/Salesforce/blip2-opt-2.7b)

### 2. **Falcon-7B-Instruct (tiiuae/falcon-7b-instruct)**
- Role: Large language model — takes caption and outputs treatment suggestion
- Link: [https://huggingface.co/tiiuae/falcon-7b-instruct](https://huggingface.co/tiiuae/falcon-7b-instruct)

---

## 📦 Requirements

Install these in your Colab notebook (they are included in the code already):

```bash
pip install -q transformers accelerate torch torchvision timm bitsandbytes
woundaid-ai/
│
├── README.md
├── woundaid_colab.ipynb     # Colab Notebook (optional)
├── requirements.txt         # Optional dependency file
└── sample_inputs/           # Sample wound images (optional)
