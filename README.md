# Debu Sinha

**Principal ML Engineer** @ Databricks | Author | IEEE Senior Member

I build evaluation and safety infrastructure for AI systems. 21 merged PRs across 7 open-source projects in the past 4 months, focused on production-grade LLM evaluation, security hardening, and deployment tooling.

---

## MLflow Core Contributor

[MLflow](https://github.com/mlflow/mlflow) is the most widely adopted open-source ML lifecycle platform (23K+ stars, 18M+ monthly PyPI downloads). I've contributed 6 merged PRs to MLflow core, building evaluation capabilities used by ML practitioners worldwide.

### GenAI Evaluation Framework

Built 3 of 5 third-party scorer integrations for MLflow's evaluation framework, connecting it to external AI safety and quality libraries. Each integration was independently reviewed and approved by MLflow maintainers:

- **[Phoenix (Arize) Integration](https://github.com/mlflow/mlflow/pull/19473)** -- Hallucination detection, relevance scoring, QA correctness, summarization quality. 5 scorers.
- **[TruLens Integration](https://github.com/mlflow/mlflow/pull/19492)** -- Groundedness, context relevance, and 6 agent trace evaluators based on the [Agent GPA framework](https://arxiv.org/abs/2510.08847). 10 scorers total.
- **[Guardrails AI Integration](https://github.com/mlflow/mlflow/pull/20038)** -- Deterministic safety validators (toxicity, PII detection, jailbreak detection) with zero LLM dependency.

### Infrastructure and Deployment

- **[LLM Judge inference parameters](https://github.com/mlflow/mlflow/pull/19152)** -- Temperature, top_p, max_tokens control for evaluation reproducibility
- **[Configurable scorer parallelism](https://github.com/mlflow/mlflow/pull/19248)** -- `MLFLOW_GENAI_EVAL_MAX_SCORER_WORKERS` for resource-constrained environments
- **[Modal deployment documentation](https://github.com/mlflow/mlflow/pull/20032)** -- Added Modal as a supported deployment target with full guide

[UV Integration Design Doc](https://github.com/debu-sinha/design-docs/blob/main/mlflow/uv-support-design-doc-v2.md) | 3 blog posts pending on [mlflow.org/blog](https://mlflow.org/blog)

---

## LlamaIndex Security and Reliability

5 merged PRs focused on hardening LlamaIndex against code execution vulnerabilities and improving API reliability. All reviewed by [@AstraBert](https://github.com/AstraBert) (LlamaIndex maintainer).

- **[Token-bucket rate limiter](https://github.com/run-llama/llama_index/pull/20712)** -- Shared rate limiter for LLM and embedding API calls with burst support and backpressure
- **[Sandbox LLM code execution](https://github.com/run-llama/llama_index/pull/20676)** -- Eliminated arbitrary code execution in EvaporateExtractor
- **[Block filesystem/network I/O](https://github.com/run-llama/llama_index/pull/20691)** -- Sandboxed safe_exec and safe_eval with timeout enforcement
- **[Replace eval() with json.loads](https://github.com/run-llama/llama_index/pull/20675)** -- Closed code injection vector in FaissMapVectorStore persistence
- **[Retry and error handling](https://github.com/run-llama/llama_index/pull/20693)** -- Graceful degradation for BaseExtractor failures

---

## Cross-Project Contributions

### TruLens (Snowflake)

4 merged PRs: [instrumentation crash fix](https://github.com/truera/trulens/pull/2328), [Databricks structured output compatibility](https://github.com/truera/trulens/pull/2308), [MLflow integration documentation](https://github.com/truera/trulens/pull/2344), [pkg_resources deprecation fix](https://github.com/truera/trulens/pull/2351).

### Guardrails AI

4 merged PRs: [uv package manager support with validator registry](https://github.com/guardrails-ai/guardrails/pull/1416), [custom validator Hub API key fix](https://github.com/guardrails-ai/guardrails/pull/1403), [MLflow integration guide](https://github.com/guardrails-ai/guardrails/pull/1394), [concurrency-safe temp file handling](https://github.com/guardrails-ai/secrets_present/pull/10).

### Other

- **[Excalidraw MCP](https://github.com/excalidraw/excalidraw-mcp/pull/18)** -- Path traversal prevention and resource exhaustion hardening
- **[Phoenix (Arize)](https://github.com/Arize-ai/phoenix/pull/11322)** -- MLflow integration documentation

---

## MLflow-Modal Deployment Plugin

[![PyPI](https://img.shields.io/pypi/v/mlflow-modal-deploy?style=flat-square)](https://pypi.org/project/mlflow-modal-deploy/)
[![Downloads](https://img.shields.io/pypi/dm/mlflow-modal-deploy?style=flat-square)](https://pypi.org/project/mlflow-modal-deploy/)

Deploy MLflow models to serverless GPU infrastructure with auto-scaling from zero to H200s.

```bash
pip install mlflow-modal-deploy
mlflow deployments create -t modal -m models:/my-model/1 --name my-deployment
```

[GitHub](https://github.com/debu-sinha/mlflow-modal-deploy) | [PyPI](https://pypi.org/project/mlflow-modal-deploy/)

---

## Publications

### Book

<a href="https://www.amazon.com/dp/1801812039">
<img src="assets/book-cover.jpg" alt="Practical Machine Learning on Databricks" width="120" align="left" style="margin-right: 15px;"/>
</a>

**[Practical Machine Learning on Databricks](https://www.amazon.com/dp/1801812039)**
<br/>Packt Publishing, 2023 | 244 pages

End-to-end guide for building production ML systems on the Lakehouse.

<br clear="left"/>

### Research

<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white"/></a>

| Paper | Venue |
|-------|-------|
| [The Semantic Illusion](https://arxiv.org/abs/2512.15068) -- Hallucination detection failure modes | arXiv 2025 |
| [Learning to Translate with Products of Novices](https://aclanthology.org/Q13-1014/) | TACL 2013 |

---

## Speaking

| Event | Topic |
|-------|-------|
| TechFutures 2025 (NYC) | [End-to-End MLOps Workshop](https://github.com/debu-sinha/techfutures-2025-mlops-databricks) |
| Data Con LA 2022 | [Databricks Feature Store](https://www.youtube.com/watch?v=xPuCCY93BMY) |
| Data Con LA 2021 | [Fraud Detection at Scale](https://www.youtube.com/watch?v=5SA2GT-vBvY) |
| NYU Guest Lecture | ML Pipelines with Apache Spark |

---

## Professional

**IEEE Senior Member** -- Recognition for significant contributions to the profession (requires 10+ years experience and documented achievements).

---

<p align="left">
<a href="https://www.linkedin.com/in/debusinha/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:debusinha2009@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ"><img src="https://img.shields.io/badge/Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white"/></a>
</p>
