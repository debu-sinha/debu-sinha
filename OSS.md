# OSS contributions

Upstream work across the MLflow, agent-runtime, and AI-safety eval ecosystems.

| Project | Merged | What landed |
|---|---:|---|
| [mlflow/mlflow](https://github.com/mlflow/mlflow/pulls?q=is%3Apr+author%3Adebu-sinha) | 11 | Third-party scorer framework ([Phoenix](https://github.com/mlflow/mlflow/pull/19473), [TruLens](https://github.com/mlflow/mlflow/pull/19492), [Guardrails](https://github.com/mlflow/mlflow/pull/20038)). Google ADK + DeepEval scorer integrations. Rule-based scorers (`RegexMatch`, `PIIDetection`, `ResponseLength`). [uv lock support](https://github.com/mlflow/mlflow/pull/20344) for model logging. |
| [mlflow/mlflow-website](https://github.com/mlflow/mlflow-website/pulls?q=is%3Apr+author%3Adebu-sinha) | 5 | Blog series on TruLens, Guardrails, Inspect AI, uv, and Modal serverless GPU integrations on mlflow.org. |
| [run-llama/llama_index](https://github.com/run-llama/llama_index/pulls?q=is%3Apr+author%3Adebu-sinha) | 6 | Sandboxed [code exec](https://github.com/run-llama/llama_index/pull/20676), [filesystem I/O](https://github.com/run-llama/llama_index/pull/20691), and [`eval()` injection](https://github.com/run-llama/llama_index/pull/20675). Token-bucket rate limiter, retry semantics on `BaseExtractor`. |
| [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai/pulls?q=is%3Apr+author%3Adebu-sinha) | 5 | First [MLflow tracking hook](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3433) for the AI Safety Institute's eval framework. [Artifact logging](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3483) and extension page registration. |
| [guardrails-ai/guardrails](https://github.com/guardrails-ai/guardrails/pulls?q=is%3Apr+author%3Adebu-sinha) | 4 | uv package manager support, dynamic registry loading (Phase 2), MLflow integration guide. |
| [omnigent-ai/omnigent](https://github.com/omnigent-ai/omnigent/pulls?q=is%3Apr+author%3Adebu-sinha) | 3 + **5 open** | OTel observability series: [#1068](https://github.com/omnigent-ai/omnigent/pull/1068) Python logging to OTel bridge (merged), [#1144](https://github.com/omnigent-ai/omnigent/pull/1144) Databricks integration guide (merged), [#1050](https://github.com/omnigent-ai/omnigent/pull/1050) GenAI semconv attrs, [#1070](https://github.com/omnigent-ai/omnigent/pull/1070) TRACEPARENT subprocess injection, [#1071](https://github.com/omnigent-ai/omnigent/pull/1071) `gen_ai.retry` events on the async retry path, [#1072](https://github.com/omnigent-ai/omnigent/pull/1072) GenAI metric instruments, [#1083](https://github.com/omnigent-ai/omnigent/pull/1083) end-to-end OTLP receiver test. |
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
