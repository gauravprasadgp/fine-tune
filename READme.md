# 🔍 Qwen3-Embedding Fine-Tuning for Semantic Similarity (with LoRA + PEFT)

This project demonstrates how to fine-tune [Qwen/Qwen3-Embedding-0.6B](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) using **LoRA adapters (via [PEFT](https://github.com/huggingface/peft))** for improved sentence embeddings on a semantic similarity task.

We aim to teach the model that **semantically similar sentences should produce similar embeddings** (high cosine similarity), while unrelated ones should not.

---

## 📦 Features

- ✅ Fine-tunes Qwen3-Embedding using [LoRA](https://arxiv.org/abs/2106.09685)
- ✅ Uses Hugging Face [`transformers`](https://github.com/huggingface/transformers), [`datasets`](https://github.com/huggingface/datasets), and `peft`
- ✅ Generates a custom dataset of 100 labeled sentence pairs (`similar` vs `unrelated`)
- ✅ Compares original vs fine-tuned model on cosine similarity
- ✅ Supports CPU, MPS (Apple), and CUDA (GPU)

---

## 🧠 Use Case

Ideal for applications like:
- Sentence similarity scoring
- Semantic search
- Duplicate detection
- Embedding-based clustering/classification
