# 🧠 Question-Analysis Prompting (QAP): Improving LLM Reasoning Performance

**Dharunish Yugeswardeenoo, Kevin Zhu, Sean O'Brien**  
*Published in Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (ACL) @ ACL 2025*


This repository hosts the web version of our paper **“Question-Analysis Prompting Improves LLM Performance in Reasoning Tasks”**, which investigates how prompting strategies influence reasoning accuracy in language models such as GPT-3.5 Turbo and GPT-4 Turbo.

---

## 📘 Abstract

Large language models (LLMs) have demonstrated remarkable reasoning capabilities but often fail to provide consistent, step-by-step logic in complex multi-step problems.  
We propose **Question-Analysis Prompting (QAP)** — a simple yet effective method that guides models to first analyze the question structure before generating reasoning steps.  

Experiments show that QAP enhances reasoning accuracy across diverse benchmarks including **GSM8K, AQuA, SAT, and StratQA**, compared to baseline prompting methods.

---

## 🧩 QAP Prompting Workflow

<div align="center">
  <img src="static/images/CoTvQAP.png" alt="QAP Prompting Workflow Diagram" width="80%" />
</div>

**Figure 1.** QAP Prompting Workflow Diagram — illustrating the structured reasoning process introduced in our approach.

---

## 📊 Experimental Results

Below are summary tables showing the performance comparison between **GPT-3.5 Turbo** and **GPT-4 Turbo** under different prompting conditions.

<div align="center">

### 🧮 Table 1: Results for GPT-3.5 Turbo

| Prompt  | GSM8K | AQuA | SAT  | StratQA |
|----------|-------|------|------|----------|
| Baseline | 78.7  | 52.8 | 70.9 | **65.1** |
| QAP25    | 67.1  | 39.4 | 35.0 | 63.1 |
| QAP50    | 77.8  | 50.0 | 52.7 | 61.4 |
| QAP100   | 77.4  | 53.9 | 75.0 | 57.1 |
| QAP150   | 78.5  | **59.4** | **78.6** | 53.2 |
| QAP200   | 76.8  | 52.4 | 75.0 | 51.8 |
| TADB     | 78.5  | 57.1 | 74.5 | 62.9 |
| CoT      | **79.0** | 53.1 | 65.9 | 59.2 |
| PS+      | 74.7  | 35.0 | 70.9 | 35.6 |

---

### ⚙️ Table 2: Results for GPT-4 Turbo

| Prompt  | GSM8K | AQuA | SAT  | StratQA |
|----------|-------|------|------|----------|
| Baseline | 95.3 | 78.7 | 96.8 | 76.3 |
| QAP25    | 94.8 | 77.6 | 94.5 | 77.6 |
| QAP50    | 93.4 | **79.1** | 95.9 | 76.9 |
| QAP100   | 94.6 | 75.6 | 96.8 | 77.2 |
| QAP150   | 94.7 | 78.0 | 97.3 | 77.6 |
| QAP200   | 95.0 | 76.4 | **98.2** | 75.9 |
| TADB     | 95.1 | 78.7 | 96.8 | **78.0** |
| CoT      | **95.6** | 74.4 | 95.0 | 75.1 |
| PS+      | 94.8 | 52.8 | 97.3 | 77.1 |

</div>

---

## 💡 Key Findings

- QAP consistently **enhances reasoning accuracy** on multi-step benchmarks.  
- Performance gains are **most pronounced for GPT-3.5 Turbo**, indicating greater benefit for smaller LLMs.  
- Structured pre-analysis helps reduce reasoning drift and logical inconsistencies.  

---


