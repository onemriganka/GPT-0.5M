# GPT-0.5m: character-Level GPT from Scratch



<img width="1024" height="1024" alt="gpt0 5m" src="https://github.com/user-attachments/assets/d2c23ca4-6688-48aa-ac45-2644731090b1" />



A **tiny GPT model ( 0.54M parameters)** built from scratch in **PyTorch** for educational purpose.  
This project demonstrates how to implement, train, and fine-tune a GPT-like Transformer on text data without relying on external frameworks.  

It includes:
- Training on **Alice in Wonderland** (character-level).
- **Text generation** from prompts.
- **Fine-tuning** on a small **Q&A dataset** for question answering.

---

## 🚀 Features

- **From Scratch Implementation**  
  Custom GPT architecture (embeddings, positional encoding, transformer blocks, causal self-attention, and output layer).

- **Character-Level Language Modeling**  
  Trained directly on characters, not words.

- **Text Generation**  
  Autoregressive generation with temperature sampling.

- **Fine-Tuning for Q&A**  
  Extended training on a handcrafted Alice Q&A dataset.

- **Lightweight Model**  
  Only **0.54M parameters**, trainable on a single Colab T4 GPU in minutes.

---

## 📂 Project Structure

```bash
GPT_0_5M.ipynb   # Main notebook (implementation + training + fine-tuning)
```

### Main Sections:
1. **Dependencies & Setup** – Install PyTorch and load text dataset.  
2. **Model Architecture** – BaseGPT with transformer blocks.  
3. **Training Loop** – Train on Alice in Wonderland.  
4. **Text Generation** – Generate new story-like text.  
5. **Fine-Tuning** – Adapt GPT to Alice Q&A dataset.  
6. **Evaluation** – Generate answers to test prompts.  
7. **Model Stats** – Training time & parameter count.  

---

## 📊 Training Details

- **Dataset:** Alice in Wonderland (Project Gutenberg) + custom Q&A.  
- **Block Size:** 128  
- **Embedding Dim:** 128  
- **Layers:** 4  
- **Heads:** 4  
- **Params:** ~0.54M  

**Training Times on Google Colab T4 GPU**  
- Base Model: ~11 minutes (50K steps)  
- Fine-Tuning: ~2 minutes (10K steps)  

---

## 📝 Example Outputs

### Generated Text (story continuation)
```
alice, “and we said to the little.
“i don’t like the look!” said the hedgehog...
...
```

### Generated Q&A
```
Q: What happens when Alice eats the cake labeled 'Eat Me'?
A: She grows very tall.
```

*(answers are imperfect due to small model size)*

---

## 🛠️ How to Run

1. Clone this repo:
```bash
git clone https://github.com/your-username/GPT-0.5M.git
cd GPT-0.5M
```

2. Open the notebook in Jupyter/Colab:
```bash
jupyter notebook GPT_0_5M.ipynb
```

3. Train the model and generate text/Q&A.

---

## 📖 What You’ll Learn

- Fundamentals of **Transformer architectures**.  
- How **GPT-style models** are trained with causal attention.  
- How to **fine-tune** a pretrained language model on a new dataset.  
- Insights into why **scaling up** matters for fluency & accuracy.  

---

## 🌟 Why This Repo is Amazing

This project is designed as a **learning playground**.  
It strips away the complexity of giant GPTs and shows the **core ideas in action**:  
from embeddings to attention to text generation.  

Perfect for students, ML beginners, and anyone curious about how GPTs are built.  

---

## 📌 Future Work

- Add **word-level** or **subword-level** tokenization.  
- Experiment with **larger models**.  
- Add **temperature/top-k sampling** for better generation.  
- Fine-tune on **bigger QA datasets**.  

---

## 📜 License

MIT License. Free to use and modify.  
