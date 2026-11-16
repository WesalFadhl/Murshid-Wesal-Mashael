# 🧭 Murshid
### LLM Application Engineering | SDA-AIE-213

**A Bilingual AI Service Assistant**

An academic project developed as part of the **LLM Application Engineering** training program at [SDAIA – Saudi Data & AI Authority](https://sdaia.gov.sa/).

---

## 📌 Project Overview

**Murshid** is a bilingual (Arabic–English) service assistant designed to explore the principles of Large Language Model (LLM) application engineering.

The project follows an incremental development approach, focusing on structured responses, model integration, input validation, controlled tool execution, and systematic evaluation.

## 🎯 Project Objectives

- Develop a bilingual AI service assistant.
- Explore LLM integration and structured output handling.
- Implement controlled, read-only tool interactions.
- Apply input validation and authorization checks.
- Evaluate system functionality through reproducible tests.

## 🛠️ Technologies & Tools

| Category | Technology |
|---|---|
| Programming Language | Python |
| Development Environment | Google Colab |
| Language Model | Google FLAN-T5 Small |
| Libraries | Hugging Face Transformers, PyTorch |
| Version Control | Git & GitHub |
| Data Format | JSON |

## 📚 Labs & Homework Progress

| Day | Core Lab | Homework | Status |
|---|---|---|---|
| **Day 1** | Basic Service Assistant | Real LLM Inference | ✅ Completed |
| **Day 2** | Structured Tickets & Read-Only Tool | Tool Validation & Dispatch | ✅ Completed |

### 🔹 Day 1 — Foundations

**Lab 1:** Developed a bilingual service assistant using a deterministic `FakeClient`, including structured responses, trace identifiers, latency measurements, and baseline validation.

**Homework 1:** Demonstrated real language model inference using `google/flan-t5-small` with tokenization and response generation.

### 🔹 Day 2 — Structured Tickets & Tool Integration

**Lab 2:** Extended the assistant with structured ticket extraction, schema validation, and a read-only status lookup with ownership verification.

**Homework 2:** Implemented a tool dispatcher to validate structured calls, enforce allowed operations, and protect application records.

## 📊 Key Results

| Evaluation | Result |
|---|---|
| Day 1 — Lab | Baseline verification completed |
| Day 1 — Homework | Successful FLAN-T5 inference |
| Day 2 — Lab | **5/5 reference cases passed** |
| Day 2 — Homework | **7/7 test cases passed** |
| Data Integrity | **Records unchanged** |

## 📂 Repository Structure

```text
Murshid-Wesal-Mashael/
│
├── 📄 README.md
├── 📓 Lab1.ipynb
├── 📊 baseline_results.json
├── 📊 day2_results.json
│
└── 📁 homework/
    ├── 📓 Homework1.ipynb
    ├── 📓 Homework day2_tools.ipynb
    ├── 📊 live_demo_result.json
    └── 📊 tools_result.json
```

The core notebook is updated cumulatively throughout the training program, while homework assignments are maintained separately.

## 👩🏻‍💻 Contributors

**Wesal Al-Numani**  
**Mashael Al-Mufleh**

Computer Science Students | King Saud University

## 🎓 Acknowledgment

Developed as part of the **LLM Application Engineering (SDA-AIE-213)** training program at [SDAIA](https://sdaia.gov.sa/).

**Instructor:** Meaad Al-Marri

**Original Course Repository:**  
https://github.com/almiyead-rgb/murshid-llm-application-engineering-sda-aie-213

---

*This repository documents ongoing academic work and will be updated as additional laboratory exercises and assignments are completed.*
