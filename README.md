README
Supplementary Material
Deterministic Tool-Grounded Multi-Agent LLM Framework for Calculation-Intensive Financial Query Answering (CIFQA)
This supplementary package accompanies the manuscript:
Deterministic Tool-Grounded Multi-Agent LLM Framework for Calculation-Intensive Financial Query Answering (CIFQA)
The package contains the source notebooks, representative benchmark, supporting resources, and instructions required to reproduce the representative experiments presented in the manuscript.
Package Contents
File	Description
Main_CIFQA_Notebook.ipynb	Main implementation of the CIFQA framework. Upload this notebook along with the supporting files to Google Colab and execute all cells to reproduce the framework and experimental results.
Ablation_Study_Notebook.ipynb	Notebook for reproducing the ablation study reported in the manuscript.
benchmark_questions.csv	CIFQA benchmark containing all 126 benchmark queries, their categories, and associated metadata.
Benchmark_questions.xlsx	Manually verified reference answers corresponding to all the  benchmark queries.
CIFQA_Results.xlsx	Complete evaluation results, including CIFQA outputs, agentic model results, and frontier LLM responses obtained using the standardized benchmark prompt.
CIFQA_Ablation_Results.xlsx	Results of the ablation study for benchmark queries applicable to each ablation experiment.
Benchmark_Prompt.docx	Standardized benchmark prompt used to evaluate all frontier LLMs under a consistent experimental setting.
Guidelines_pdf.pdf	Financial product guideline document used as the retrieval knowledge source for policy and rule-based queries.
int_rate_new.xlsx	Structured interest-rate table used by the deterministic rate lookup engine during financial computation.

System Requirements
•	Google Colab
•	Python 3.10 or later
•	Internet connection
•	Valid API keys for:
o	groq
o	OpenRouter

Running the Main CIFQA Notebook
Open Main_CIFQA_Notebook.ipynb using Google Colab.
Step 1: Configure API Keys
Before running the notebook, open the Google Colab Secrets (🔑 Secrets) panel and add the following secret variables exactly as shown below:
•	GROQ_API_KEY
•	Open_router_key
These API keys are required to access the large language models used by the CIFQA framework.
Step 2: Upload Supporting Files
Upload the following files into the sample_data folder in Google Colab:
•	benchmark_demo.csv
•	Guidelines_pdf.pdf
•	int_rate_new.xlsx
Step 3: Execute the Notebook
Run all notebook cells sequentially.
The notebook automatically installs all required Python libraries and executes the CIFQA framework on the representative benchmark.
Running the Ablation Study Notebook
Open Ablation_Study_Notebook.ipynb using Google Colab.
Step 1: Configure API Keys
Before running the notebook, add the following secret variables in Google Colab Secrets:
•	GROQ_API_KEY
•	Open_router_key
Step 2: Upload Supporting Files
Upload the following files into the sample_data folder:
•	benchmark_demo.csv
•	Guidelines_pdf.pdf
•	int_rate_new.xlsx
Step 3: Execute the Notebook
Run all notebook cells sequentially.
The notebook reproduces the representative ablation experiments reported in the manuscript.
Reproducibility
This supplementary package includes a representative benchmark consisting of 20 manually verified financial queries together with their corresponding reference answers.
The complete 126-query benchmark used for the experiments reported in the manuscript is proprietary and is therefore not publicly distributed. The released benchmark is intended to enable reviewers and readers to verify the implementation and reproducibility of the CIFQA framework while protecting proprietary evaluation data.
Notes
•	The notebooks automatically install all required Python packages.
•	The benchmark prompt included in this package corresponds to the prompt used for evaluating frontier LLMs reported in the manuscript.
•	Users are responsible for providing their own GROQ and OpenRouter API credentials.
•	The notebooks are designed to execute in Google Colab without requiring additional environment configuration.
Authors
Kunjesh Parekh
School of Artificial Intelligence and Data Science
Indian Institute of Technology Jodhpur
Divya Sharma
School of Artificial Intelligence and Data Science
Indian Institute of Technology Jodhpur
Anil Kumar Tiwari
School of Artificial Intelligence and Data Science
Indian Institute of Technology Jodhpur
