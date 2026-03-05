# LLM with Embeddings using Simple English Wikipedia

## Overview

This project demonstrates a simple pipeline for building a language model using the **Simple English Wikipedia dataset**.
The workflow includes extracting raw text from a Wikipedia XML dump, cleaning the text, preparing a dataset for training, and building a **GPT-style neural language model using PyTorch**.

The model learns to predict the **next token in a sequence**, forming the basis of a generative language model.

---

## Dataset

Dataset used: **Simple English Wikipedia XML Dump**

The raw XML file contains structured Wikipedia articles.
Text is extracted from `<text>` tags and processed into plain text suitable for training a language model.

Processing steps include:

* XML parsing
* text extraction
* cleaning and normalization
* dataset truncation for faster experimentation

---

## Project Workflow

The notebook follows these main steps:

1. **Extract Wikipedia text**

   * Parse XML file
   * Extract article text

2. **Text Cleaning**

   * Remove non-ASCII characters
   * Normalize whitespace
   * Remove unwanted symbols

3. **Dataset Preparation**

   * Save cleaned text
   * Limit dataset size for experimentation

4. **Tokenizer**

   * Use GPT-2 tokenizer for tokenization

5. **Model Architecture**

   * Transformer-based language model
   * Embedding layer
   * Attention layers
   * Feed-forward layers

6. **Training Setup**

   * PyTorch dataset and dataloader
   * Optimization and training loop

7. **Model Loading / Inference**

   * Load trained model
   * Generate predictions

---

## Technologies Used

* Python
* PyTorch
* Transformers
* WikiExtractor
* Regex
* XML parsing

---

## Key Libraries

* torch
* transformers
* tiktoken
* wikiextractor

---

## How to Run

Clone the repository:

```
git clone https://github.com/yourusername/simplewiki-gpt-embedding-model
```

Install dependencies:

```
pip install -r requirements.txt
```

Open the notebook:

```
jupyter notebook LLM_with_embedding.ipynb
```

---

## Author

Sangeetha KV
PhD Mathematics | Machine Learning | Data Science
