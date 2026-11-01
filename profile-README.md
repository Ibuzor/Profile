# Hi, I'm Ibuzor 

I recently completed the MIT Professional Education Applied AI and Data Science Program and am now studying software development with an AI focus at NBI Handelsakademin. My work so far is in classification modeling for regulated settings, where a prediction has to come with a reason a person can read and defend.

## Featured project

### Home Equity Loan Default Prediction

A classification model that predicts default on home equity loans, built for a bank that has to justify every rejection under the Equal Credit Opportunity Act (ECOA). This was my capstone for the MIT program.

- **Data:** the HMEQ dataset, 5,960 loan records with about a 20% default rate.
- **Models compared:** logistic regression as a baseline, a decision tree, a random forest, an Explainable Boosting Machine, and XGBoost with monotonic constraints on key features so its behavior can be defended to a regulator.
- **Metric choice:** I judged models on recall, precision, F1 and ROC-AUC instead of accuracy. Approving a borrower who later defaults costs the bank more than rejecting a reliable one, so missed defaulters were weighted more heavily.
- **Missing data:** missing values in DEBTINC and VALUE were strongly linked to default, so I kept binary missingness indicators as features instead of imputing them away.
- **Explanations:** SHAP values give feature-level reasons for each prediction. A retrieval-based generator then drafts adverse action notices from those values, using the reason codes in Regulation B (12 CFR Part 1002, Appendix C).
- **Result:** XGBoost with monotonic constraints was my recommended model, chosen for its recall under the cost asymmetry above.
- **Grade:** 94/100 overall (milestone 20/20, final submission 40/40, live presentation 34/40).

**Tools:** Python, pandas, scikit-learn, XGBoost, SHAP, sentence-transformers, Anthropic API

[View repository](https://github.com/Ibuzor/Loan-Default-Prediction)

## Technical toolbox

| Category | Technologies |
| --- | --- |
| Languages | Python (pandas, NumPy, scikit-learn) |
| Modeling and interpretation | XGBoost, Random Forest, SHAP, class-imbalance handling, threshold tuning |
| Text and LLM work | sentence-transformers, retrieval-based generation, Anthropic API |
| Visualization | Matplotlib, Seaborn |
| Tools | Git, GitHub, Google Colab, Jupyter Notebooks |

## Projects I plan to build

I haven't started these yet.

- **Customer churn prediction.** A pipeline on historical customer behavior data to find high-risk segments, likely using random forests and XGBoost.
- **Retail image classification.** A convolutional neural network to sort product images into inventory categories, with data augmentation and transfer learning.

## Education

- Software Developer with an AI specialization, NBI Handelsakademin
- Applied AI and Data Science Program, MIT Professional Education
- IT Project Management, IT Högskolan

## Contact

- LinkedIn: [linkedin.com/in/ibuzor](https://linkedin.com/in/ibuzor)
- Email: [ibuzor@gmail.com](mailto:ibuzor@gmail.com)
