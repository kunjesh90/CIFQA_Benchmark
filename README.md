# CIFQA Benchmark

**Deterministic Tool-Grounded Multi-Agent LLM Framework for Calculation-Intensive Financial Query Answering (CIFQA)**

This repository contains the benchmark, implementation notebooks, evaluation resources, and supplementary material accompanying the manuscript:

> **Deterministic Tool-Grounded Multi-Agent LLM Framework for Calculation-Intensive Financial Query Answering (CIFQA)**

The repository enables researchers to reproduce the experiments reported in the manuscript and evaluate large language models (LLMs) on calculation-intensive financial reasoning tasks.

---

# Repository Contents

| File | Description |
|------|-------------|
| `Main_CIFQA_Notebook.ipynb` | Main implementation of the CIFQA framework. Upload this notebook along with the supporting files to Google Colab and execute all cells to reproduce the framework and experimental results. |
| `Ablation_Study_Notebook.ipynb` | Notebook for reproducing the ablation study presented in the manuscript. |
| `benchmark_questions.csv` | CIFQA benchmark containing all **126 benchmark queries**, their categories, and associated metadata. |
| `Benchmark_Answers_Manual_Calc.xlsx` | Manually verified ground-truth answers for all benchmark queries. |
| `CIFQA_Results.xlsx` | Complete evaluation results, including CIFQA outputs, agentic model results, and frontier LLM responses obtained using the standardized benchmark prompt. |
| `CIFQA_Ablation_Results.xlsx` | Results of the ablation study for benchmark queries applicable to each ablation experiment. |
| `Benchmark_Prompt.docx` | Standardized benchmark prompt used for evaluating frontier LLMs under a consistent experimental setting. |
| `Guidelines_pdf.pdf` | Financial product guideline document used as the retrieval knowledge source for policy and rule-based queries. |
| `int_rate_new.xlsx` | Structured interest-rate table used by the deterministic rate lookup engine during financial computation. |

---

# System Requirements

- Google Colab
- Python 3.10 or later
- Internet connection
- Valid API credentials for:
  - Groq
  - OpenRouter

---

# Running the Main CIFQA Notebook

## Step 1 – Configure API Keys

Open **Google Colab → Secrets** and create the following secret variables:

```
GROQ_API_KEY
Open_router_key
```

These credentials are required to access the LLM backends used by CIFQA.

---

## Step 2 – Upload Supporting Files

Upload the following files into the `sample_data` directory in Google Colab:

```
benchmark_questions.csv
Guidelines_pdf.pdf
int_rate_new.xlsx
```

---

## Step 3 – Execute the Notebook

Run all notebook cells sequentially.

The notebook automatically installs the required Python packages and reproduces the CIFQA framework experiments.

---

# Running the Ablation Study Notebook

## Step 1 – Configure API Keys

Create the following Google Colab secret variables:

```
GROQ_API_KEY
Open_router_key
```

---

## Step 2 – Upload Supporting Files

Upload the following files:

```
benchmark_questions.csv
Guidelines_pdf.pdf
int_rate_new.xlsx
```

---

## Step 3 – Execute

Run all notebook cells sequentially.

The notebook reproduces the ablation experiments reported in the paper.

---

# Benchmark

The released benchmark contains:

- **126 expert-designed financial queries**
- Manually verified ground-truth answers
- Query categories
- Supporting financial knowledge resources
- Evaluation prompt
- Experimental outputs reported in the manuscript

The benchmark covers:

- Calculation-intensive financial reasoning
- Interest-rate lookup
- Policy interpretation
- Edge-case financial scenarios

---

# Reproducibility

This repository contains all benchmark queries, manually verified ground-truth annotations, supporting financial resources, and evaluation notebooks required to reproduce the experiments reported in the accompanying manuscript.

---

# Citation

If you use the CIFQA benchmark or implementation in your research, please cite the accompanying paper.

The official BibTeX citation and DOI will be added after the paper is published.

---

# License

This repository is released under the MIT License.

---

# Authors

**Kunjesh Parekh**  
School of Artificial Intelligence and Data Science  
Indian Institute of Technology Jodhpur

**Divya Sharma**  
School of Artificial Intelligence and Data Science  
Indian Institute of Technology Jodhpur

**Anil Kumar Tiwari**  
School of Artificial Intelligence and Data Science  
Indian Institute of Technology Jodhpur
