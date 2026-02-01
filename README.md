# Debu Sinha

**Principal ML Engineer** @ Databricks | Author | IEEE Senior Member

I build production-grade ML and GenAI systems, with a focus on deployment, evaluation, and reliability. My contributions include implementing core evaluation capabilities in MLflow and building tooling used in enterprise AI systems.

---

## Technical Contributions

### MLflow Core Contributor

[**MLflow**](https://github.com/mlflow/mlflow) is one of the most widely adopted open-source ML lifecycle platforms globally (23K+ stars, 18M+ monthly PyPI downloads).

#### Production GenAI Evaluation Capabilities

Implemented 3 of 5 third-party scorer integrations for MLflow's GenAI evaluation framework. Each contribution was independently reviewed, approved, and merged by senior MLflow maintainers:

| Integration | PR | Maintainer Review | Production Impact |
|-------------|-----|-------------------|-------------------|
| **Phoenix (Arize)** | [#19473](https://github.com/mlflow/mlflow/pull/19473) | Reviewed by @smoorjani, @B-Step62 | Hallucination detection, relevance scoring |
| **TruLens** | [#19492](https://github.com/mlflow/mlflow/pull/19492) | Reviewed by @smoorjani, @B-Step62 | Groundedness, context relevance, agent evaluation |
| **Guardrails AI** | [#20038](https://github.com/mlflow/mlflow/pull/20038) | Reviewed by @smoorjani | Safety validators (toxicity, PII, jailbreak detection) |

These capabilities are now available to ML practitioners and enterprises worldwide.

#### Infrastructure & Deployment Contributions

| PR | Capability | Status | Impact |
|----|------------|--------|--------|
| [#19152](https://github.com/mlflow/mlflow/pull/19152) | LLM Judge inference parameters | ✅ Merged | Temperature, top_p control for evaluation |
| [#19248](https://github.com/mlflow/mlflow/pull/19248) | Configurable scorer parallelism | ✅ Merged | `MLFLOW_GENAI_EVAL_MAX_SCORER_WORKERS` |
| [#20344](https://github.com/mlflow/mlflow/pull/20344) | UV package manager integration | 🔄 In Review | Automatic dependency inference |

[UV Integration Design Doc](https://github.com/debu-sinha/design-docs/blob/main/mlflow/uv-support-design-doc-v2.md)

---

### Cross-Project Contributions

Bug fixes independently reviewed and merged by external maintainers:

| Repository | PR | Issue Resolved |
|------------|-----|----------------|
| [truera/trulens](https://github.com/truera/trulens/pull/2328) | #2328 | Instrumentation crash on non-callable objects |
| [truera/trulens](https://github.com/truera/trulens/pull/2308) | #2308 | Databricks structured outputs compatibility |

Open contributions under review:

| Repository | PR | Proposed Fix |
|------------|-----|--------------|
| [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph/pull/6547) | #6547 | Type signature for conditional edges |
| [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph/pull/6544) | #6544 | functools.partial handling in ToolNode |

---

### MLflow-Modal Deployment Plugin

[![PyPI](https://img.shields.io/pypi/v/mlflow-modal-deploy?style=flat-square)](https://pypi.org/project/mlflow-modal-deploy/)
[![Downloads](https://img.shields.io/pypi/dm/mlflow-modal-deploy?style=flat-square)](https://pypi.org/project/mlflow-modal-deploy/)

Production deployment capability enabling MLflow models to run on serverless GPU infrastructure:

```bash
pip install mlflow-modal-deploy
mlflow deployments create -t modal -m models:/my-model/1 --name my-deployment
```

- Auto-scaling from zero to thousands of GPUs (T4 → H200)
- Sub-second cold starts
- Native MLflow deployment interface

[GitHub](https://github.com/debu-sinha/mlflow-modal-deploy) | [PyPI](https://pypi.org/project/mlflow-modal-deploy/)

---

## Publications

### Book

<a href="https://www.amazon.com/dp/1801812039">
<img src="assets/book-cover.jpg" alt="Practical Machine Learning on Databricks" width="120" align="left" style="margin-right: 15px;"/>
</a>

**[Practical Machine Learning on Databricks](https://www.amazon.com/dp/1801812039)**
<br/>Packt Publishing, 2023 | 244 pages

End-to-end guide for building production ML systems. Best-seller in category.

<br clear="left"/>

### Research Papers

<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white"/></a> Research Affiliate, Johns Hopkins University

| Paper | Focus | Venue |
|-------|-------|-------|
| **The Semantic Illusion** | Hallucination detection failure modes | [arXiv:2512.15068](https://arxiv.org/abs/2512.15068) |
| **Demystifying Large Language Models** | LLM architecture survey | [IJCET](https://iaeme.com/MasterAdmin/Journal_uploads/IJCET/VOLUME_16_ISSUE_1/IJCET_16_01_180.pdf) |
| **Reinforcement Learning for Real-World Impact** | RL applications | [IJSRCET](https://ijsrcseit.com/index.php/home/article/view/CSEIT251112170/CSEIT251112170) |
| **AI in Healthcare** | Clinical ML pipelines | [IRJMETS](https://www.irjmets.com/uploadedfiles/paper//issue_2_february_2025/67992/final/fin_irjmets1740491159.pdf) |

---

## Speaking

| Event | Topic |
|-------|-------|
| **TechFutures 2025** (NYC) | [End-to-End MLOps Workshop](https://github.com/debu-sinha/techfutures-2025-mlops-databricks) |
| **Data Con LA 2022** | [Databricks Feature Store](https://www.youtube.com/watch?v=xPuCCY93BMY) |
| **Data Con LA 2021** | [Fraud Detection at Scale](https://www.youtube.com/watch?v=5SA2GT-vBvY) |
| **NYU Guest Lecture** | ML Pipelines with Apache Spark |

---

## Professional

**IEEE Senior Member** — Recognition for significant contributions to the profession (requires 10+ years experience and documented achievements)

---

## Contact

<p align="left">
<a href="https://www.linkedin.com/in/debusinha/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:debusinha2009@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ"><img src="https://img.shields.io/badge/Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white"/></a>
</p>
