# Dialogue Text Summarization using a Fine-Tuned T5 Model

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/YOUR-REPO-NAME/blob/main/YOUR-NOTEBOOK-NAME.ipynb)

**Final Year Project** by Nivedha

## About

This project fine-tunes a pre-trained Transformer model (**T5-small**) to generate short summaries of two-person chat dialogues. It covers the full pipeline: data exploration, preprocessing, fine-tuning, evaluation with ROUGE, and an interactive Gradio demo.

## Dataset

[SamSum](https://huggingface.co/datasets/knkarthick/samsum): about 16,000 messenger-style dialogues, each paired with a human-written summary.

## Model

- Base model: `t5-small`
- Input prefix: `summarize: `
- Max input length: 512 tokens
- Max summary length: 64 tokens
- Epochs: 3, learning rate: 3e-4, batch size: 8

## Results

| Model | ROUGE-1 | ROUGE-2 | ROUGE-L |
|-------|---------|---------|---------|
| Base T5-small (no fine-tuning) | XX.XX | XX.XX | XX.XX |
| Fine-tuned T5-small | XX.XX | XX.XX | XX.XX |

*(Replace XX.XX with your scores from the notebook.)*

## How to Run

1. Click the **Open in Colab** badge above.
2. Set the runtime to GPU: **Runtime → Change runtime type → GPU**.
3. Click **Runtime → Run all**.
4. At the end, a Gradio link appears where you can type your own dialogue and get a summary.

## Project Pipeline

Load data → Explore → Preprocess and tokenize → Fine-tune T5 → Evaluate → Demo

## Demo

*(Add a screenshot of your Gradio demo here.)*

## Limitations and Future Work

- May struggle with very long dialogues or heavy slang.
- Future work: try a larger model (T5-base), train for more epochs, handle multi-person conversations.

## Tech Stack

Python, PyTorch, Hugging Face Transformers, Datasets, Evaluate (ROUGE), Gradio, Google Colab
