# Debu Sinha

**Lead Specialist Solutions Architect (Applied AI and ML)** @ Databricks. I work on the layer between LLM evaluation infrastructure and the agent frameworks built on top: tracing, scorers, judges, retry semantics, safety hardening, and agent observability.

Reviewer for NeurIPS 2026 (main track, Evaluations & Datasets, Position Papers). Technical manuscript reviewer for Packt Publishing and Manning Publications. IEEE Senior Member.

## Selected work

- [SycoBench-600: Measuring Sycophancy and Correction Selectivity in LLM Assistants](https://aclanthology.org/2026.findings-acl.1759/) - ACL 2026 Findings. Introduces correction selectivity as a separate evaluation axis from sycophancy. Code, dataset, and per-model results at [sycobench-600](https://github.com/debu-sinha/sycobench-600).

- [The Semantic Illusion: Certified Limits of Embedding-Based Hallucination Detection in RAG Systems](https://arxiv.org/abs/2512.15068) - arXiv preprint on why semantic-similarity and NLI-style detectors can fail on realistic RAG hallucinations even when conformal coverage is calibrated.

- MLflow GenAI evaluation integrations - third-party scorer framework work across [Phoenix](https://github.com/mlflow/mlflow/pull/19473), [TruLens](https://github.com/mlflow/mlflow/pull/19492), [Guardrails AI](https://github.com/mlflow/mlflow/pull/20038), uv dependency support, and related mlflow.org writeups.

- Inspect AI + MLflow tracking - first [MLflow tracking hook](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3433) for the UK AI Safety Institute's Inspect framework, followed by artifact logging and tracing work.

- OTel observability finish for [omnigent](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha) ([3 merged](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha+is%3Amerged), [5 open](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha+is%3Aopen)): GenAI semconv span attributes, W3C TRACEPARENT subprocess propagation, GenAI metric instruments, retry events on the production async path, end-to-end OTLP receiver test, plus the canonical [Databricks integration guide](https://github.com/omnigent-ai/omnigent/pull/1144).

## Publications

<a href="https://www.amazon.com/dp/1801812039"><img src="assets/book-cover.jpg" alt="Practical Machine Learning on Databricks" width="120" align="left" style="margin-right: 15px;"/></a>

[Practical Machine Learning on Databricks](https://www.amazon.com/dp/1801812039) (Packt, 2023)

[SycoBench-600: Measuring Sycophancy and Correction Selectivity in LLM Assistants](https://aclanthology.org/2026.findings-acl.1759/) (ACL 2026 Findings)

[The Semantic Illusion: Certified Limits of Embedding-Based Hallucination Detection in RAG Systems](https://arxiv.org/abs/2512.15068) (arXiv, 2025)

[Learning to Translate with Products of Novices](https://aclanthology.org/Q13-1014/) (TACL, 2013)

<br clear="left"/>

## Writing on mlflow.org

- [Reproducible Model Dependencies with uv and MLflow](https://mlflow.org/docs/latest/ml/model/dependencies/#using-uv-for-dependency-management)
- [Tracking and Debugging AI Safety Evaluations with Inspect AI and MLflow](https://mlflow.org/blog/inspect-mlflow-integration)
- [Agent Trace Evaluation with TruLens Scorers in MLflow](https://mlflow.org/blog/mlflow-trulens-evaluation)
- [Deterministic Safety and PII Checks with Guardrails AI in MLflow](https://mlflow.org/blog/mlflow-guardrails-scorers)
- [Deploy MLflow Models to Serverless GPUs with Modal](https://mlflow.org/blog/mlflow-modal-deploy)
- [Third-Party Scorers in MLflow](https://mlflow.org/blog/third-party-scorers)

---

[Full OSS contributions](OSS.md) | [Speaking and workshops](SPEAKING.md) | <a href="https://www.linkedin.com/in/debusinha/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a> | <a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white"/></a>
