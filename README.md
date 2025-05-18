
# arXivBot – RAG-Powered Research Paper Assistant

**arXivBot** is a research assistant tool that leverages **Retrieval-Augmented Generation (RAG)** and a fine-tuned **Falcon-7B** model to help users explore, summarize, and interact with academic papers (like those from arXiv). The entire prototype is implemented in a single Jupyter Notebook.

---

## Project Overview

With thousands of research papers published monthly, keeping up is tough. arXivBot solves this by:
- Using **dense vector retrieval** to find relevant document sections
- Feeding that context into a **fine-tuned Falcon-7B model**
- Generating **summaries and answers** to user queries

All logic — data loading, vectorization, querying, and generation — is written in one Jupyter Notebook.

---

## Features

-  Query research papers using semantic search (LlamaIndex)
-  Summarize papers or answer complex questions
-  RAG workflow integrated into a single notebook
-  Fine-tuned Falcon-7B with LoRA + 4-bit quantization for efficiency

---

##  Requirements

Install the following Python libraries:

```bash
pip install transformers llama-index sentence-transformers bitsandbytes accelerate
````

> You may also need:
>
> * `PyPDF2`, `faiss-cpu`, `huggingface_hub`, `langchain`, etc., depending on your setup

---

##  How to Use

1. **Open** the Jupyter Notebook: `arxivbot.ipynb`
2. **Run cells sequentially**:

   * Load and parse PDFs
   * Build vector index using LlamaIndex or FAISS
   * Fine-tune or load the Falcon-7B model
   * Enter your query and get the generated response

---


