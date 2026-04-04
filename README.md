# Xstock
Xstock: A 15-Year Longitudinal Dataset Bridging Social Media and B2B Financials for Explainable Stock Forecasting

[![Hugging Face Dataset](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Datasets-blue)](https://huggingface.co/datasets/Xiuze/Xstock)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)

**Xstock** is a 15-year longitudinal benchmark (2011–2025) designed to connect Business-to-Business (B2B) social media discourse with institutional financial performance. By merging **220,000 corporate tweets** with granular **SEC 10-K revenue segment filings**, this project provides a robust framework for **Explainable AI (XAI)** in quantitative finance.

---

## 🌟 Key Innovations

- **Fiscally Grounded Alignment**: Unlike retail-centric datasets, Xstock maps social signals to specific revenue segments, revealing a strong correlation ($r=0.35$) between disclosure volume and fundamental growth.
- **Strategic Narrative Buffering**: Our analysis identifies a unique corporate resilience mechanism where firms pivot toward non-business signaling (e.g., ESG, Thought Leadership) during fiscal downturns.
- **Quantitative Chain-of-Thought (Q-CoT)**: We propose a reasoning paradigm that utilizes weighted scoring and "de-hyping" heuristics to achieve a **fourfold recall improvement** in forecasting market losses.

---

## 📂 Project Structure

```bash
.
├── data/                   # Data loading and SEC 10-K parsing scripts
├── experiments/            # Core reasoning pipelines
│   ├── run_experiment.py   # Main execution script for all modes
│   └── prompt_templates.py # Normal, CoT, and Q-CoT implementations
├── models/                 # LLM API wrappers (GPT-4o, Gemini 2.5, Qwen)
├── analysis/               # Statistical notebooks (r-value & sentiment plots)
├── requirements.txt        # Dependency list
└── README.md
```

## 🚀 Getting Started
### 1. Installation
```bash
git clone [https://github.com/Xiuze/Xstock.git](https://github.com/Xiuze/Xstock.git)
cd Xstock
pip install -r requirements.txt
```

### 2. Run Experiments
You can replicate our results by running the experiment in Q-CoT mode:
```python

```

## 📊 Dataset Access
The full dataset is available on Hugging Face: [Xiuze/Xstock](https://huggingface.co/datasets/Xiuze/Xstock).
```python
from datasets import load_dataset
dataset = load_dataset("Xiuze/Xstock")
```

## 📖 Citation
If you use Xstock in your research, please cite our work:
```

```

## ⚖️ License
Distributed under the **CC BY-NC 4.0 License**. Non-commercial research use only.

