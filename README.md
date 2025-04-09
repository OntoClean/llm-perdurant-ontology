# 🧠 LLM-Guided Perdurant Ontology Constructor

This repository implements a two-stage automated pipeline for constructing perdurant subsumption hierarchies using **Large Language Models (LLMs)**, guided by formal **meta-property constraints**.

---

## 🚀 Overview

The framework classifies and organizes events, processes, and states into taxonomic structures that are:

- ✅ Semantically accurate
- ✅ Ontologically sound
- ✅ Validated through inheritance constraints

It uses the following meta-properties:
- **Cumulativity**
- **Homeomericity**
- **Temporal Extent**
- **Agentivity**

---

## 🛠️ Features

### 🔹 Stage 1: Meta-Property Assignment & Upper-Tier Classification
- Uses few-shot prompts with OpenAI to assign meta-properties.
- Classifies events into one of six DOLCE-inspired categories (State, Process, Achievement, Accomplishment, Phenomenon, Phenomenal Boundary).
- Checks inheritance consistency with parent nodes before integration.

### 🔹 Stage 2: Intermediate Layer Grouping
- Identifies when multiple children under the same parent node should be grouped.
- Suggests intermediate layers based on LLM analysis.
- Validates the coherence of the grouping based on meta-property constraints.

---

## 📂 Folder Structure

```bash
.
├── pipeline.py               # Main pipeline code
├── .env                      # API key (not committed)
├── README.md                 # Project description
├── requirements.txt          # Python dependencies
└── images/                   # (Optional) Diagrams for taxonomy illustration
