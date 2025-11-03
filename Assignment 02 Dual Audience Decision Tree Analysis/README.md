# Dual-Audience Decision Tree Analysis

## Assignment Overview
You will build and evaluate decision tree models using a dataset from your industry, then document your work in a single Jupyter notebook with TWO distinct sections explaining your analysis to different audiences. This reflects real-world data analyst work: communicating technical details to your data team AND translating findings into actionable insights for business leaders.

---

## Assignment Structure: Single Jupyter Notebook

Your notebook should contain these sections in order:

### Section 1: Technical Analysis & Code

Build three decision tree models with different max_depth parameters:
- Shallow tree: max_depth = 3
- Medium tree: max_depth = 5  
- Deep tree: max_depth = 10

**Required elements:**
- Dataset loading and basic exploration
- Train/test split (80/20)
- Three separate models with different depths
- Accuracy scores for training AND test data for each model
- Confusion matrices for all three models
- Visualizations of all three trees (or at least shallow and medium if deep tree is too large)
- Feature importance chart for your final chosen model

---

### Section 2: Technical Stakeholder Report

Use markdown cells to write a report for your data science team, analytics manager, or technical colleagues.

**Required content (in markdown cells):**

1. **Dataset & Prediction Goal** - What you're predicting and why it matters
2. **Methodology Summary** - Explain your train/test split and three depth settings tested
3. **Model Performance Comparison** - Discuss the accuracy scores (training vs test) for all three depths. What patterns do you see?
4. **Overfitting Analysis** - Which model(s) show signs of overfitting? How can you tell from the training vs test accuracy? What does this mean for model selection?
5. **Tree Structure Comparison** - Describe what you notice when comparing the visualizations of different depth trees
6. **Technical Recommendation** - Which depth did you select as optimal and why? Discuss the bias-variance tradeoff.

**Tone & Language:** Use technical terminology (overfitting, accuracy, hyperparameters, train/test split, bias-variance tradeoff). Your audience understands machine learning.

---

### Section 3: Non-Technical Stakeholder Report

Use markdown cells to write a separate report for business managers or executives with NO machine learning background.

**Required content (in markdown cells):**

1. **Business Question** - What problem are you solving? (Avoid terms like "decision tree model")
2. **Key Findings** - What are the top 3 factors that predict your target? Explain in plain language what your simplified tree visualization shows
3. **Performance Summary** - "Our analysis correctly predicts [target] X% of the time" - translate your accuracy into business terms
4. **Real-World Example** - Walk through one actual prediction using your tree as a decision flowchart. "If a customer has X and Y, then we predict Z"
5. **Business Recommendations** - Provide 2-3 specific, actionable recommendations based on your findings
6. **Limitations** - In simple terms, what should business leaders know about when this analysis might not be accurate?

**Tone & Language:** Clear, jargon-free language. Replace "accuracy" with "correct predictions," "features" with "factors," "model" with "analysis." Use analogies and plain explanations.

---

### Section 4: Reflection

Write 2-3 paragraphs answering: "What was most challenging about translating technical findings for a non-technical audience? What strategies did you use to simplify complex concepts?"

---

## Deliverable
Consider this assignment part of your online portfolio to showcase your skills to prospective employers.

In Blackboard/Canvas: Submit a link to your GitHub repo.

In your repo:
1. Create a new folder: Dual Audience Decision Tree Analysis
2. Add an appropriate README.md explaining the project/analysis (the lay of the land). HINT: Ask ChatGPT what makes a good README.md
3. A single .ipynb file (Jupyter notebook) containing all four sections.

---

## Tips for Success

- **Use markdown headers clearly** - Label each section so it's obvious when you're switching audiences
- **Technical report:** Show your thinking. Explain WHY you made decisions, not just WHAT you found
- **Non-technical report:** Imagine explaining this to a store manager or family member. Would they understand?
- **The "grandmother test":** If your grandmother couldn't understand your non-technical section, revise it
- **Keep visualizations** - Include the same charts in both sections but explain them differently for each audience
