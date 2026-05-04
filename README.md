# EU Climate Policy Q&A RAG Assistant

A retrieval-augmented generation (RAG) system that helps students and early-stage policy learners navigate EU climate policy documents quickly and accurately.

## The Problem

Students and early-stage policy learners struggle to understand EU climate policy because key information is spread across multiple complex and technical documents, such as the European Climate Law and related EU policy pages. This makes it difficult to extract accurate, connected, and trustworthy answers without misinterpretation.

## What It Does

A user asks a question like: *"How does the EU's 2030 climate target relate to the 2040 goal?"* The system uses an **Agentic RAG approach** to retrieve relevant passages from official documents, decides whether the information is sufficient, and returns a clear, concise answer with citations. If the documents do not contain enough information, the system either explicitly states that or supplements the answer using a web search tool with external sources.

## Setup

1. Install uv if you don't have it yet: https://docs.astral.sh/uv/getting-started/installation/

2. Clone this repository (or download the zip and extract it).

3. Create a `.env` file from the template and add your API key:

       cp .env.example .env

4. Install dependencies:

       uv sync

5. Start Jupyter:

       uv run jupyter notebook

## Notebooks

- `notebooks/01-setup.ipynb` - smoke test that confirms your environment works
- `notebooks/02-rag.ipynb` - a minimal RAG baseline you can adapt to your own data

## Data

Put your project data in the `data/` folder. See `notebooks/02-rag.ipynb` for how to load it.
