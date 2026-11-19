# DSA 2050A — Week 9: Model selection and defensible evaluation

**Group name/number:** [Existing course group]  
**Members and student IDs:** [List all group members]  
**Submission:** One shared GitHub repository link per group  
**Course:** DSA 2050A Data Science Methodology  
**Week:** 9

## Group responsibilities
Complete the lab **in your existing groups**. Work together on one notebook and one repository. Record each member's concrete contribution in the table below. Each member should contribute visibly through Git commits or documented co-authored work.

| Group member | Student ID | Work completed | GitHub username or commit reference |
|---|---|---|---|
| [Name] | [ID] | [Example: evaluation pipeline] | [Username] |
| [Name] | [ID] | [Example: error analysis and README] | [Username] |

## Study objective
Explain the customer churn decision and why model selection must use development data only.

## Data statement
Synthetic fictional customer data created for teaching. No real customer records.

## Setup and reproduction
1. Open this folder in VS Code.
2. Create/select a Python environment (3.10–3.13 recommended).
3. In **Terminal → New Terminal**, run `python -m pip install -r requirements.txt`.
4. Open `notebooks/Week9_Model_Selection_Lab.ipynb` and **Select Kernel**.
5. Run each cell in order. Complete the rationale before the final-test cell.

## Prediction-time features and excluded fields
- Target: `churn` (1 = left; 0 = stayed).
- Excluded: `customer_id` (identifier), `cancellation_confirmed` (post-outcome leakage).
- Allowed features: [Explain]

## Experiments and model selection
- Primary metric chosen before comparison: **F1**.
- CV: **5-fold stratified, shuffle=True, seed=42**.
- Include the candidate comparison table from `reports/experiment_log.csv`.
- **Chosen model:** [Fill]
- **Tuned hyperparameters:** [Fill]
- **Mean/SD CV F1:** [Fill]
- **Why this choice:** [Write 100–200 words]

## Error and subgroup analysis
- Summarize confusion matrix, false negatives and false positives.
- Compare new versus established customer recall **with subgroup sample sizes**.
- Explain business implications.

## Permutation importance
- Top two features and approximate importance values.
- Explain why association is not causation.

## Final test (run once only)
- F1: [Fill] ; precision: [Fill] ; recall: [Fill]
- Compare CV vs test and discuss whether the difference is concerning.

## Limitations and ethics
- Provide at least two realistic limitations (dataset is synthetic; hidden customer dynamics; temporal drift, etc.).
- Note monitoring / human review needs before real use.

## Evidence checklist
- [ ] Executed notebook with explanations
- [ ] `reports/experiment_log.csv`
- [ ] `reports/subgroup_metrics.csv`
- [ ] `reports/permutation_importance.csv`
- [ ] `reports/frozen_selection.json` created before test
- [ ] `reports/final_metrics.json` generated once
- [ ] Two generated PNG charts
- [ ] Meaningful commits or co-authorship evidence for all group members
- [ ] Completed group contribution table with names and student IDs

## Final group review
- [ ] One team member verified the notebook runs from start to finish
- [ ] Group discussed and approved the written model-selection rationale
- [ ] No one used final-test scores to revise the model
- [ ] One representative will submit the shared URL to the course LMS

## GitHub repository URL
[Paste URL here]
# DSA2050-GROUP-LAB
