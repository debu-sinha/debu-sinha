# Debu Sinha

**Lead Applied AI/ML Engineer (Solutions Architecture)** @ Databricks
IEEE Senior Member · NeurIPS 2026 reviewer (Datasets & Benchmarks)

I work on the layer between AI evaluation infrastructure and the agent
frameworks built on top: tracing, scorers, judges, safety hardening.
Author of [_Practical Machine Learning on Databricks_](https://www.amazon.com/dp/1801812039)
(Packt, 2023). Built the first MLflow tracking integration for the
[UK AI Safety Institute's `inspect_ai` framework](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3433),
and the third-party scorer framework in MLflow that connects
[Phoenix](https://github.com/mlflow/mlflow/pull/19473),
[TruLens](https://github.com/mlflow/mlflow/pull/19492), and
[Guardrails AI](https://github.com/mlflow/mlflow/pull/20038)
into the GenAI eval pipeline.

## Currently shipping

- **[OTel observability finish for omnigent](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha)** ([6 open PRs](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha+is%3Aopen)) — GenAI semconv span attributes, W3C TRACEPARENT subprocess propagation, Python `logging` to OTel bridge, GenAI metric instruments, `gen_ai.retry` span events, end-to-end OTLP receiver test.
- **[omnigent-mlflow](https://pypi.org/project/omnigent-mlflow/) v0.1.1** on PyPI — MLflow tracing adapter for omnigent agents (one span per StreamHooks callback, one trace per turn) while the upstream work lands.
- **[inspect-mlflow](https://github.com/debu-sinha/inspect-mlflow) v0.8.0** — cost + latency tracking on every Inspect AI sample, plus S3 artifact upload.


| Project | Merged | What landed |
|---|---:|---|
| [mlflow/mlflow](https://github.com/mlflow/mlflow/pulls?q=is%3Apr+author%3Adebu-sinha) | 11 | Third-party scorer framework ([Phoenix](https://github.com/mlflow/mlflow/pull/19473), [TruLens](https://github.com/mlflow/mlflow/pull/19492), [Guardrails](https://github.com/mlflow/mlflow/pull/20038)). Google ADK + DeepEval scorer integrations. Rule-based scorers (`RegexMatch`, `PIIDetection`, `ResponseLength`). [uv lock support](https://github.com/mlflow/mlflow/pull/20344) for model logging. |
| [mlflow/mlflow-website](https://github.com/mlflow/mlflow-website/pulls?q=is%3Apr+author%3Adebu-sinha) | 5 | Blog series on TruLens, Guardrails, Inspect AI, uv, and Modal serverless GPU integrations on mlflow.org. |
| [run-llama/llama_index](https://github.com/run-llama/llama_index/pulls?q=is%3Apr+author%3Adebu-sinha) | 6 | Sandboxed [code exec](https://github.com/run-llama/llama_index/pull/20676), [filesystem I/O](https://github.com/run-llama/llama_index/pull/20691), and [`eval()` injection](https://github.com/run-llama/llama_index/pull/20675). Token-bucket rate limiter, retry semantics on `BaseExtractor`. |
| [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai/pulls?q=is%3Apr+author%3Adebu-sinha) | 5 | First [MLflow tracking hook](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3433) for the AI Safety Institute's eval framework. [Artifact logging](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3483) and extension page registration. |
| [guardrails-ai/guardrails](https://github.com/guardrails-ai/guardrails/pulls?q=is%3Apr+author%3Adebu-sinha) | 4 | uv package manager support, dynamic registry loading (Phase 2), MLflow integration guide. |
| [omnigent-ai/omnigent](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha) | 1 + **6 open** | OTel observability series: [#1050](https://github.com/omnigent-ai/omnigent/pull/1050) GenAI semconv attrs, [#1070](https://github.com/omnigent-ai/omnigent/pull/1070) TRACEPARENT subprocess injection, [#1068](https://github.com/omnigent-ai/omnigent/pull/1068) Python logging to OTel bridge, [#1072](https://github.com/omnigent-ai/omnigent/pull/1072) GenAI metric instruments, [#1071](https://github.com/omnigent-ai/omnigent/pull/1071) `gen_ai.retry` events, [#1083](https://github.com/omnigent-ai/omnigent/pull/1083) end-to-end OTLP receiver test. |
| [truera/trulens](https://github.com/truera/trulens/pulls?q=is%3Apr+author%3Adebu-sinha) | 2 | Dropped `pkg_resources` from `trulens-core`. MLflow integration guide. |
| [Arize-ai/phoenix](https://github.com/Arize-ai/phoenix/pulls?q=is%3Apr+author%3Adebu-sinha) | 1 | MLflow added to eval-library integrations docs. |
| [pydantic/pydantic-ai](https://github.com/pydantic/pydantic-ai/pulls?q=is%3Apr+author%3Adebu-sinha) | 1 | YAML round-trip fix on `HasMatchingSpan` SpanQuery args. |
| [UKGovernmentBEIS/inspect_evals](https://github.com/UKGovernmentBEIS/inspect_evals/pulls?q=is%3Apr+author%3Adebu-sinha) | 1 | CodeIPI: Indirect Prompt Injection benchmark for coding agents. |
| [excalidraw/excalidraw-mcp](https://github.com/excalidraw/excalidraw-mcp/pulls?q=is%3Apr+author%3Adebu-sinha) | 1 | Hardened checkpoint store against path traversal and resource exhaustion. |

## Maintained packages

[![PyPI mlflow-modal-deploy](https://img.shields.io/pypi/v/mlflow-modal-deploy?label=mlflow-modal-deploy)](https://pypi.org/project/mlflow-modal-deploy/) [![Downloads modal-deploy](https://img.shields.io/pypi/dm/mlflow-modal-deploy?label=modal-deploy%20downloads)](https://pypi.org/project/mlflow-modal-deploy/) [![PyPI omnigent-mlflow](https://img.shields.io/pypi/v/omnigent-mlflow?label=omnigent-mlflow)](https://pypi.org/project/omnigent-mlflow/)

- [mlflow-modal-deploy](https://github.com/debu-sinha/mlflow-modal-deploy) - Deploy MLflow models to serverless GPUs (T4 to H200) via Modal
- [omnigent-mlflow](https://github.com/debu-sinha/omnigent-mlflow-quickstart) - MLflow tracing adapter for omnigent agents
- [inspect-mlflow](https://github.com/debu-sinha/inspect-mlflow) - MLflow integration for Inspect AI evals (experiment tracking, execution tracing, S3 artifact upload)
- [agentsec](https://github.com/debu-sinha/agentsec) - Security scanner for agentic AI installations (OpenClaw, MCP server hardening)
- [sycobench-600](https://github.com/debu-sinha/sycobench-600) - ACL 2026 Findings benchmark for measuring LLM sycophancy and correction selectivity

## Publications

<a href="https://www.amazon.com/dp/1801812039"><img src="assets/book-cover.jpg" alt="Practical Machine Learning on Databricks" width="120" align="left" style="margin-right: 15px;"/></a>

**[Practical Machine Learning on Databricks](https://www.amazon.com/dp/1801812039)** (Packt, 2023)

**[The Semantic Illusion: Why Surface Sycophancy Metrics Miss Most Yielding](https://arxiv.org/abs/2512.15068)** (arXiv 2025 / ACL 2026 Findings)

**[Learning to Translate with Products of Novices](https://aclanthology.org/Q13-1014/)** (TACL, 2013)

<br clear="left"/>

## Blog series on mlflow.org

- [Reproducible Model Dependencies with uv and MLflow](https://mlflow.org/blog/mlflow-uv-dependency-management)
- [Tracking and Debugging AI Safety Evaluations with Inspect AI and MLflow](https://mlflow.org/blog/inspect-mlflow-integration)
- [Agent Trace Evaluation with TruLens Scorers in MLflow](https://mlflow.org/blog/mlflow-trulens-evaluation)
- [Deterministic Safety and PII Checks with Guardrails AI in MLflow](https://mlflow.org/blog/mlflow-guardrails-scorers)
- [Deploy MLflow Models to Serverless GPUs with Modal](https://mlflow.org/blog/mlflow-modal-deploy)
- [Third-Party Scorers in MLflow](https://mlflow.org/blog/third-party-scorers)

## Speaking

[ODSC AI East 2026 (Boston)](https://odsc.com/boston/) · [TechFutures 2025 (NYC)](https://github.com/debu-sinha/techfutures-2025-mlops-databricks) · [Data Con LA](https://www.youtube.com/watch?v=xPuCCY93BMY) · [Hevo Data Lakehouse Panel](https://hevodata.com/webinar/building-and-managing-the-modern-datastore-the-data-lakehouse/) · [Databricks Community](https://www.youtube.com/watch?v=btEya9kdW4Y)

## Workshops

- [mlflow-eval-workshop](https://github.com/debu-sinha/mlflow-eval-workshop) - Evaluating LLM applications with MLflow (ODSC AI East 2026)
- [databricks-gepa-workshop](https://github.com/debu-sinha/databricks-gepa-workshop) - GEPA prompt optimization on Databricks
- [databricks-genai-evaluation-workshop](https://github.com/debu-sinha/databricks-genai-evaluation-workshop) - MLflow GenAI tracing, custom scorers, LLM judges
- [scribd-evaluation-workshop](https://github.com/debu-sinha/scribd-evaluation-workshop) - End-to-end GenAI evaluation on Databricks
- [mlflow-uc-traces-quickstart](https://github.com/debu-sinha/mlflow-uc-traces-quickstart) - Databricks notebook for the MLflow OTel-Traces-in-UC Public Preview

---

<p align="left">
<a href="https://www.linkedin.com/in/debusinha/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white"/></a>
</p>
