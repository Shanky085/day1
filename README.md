# FlyRank Machine Learning Engineering Internship

A portfolio repository documenting my work during the **FlyRank Machine Learning Engineering Internship**.

The project focused on **Refresh / Content Opportunity Scoring**: using observed content and search-performance signals to prioritize pages for human review for a possible content refresh.

## Capstone

**Research paper:** https://shanky085.github.io/day1/

**Repository:** https://github.com/Shanky085/day1

**Lane:** Lane 2 — Refresh / Content Opportunity Scoring

### Key result

I compared a simple Week-4 rule-based baseline with a Logistic Regression model using an anonymized content-refresh dataset.

| Method | Average Precision | ROC-AUC |
|---|---:|---:|
| W04 baseline rule | 0.4974 | 0.4644 |
| Logistic Regression | 0.5582 | 0.5621 |

The final evaluation used an 80/20 client-grouped split with **zero client overlap** between training and test sets. These results are treated as measured, directional evidence for decision-support rather than proof of causal refresh impact.

## Completed Track Work

- ✅ **Week 1 — Research question**  
  Defined the search/content problem and the initial analysis direction.

- ✅ **Week 2 — ML task framing**  
  Converted the problem into a concrete ML task with an explicit target and decision use case.

- ✅ **Week 3 — Data contract**  
  Defined the data grain, time-window assumptions, validation checks, features, and a deliberate leakage experiment.

- ✅ **Week 4 — Baseline scoring**  
  Built and audited a simple rule-based action score with reason codes and ranked recommendations.

- ✅ **Week 5 — Modeling**  
  Trained and evaluated Logistic Regression and compared it with the Week-4 baseline on the same evaluation design.

- ✅ **Week 6 — Validation & leakage audit**  
  Audited validation design, feature leakage, failure modes, and claim strength using grouped validation.

- ✅ **Week 7 — Action playbook**  
  Converted model/signal output into ranked refresh, monitor, and leave actions with human-review rules and no-go cases.

- ✅ **Week 8 — Research paper & showcase**  
  Built and deployed the final research paper on GitHub Pages, then added a 5-minute demo outline plus social and employer-facing shareable summaries.

## Notebooks

| Week | Notebook | Focus |
|---|---|---|
| W01 | [`w01_research_question.ipynb`](work/notebooks/w01_research_question.ipynb) | Research question |
| W02 | [`w02_ml_task_framing.ipynb`](work/notebooks/w02_ml_task_framing.ipynb) | ML task framing |
| W03 | [`w03_data_contract.ipynb`](work/notebooks/w03_data_contract.ipynb) | Data contract |
| W03 | [`w03_feature_leakage_check.ipynb`](work/notebooks/w03_feature_leakage_check.ipynb) | Leakage check |
| W04 | [`w04_baseline_score.ipynb`](work/notebooks/w04_baseline_score.ipynb) | Baseline action score |
| W04 | [`w04_signal_audit.ipynb`](work/notebooks/w04_signal_audit.ipynb) | Signal audit |
| W05 | [`w05_model.ipynb`](work/notebooks/w05_model.ipynb) | Model training and comparison |
| W06 | [`w06_validation_audit.ipynb`](work/notebooks/w06_validation_audit.ipynb) | Validation and leakage audit |
| W07 | [`w07_action_playbook.ipynb`](work/notebooks/w07_action_playbook.ipynb) | Action playbook |
| Capstone | [`capstone.ipynb`](work/notebooks/capstone.ipynb) | Final research workflow and showcase material |

## Research Approach

The capstone follows a deliberately conservative workflow:

**Question → Data Contract → Baseline → Model → Validation → Leakage Audit → Action Playbook → Research Paper**

The final recommendations are intended for **human decision-support**. The system does not automatically publish, rewrite, delete, redirect, or change production SEO settings.

## Repository Structure

```text
.
├── docs/                         # Deployed research paper and supporting docs
├── submission/                   # Final submission metadata
│   └── paper_url.txt             # Exact deployed paper URL
├── work/
│   ├── notebooks/                # Weekly notebooks + capstone
│   ├── figures/                  # Reusable research figures
│   └── outputs/                  # Regenerable outputs / metrics receipts
└── scripts/                      # Reference pipeline utilities
```

## Public-Safety & Reproducibility

The public artifact uses the anonymized internship dataset and avoids exposing client names, private queries, private URLs, credentials, or raw identifying exports. Historical notebooks remain available in `work/notebooks/` so the research process can be inspected and reproduced.

## Data Credit

**Built on the FlyRank ML Internship dataset.**  
https://flyrank.ai

## Author

**Shanky Pal**  
B.Tech CSE (AI/ML)
