📰 **Project Overview – MediaEval 2025: NewsImages Task**

This project presents Team CVG-IBA’s submission for the MediaEval 2025 NewsImages Task, which challenges participants to generate or retrieve relevant and ethically appropriate images for online news articles. The goal is to balance relevance with non-photorealistic compliance—producing visuals that enhance article understanding without misleading realism.

We participated in both subtasks: (This repository contains code for retrieval only)

🔍 **Retrieval**

Methods Used: **SEEK** (for small subset) and **TRACE** (for large dataset).

Tech Stack: Fine-tuned CLIP model + FAISS indexing.

**Highlights**:

CLIP fine-tuned on news article-image pairs.

FAISS used for fast cosine similarity–based image lookup.

SEEK used CLIP directly on titles; TRACE utilized enriched embeddings with tags.

📊 Results

Evaluation Metric: Mean Reciprocal Rank (MRR), Precision@K, and Likert-scale ratings.

Top Score: VIVID achieved 3.401, outperforming both retrieval methods and the baseline.

| Dataset | Method      | Avg. Score |
| ------- | ----------- | ---------- |
| Small   | VIVID       | **3.401**  |
| Large   | PromptForge | 3.194      |
|         | TRACE       | 3.114      |


