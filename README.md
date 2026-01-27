# Hey, I'm Debu Sinha

**Lead Applied AI/ML Engineer (Solutions Architecture)** @ Databricks | Author | Open Source Contributor

Building ML platforms at scale. Helping enterprises ship AI from prototype to production.

---

## Tech Stack

<p align="left">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white"/>
<img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white"/>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"/>
<img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
</p>

---

## Book

<a href="https://www.amazon.com/dp/1801812039">
<img src="https://m.media-amazon.com/images/I/71z5VfSjNQL._SY466_.jpg" alt="Practical Machine Learning on Databricks" width="150" align="left" style="margin-right: 15px;"/>
</a>

### [Practical Machine Learning on Databricks](https://www.amazon.com/dp/1801812039)
**Packt Publishing, 2023** | 244 pages

End-to-end guide for building production ML systems on Databricks - from data engineering to MLOps. Reached best seller status in its category within 2 weeks of release.

<br clear="left"/>

---

## Research

<a href="https://scholar.google.com/citations?user=V2LfrPwAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white"/></a>  **Research Affiliate, Johns Hopkins University**

### AI Reliability Under Distribution Shift

A research program examining how AI systems fail when deployment conditions differ from training/calibration:

| Paper | Focus | arXiv |
|-------|-------|-------|
| **The Semantic Illusion** | Embedding-based hallucination detection fails on RLHF outputs (95% coverage to 100% FPR) | [2512.15068](https://arxiv.org/abs/2512.15068) |

### Other Publications

| Paper | Venue |
|-------|-------|
| [Demystifying Large Language Models](https://iaeme.com/MasterAdmin/Journal_uploads/IJCET/VOLUME_16_ISSUE_1/IJCET_16_01_180.pdf) | IJCET |
| [Reinforcement Learning for Real-World Impact](https://ijsrcseit.com/index.php/home/article/view/CSEIT251112170/CSEIT251112170) | IJSRCET |
| [AI in Education: Opportunities and Challenges](https://iaeme.com/MasterAdmin/Journal_uploads/IJRCAIT/VOLUME_8_ISSUE_1/IJRCAIT_08_01_233.pdf) | IAEME |
| [AI in Healthcare: Data to Patient Outcomes](https://www.irjmets.com/uploadedfiles/paper//issue_2_february_2025/67992/final/fin_irjmets1740491159.pdf) | IRJMETS |

---

## Open Source Contributions

### MLflow Core Contributor

Active contributor to [**MLflow**](https://github.com/mlflow/mlflow) (23K+ stars) - the leading open-source ML lifecycle platform.

#### Third-Party Scorer Ecosystem

Building integrations that connect MLflow's GenAI evaluation with major LLM evaluation frameworks:

| Integration | Status | PR | Ecosystem Reach |
|-------------|--------|-----|-----------------|
| **Phoenix (Arize)** | Merged | [#19473](https://github.com/mlflow/mlflow/pull/19473) | 500K+ monthly downloads |
| **TruLens** | In Review | [#19492](https://github.com/mlflow/mlflow/pull/19492) | 100K+ monthly downloads |
| **Guardrails AI** | In Review | [#20038](https://github.com/mlflow/mlflow/pull/20038) | 200K+ monthly downloads |

#### UV Package Manager Support

Native [UV](https://github.com/astral-sh/uv) integration for MLflow model logging - automatic dependency inference for UV-managed projects:

| Feature | PR | Description |
|---------|-----|-------------|
| UV Support (Phase 1 + 2) | [#20344](https://github.com/mlflow/mlflow/pull/20344) | Auto-detection, `uv export`, dependency groups, UV sync |

[Design Doc](https://github.com/debu-sinha/design-docs/blob/main/mlflow/uv-support-design-doc-v2.md) | [UV Issue #17702](https://github.com/astral-sh/uv/issues/17702)

#### Other Contributions

| PR | Feature | Status |
|----|---------|--------|
| [#19152](https://github.com/mlflow/mlflow/pull/19152) | `inference_params` for LLM Judges (temperature, top_p) | Merged |
| [#19248](https://github.com/mlflow/mlflow/pull/19248) | Configurable parallelism (`MLFLOW_GENAI_EVAL_MAX_SCORER_WORKERS`) | Merged |

### MLflow-Modal Plugin

[![PyPI](https://img.shields.io/pypi/v/mlflow-modal?style=flat-square)](https://pypi.org/project/mlflow-modal/)

Serverless GPU deployment for MLflow models on [Modal](https://modal.com):

```bash
pip install mlflow-modal
mlflow deployments create -t modal -m models:/my-model/1 --name my-deployment
```

- Auto-scaling from zero to thousands of GPUs (T4 to H200)
- Sub-second cold starts with Modal's container snapshots
- Native MLflow deployment interface

[GitHub](https://github.com/debu-sinha/mlflow-modal-deploy) | [PyPI](https://pypi.org/project/mlflow-modal/)

---

## Speaking

- **TechFutures 2025** (NYC) - End-to-End MLOps Pipelines Workshop ([GitHub](https://github.com/debu-sinha/techfutures-2025-mlops-databricks))
- **Data Con LA 2022** - Simplifying AI/ML using Databricks Feature Store ([YouTube](https://www.youtube.com/watch?v=xPuCCY93BMY))
- **Data Con LA 2021** - Detecting Fake Reviews at Scale using Spark and John Snow Labs ([YouTube](https://www.youtube.com/watch?v=5SA2GT-vBvY))
- **NYU Guest Lecture** - ML Pipeline with Apache Spark

---

## Professional Memberships

<p align="left">
<img src="https://img.shields.io/badge/IEEE-Senior_Member-00629B?style=flat-square&logo=ieee&logoColor=white"/>
<img src="https://img.shields.io/badge/IETE-Fellow-blue?style=flat-square"/>
<img src="https://img.shields.io/badge/IAEME-Fellow-green?style=flat-square"/>
</p>

---

## Connect

<p align="left">
<a href="https://www.linkedin.com/in/debusinha/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:debusinha2009@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

---

<p align="left">
<img src="https://komarev.com/ghpvc/?username=debu-sinha&color=blueviolet&style=flat-square&label=Profile+Views"/>
</p>
