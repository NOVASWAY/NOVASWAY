# AI + Security Portfolio Lab

A practical learning track for applying AI to defensive security while keeping data local, outputs reviewable, and claims honest. This page describes planned experiments—not completed projects.

## Tools to explore

- **Ollama** — run open-weight language models locally for privacy-conscious experiments.
- **Hugging Face Transformers** — learn model inference and experiment with text classification.
- **MITRE ATT&CK** — give detection findings a consistent, defensible vocabulary.
- **Promptfoo** — evaluate prompts and test for unsafe or unreliable model behavior.
- **Python** — build small, reproducible command-line tools and evaluation scripts.

## Project roadmap

### 1. Local SOC alert triage assistant

Feed sanitized sample alerts to a local model and ask it to produce a concise summary, evidence cited from the input, uncertainty, and suggested analyst checks. Compare its output with a rule-based baseline and record false or unsupported claims.

**Guardrails:** use synthetic or sanitized data; do not send logs to hosted services; never let the model execute commands or close alerts; require an analyst to verify every recommendation.

### 2. Phishing-language classifier experiment

Use a public, appropriately licensed dataset to compare a simple baseline with a Hugging Face text-classification model. Report precision, recall, false positives, dataset limitations, and examples where the model is uncertain. Treat the result as a triage aid, not a verdict.

### 3. Prompt-injection evaluation mini-lab

Build a small test set of benign adversarial prompts and use Promptfoo to check whether a model follows the intended task, reveals configured test secrets, or produces unsupported claims. Document the threat model and limits; keep the tests local and isolated.

## Progress

These are proposed portfolio projects. I’ll update this page with code, reproducible steps, evaluation results, and lessons learned as each experiment is completed.
