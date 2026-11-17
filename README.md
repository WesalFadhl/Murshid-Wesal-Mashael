# 🧭 Murshid — LLM Application Engineering

[![SDAIA](https://img.shields.io/badge/SDAIA-Training_Program-006C67?style=for-the-badge)](https://sdaia.gov.sa/)
![Course](https://img.shields.io/badge/Course-SDA--AIE--213-blue)
![Python](https://img.shields.io/badge/Python-3.x-yellow?logo=python)
![Status](https://img.shields.io/badge/Status-In_Progress-orange)

### SDAIA | SDA-AIE-213

A hands-on, four-day LLM Application Engineering project developed as part of a training program at the **Saudi Data & Artificial Intelligence Authority (SDAIA)**.

**Murshid** is a bilingual (Arabic–English) public-service assistant designed to demonstrate structured responses, controlled tool interactions, input validation, guardrails, and systematic testing.

This repository documents the progressive development of the project through cumulative labs and independent homework assignments.

---

## 🎯 Project Objectives

- Develop a bilingual assistant for public-service inquiries.
- Implement structured and consistent responses.
- Simulate controlled tool calling for application-status requests.
- Apply input validation, output validation, and guardrails.
- Evaluate system behavior through reproducible test cases.
- Document implementation results, limitations, and improvements.

## 🛠️ Technologies & Tools

| Category | Technology |
|---|---|
| Programming Language | Python 3 |
| Development Environment | Google Colab |
| Model Experiment | Hugging Face Transformers (`google/flan-t5-small`) |
| Data Format | JSON |
| Testing | Python Assertions and Mock Testing |
| Version Control | Git & GitHub |

## 📚 Core Labs

All four core labs are developed cumulatively in the same notebook, `Lab1.ipynb`.

| Day | Topic | Implementation | Status |
|---|---|---|---|
| Day 1 | Bilingual Assistant | FAQ responses, mock client, structured outputs, latency and trace tracking | ✅ Completed |
| Day 2 | Tool Calling | Ticket extraction, validation, status lookup, routing, and authorization checks | ✅ Completed |
| Day 3 | Guardrails & Golden Tests | Input/output validation, instruction-injection protection, and ten golden test cases | ✅ Completed |
| Day 4 | Measurement & Caching | Performance evaluation and caching | ⏳ Upcoming |

## 🧪 Optional Homework

Each optional assignment is implemented separately from the cumulative project notebook.

| Day | Assignment | Outcome | Status |
|---|---|---|---|
| Day 1 | Live Model Demonstration | Local inference using `google/flan-t5-small` | ✅ Completed |
| Day 2 | Structured Tool Dispatcher | Seven test cases passed with unchanged source records | ✅ Completed |
| Day 3 | Error Handling & Input Validation | Three expected errors caught; corrected input accepted | ✅ Completed |
| Day 4 | Upcoming Assignment | Not started | ⏳ Upcoming |

## 📊 Evaluation Results

| Evaluation | Result |
|---|---|
| Day 1 Baseline | Baseline results recorded |
| Day 2 Tool Calling | All required checks passed |
| Day 2 Homework | **7/7 tests passed (100%)** |
| Day 3 Golden Test Suite | **10/10 tests passed (100%)** |
| Day 3 Execution Mode | Mock |
| Day 3 Homework | **3/3 expected errors caught** |
| Corrected Input | Accepted |
| Day 3 Homework Checks | Passed |

**Important:** The Day 3 pass rate represents performance on ten predefined deterministic mock cases. It does not establish production-level security or general accuracy.

## 📁 Repository Structure

```text
Murshid-Wesal-Mashael/
│
├── README.md
├── Lab1.ipynb
├── baseline_results.json
├── day2_results.json
├── day3_results.json
│
└── homework/
    ├── Add Homework 1 JSON Results
    ├── Homework day2_tools.ipynb
    ├── Homework1.ipynb
    ├── Homework2 result JSON
    ├── Homework3.ipynb
    └── day3_results.json
```

The repository contains the cumulative lab notebook, core lab results, and separate homework notebooks and evidence files.

## 🔍 Day 3 — Guardrails & Validation

Day 3 introduces a controlled pipeline with input validation, output validation, and predefined expected behaviors.

The golden test suite covers:

- Arabic and English FAQ responses.
- Authorized application-status lookup.
- Missing references and clarification requests.
- Out-of-scope inquiries.
- Access-denied scenarios.
- Instruction-injection attempts.
- Invalid input and malformed output.

**Golden Test Results:** 10/10 passed in mock mode.

The optional Day 3 homework demonstrates deliberate input rejection using Python exceptions.

Three invalid inputs are tested: `None`, whitespace-only text, and text exceeding 500 characters.

The implementation uses `raise` to signal invalid input, `try` to execute validation, and `except` to catch and verify expected errors.

A correctly caught rejection is considered a successful test because the system identifies invalid input and prevents it from being accepted.

## ⚠️ Limitations

- Core testing relies on synthetic data and deterministic mock behavior.
- Keyword-based guardrails are insufficient for production-level security.
- Evaluation coverage is limited to predefined scenarios.
- Live-model behavior may differ from mock results.

## 👩🏻‍💻 Contributors

- **Wesal Al-Numani**
- **Mashael Al-Mufleh**

## 🏛️ Training Information

**Program:** LLM Application Engineering (SDA-AIE-213)

**Organization:** [Saudi Data & Artificial Intelligence Authority (SDAIA)](https://sdaia.gov.sa/)

**Instructor:** Meaad Al-Marri

**Course Repository:** [Murshid — LLM Application Engineering](https://github.com/almiyead-rgb/murshid-llm-application-engineering-sda-aie-213)

---

*Developed as part of the SDAIA LLM Application Engineering training program.*
