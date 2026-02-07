
```
├── Experiment/
│   ├── Scenario1/                 
│   │   ├── CodeLlama/
│   │   └── Gemini/
│   └── Scenario2/                 
│       ├── CodeLlama/
│       └── Gemini/
│
├── Evaluation/                   # Evaluation code for SR
│
├── VulnerabilitySummaryModule/
│   ├── Finetune/                   # Fine-tuning a vulnerability summarizer
│   └── Inference/                  # Inference-time generation of summaries
```


---

## 📘 Modules

### 🛡️ Vulnerability Summary Module

A lightweight sub-LLM trained to summarize retrieved code with:
- **Vulnerability serverity**
- **Associated security intent**

Helps reduce generation of unsafe code when used as a gating or prompt-enhancement module.

- `Finetune/`: contains finetune LLM.
- `Inference/`: inference scripts for generating summaries.

---
### 📊 Evaluation

Contains code to compute:
- **Secure Rate (SR)**: Based on static analyzer output
