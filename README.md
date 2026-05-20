# Note 🚧

This is an ongoing learning project. It is not yet a polished tool for other people to install and use.

The current goal is to build a small but realistic RAG system over a LaTeX academic paper, while learning as I do it.

# LaTeX Paper RAG Assistant 📄🔎

A simple Retrieval-Augmented Generation project for asking questions about a LaTeX academic paper.

This project is my first practical RAG system. Instead of using a generic PDF or website, I use a paper written in LaTeX because academic papers have structure: sections, equations, appendices, references, figures, and old drafts. The goal is to understand the full RAG pipeline in a small but realistic setting, starting from a simple notebook prototype and gradually making it more LaTeX-aware.

## What this project does

The project:

1. Loads `.tex` files from a LaTeX paper project.
2. Cleans obvious LaTeX noise such as comments.
3. Splits the paper into retrievable chunks.
4. Embeds the chunks.
5. Stores them in a local FAISS vector index.
6. Answers questions using retrieved paper chunks as context.
7. Prints the sources used for each answer.



## ⚠️ Very Very important privacy note ⚠️

Do not commit an unpublished paper to a public GitHub repository.

This repo ignores the `paper/` folder by default. Put your real Overleaf files there locally:

```text
paper/
├── main.tex
├── Appendix.tex
├── Images/
└── ...