# Final Project: Feature Discovery for Predictive Analytics

## Project Overview

**The Challenge:** In predictive analytics, the features you use can make or break your models. But what if the most important features aren't obvious? In this project, you'll use unsupervised learning to discover hidden features, groups, or patterns in your data that can improve your predictions. Then, you'll build predictive models that leverage these discoveries to make better forecasts.

Think of it like this: Imagine you're opening a new coffee shop and want to predict daily sales. Instead of just using obvious features (day of week, weather), you first discover natural customer groups in your neighborhood (morning commuters, afternoon studiers, evening socializers). Once you know these groups exist, you can use "customer segment" as a feature to predict what each group will order and when they'll visit. **Feature discovery first, then better predictions.**

## Required Deliverables

### Jupyter Notebook (uploaded to GitHub)

- **Phase 1:** Feature Discovery Using Unsupervised Learning
- **Phase 2:** Building Predictive Models with Discovered Features

**Code Requirements:** Your notebook should be well-commented, organized into clear sections with markdown cells explaining your thought process, and reproducible (set random seeds where applicable). Include a final reflection section: What surprised you? What would you do differently?

### Stakeholder Report (PDF, 2-3 pages, no code, no jargon)

Brief report explaining what you found and why it matters to decision-makers

### 3-Minute Video (Loom, Zoom, or similar)

Walk through your discovery process like you're explaining to your future boss

## Dataset Requirements

- **Size:** Minimum 1,000 rows
- **Variables:** At least 8 variables (must include both numbers and categories)
- **Source:** Must be related to YOUR career field/interest
- **Originality:** Cannot be a dataset you've used in any previous assignment
- **Quality:** Real-world data (messy is okay - you'll clean it!)

**Examples of real-world data:** Customer transaction data, survey responses, sensor readings, public health records, financial market data, etc.

**Examples that don't count:** Toy datasets (Iris, Titanic), synthetic data, pre-cleaned academic datasets

**Where to find datasets:** Kaggle, government data portals (data.gov), industry associations, your company's public data, academic repositories

> **Note:** Submit your dataset choice for approval early. Include: dataset source, why it's career-relevant, and confirmation it meets size/variable requirements.

## Phase 1: Feature Discovery Using Unsupervised Learning

**Goal:** Use unsupervised learning techniques to discover new features, segments, or patterns that will improve your predictive models in Phase 2.

### What You Must Do:

#### Step 1: Data Cleaning & EDA

- Document at least 5 data quality issues you found and how you fixed them
- Create at least 4-6 visualizations showing distributions, relationships, and potential patterns (aim for 6+ for excellent work)
- Explain what you notice in plain language

#### Step 2: Unsupervised Feature Discovery

Use unsupervised learning to discover features that will improve your predictions. You must complete **ONE** of these (you may do both if you wish, but must fully complete at least one):

##### Option A: Clustering

- Try at least 3-4 different values of k (e.g., k=2, 3, 4, 5) and use the elbow method or silhouette scores to select the optimal number
- Use the elbow method or silhouette scores to help decide

**Minimum 4 visualizations required:**

1. Elbow plot or silhouette plot
2. Scatter plot showing your final clusters (color-coded)
3. At least 2 additional visualizations comparing clusters (box plots, bar charts, heatmaps showing cluster characteristics)

**Describe each cluster:** What makes this group different? Give them meaningful names that reflect their characteristics. **Think ahead:** How might cluster membership help you predict your target variable in Phase 2?

**Examples of good cluster names:**
- ✅ "Budget-conscious families" (not "Cluster 1")
- ✅ "Premium business travelers" (not "High-value customers")
- ✅ "Occasional weekend shoppers" (not "Low-frequency segment")

**Examples of poor cluster names:**
- ❌ "Cluster 1", "Cluster 2"
- ❌ "High-value customers" (too generic)
- ❌ "Group A" (not descriptive)

##### Option B: PCA (Principal Component Analysis)

- Reduce your features to find the main patterns
- Show how much variance each component explains

**Minimum 4 visualizations required:**

1. Scree plot (variance explained)
2. Cumulative variance plot
3. Biplot or component loading visualization
4. Scatter plot of data in PC space (first 2-3 components)

**Interpret what each component means:** What real-world characteristic does it represent? **Think ahead:** How might these principal components help you predict your target variable in Phase 2?

> **Critical Requirement:** You must explain what you discovered in words a non-technical person would understand. What hidden groups or patterns exist in your data? **Most importantly:** How will these discoveries help you make better predictions?

> **Important Note:** If your initial unsupervised analysis doesn't reveal clear patterns, document this! Try different preprocessing (scaling, feature selection) or different methods. Sometimes discovering "no clear patterns" is valuable learning. Explain why patterns might not exist in your data and what this means for your predictive models.

## Phase 2: Building Predictive Models with Discovered Features

**Goal:** Build predictive models that leverage the features you discovered in Phase 1 to make accurate predictions about future outcomes.

### What You Must Do:

#### Step 3: Integrate Discovered Features into Predictive Models

Take the features you discovered in Phase 1 (cluster memberships, principal components, or derived features) and integrate them into your predictive models. You have options:

**If you did clustering:**

- Add cluster membership as a new feature in your prediction models
- **OR** predict within each cluster separately
- **OR** use clusters to create new engineered features (e.g., "distance from cluster center")

**If you did PCA:**

- Use principal components as features in your models
- **OR** create new features based on what the components represent
- **OR** stratify your analysis based on component scores

You may create new features based on your discoveries (e.g., "distance from cluster center", "component scores"). Document any feature engineering you perform.

#### Step 4: Build Predictive Models

Build at least 3 different predictive models. Your problem will determine which type:

**For Regression Problems (predicting a number):**

- **Required:** Linear Regression or Multiple Regression (baseline)
- **Required:** At least one ensemble method (Random Forest Regressor, Bagging, Gradient Boosting, or other ensemble techniques)
- **Required:** One additional model from: Decision Tree Regressor or another ensemble method

**For Classification Problems (predicting a category):**

- **Required:** Logistic Regression (baseline)
- **Required:** At least one ensemble method (Random Forest Classifier, Bagging, Gradient Boosting, or other ensemble techniques)
- **Required:** One additional model from: Decision Tree Classifier or another ensemble method

**Optional:**

- Mix regression and classification if your project naturally requires both
- Use multiple ensemble methods to compare their approaches

**Evaluation Metrics:** Report appropriate metrics for your problem type:

- **For regression:** R², MAE (Mean Absolute Error), RMSE (Root Mean Squared Error)
- **For classification:** Accuracy, Precision, Recall, F1-score, and a confusion matrix

#### Step 5: Show the Impact

Compare models that DON'T use your Phase 1 discoveries vs. models that DO use them.

**Methodology:**

- Use the same train/test split for fair comparison
- Include a baseline model (no Phase 1 features) for comparison
- Report at least 2-3 appropriate metrics (see Step 4 for metric requirements)

Create a comparison table showing performance metrics for all models.

**Explain:** Did your unsupervised insights actually help? Quantify the improvement: Did accuracy improve by 5%? Did RMSE decrease by 10%? If your discoveries didn't help, explain why (this is still valuable learning!).

## Stakeholder Report Requirements

- **Audience:** Decision-makers in your field who don't know data science
- **Length:** 2-3 pages (brief and focused)

### Required Sections:

#### Executive Summary

- What you studied and why it matters
- Your main feature discovery from Phase 1
- How those features improved your predictions in Phase 2
- Your recommendation based on the predictive models

#### The Feature Discovery

- What features, groups, or patterns did you discover using unsupervised learning?
- Show visualizations (with clear labels and titles)
- How do these discoveries relate to what you're trying to predict?
- Why should your audience care about these features?

#### The Predictive Models

- What were you trying to predict?
- Which predictive model worked best and why?
- How did your Phase 1 feature discoveries improve prediction accuracy?
- Show before/after comparison of model performance

#### Business Recommendations

- What should your organization do with this information?
- Give 3-5 specific, actionable recommendations

#### Limitations & Next Steps

- What are the weaknesses of your analysis?
- What would you do with more time/data/resources?

### Writing Guidelines:

- No code
- No jargon (or define it immediately)
- Use visuals to tell your story
- Write at a level your parents/siblings could understand

## Video Requirements (Loom, Zoom, or similar)

- **Length:** Exactly 3 minutes (2:45 - 3:15 acceptable)

### What to Cover:

1. **The Setup (30 seconds):** What are you trying to predict and why does it matter?
2. **The Feature Discovery (1 minute):** What features did you discover using unsupervised learning? Show key visualizations
3. **The Predictive Models (1 minute):** How did those discovered features improve your prediction accuracy? Show before/after comparison
4. **The Recommendation (30 seconds):** What should someone do with your predictive insights?

### Tips:

- Practice first! You need to be concise
- Screen-share your key visuals
- Speak clearly and enthusiastically
- Imagine you're presenting to a hiring manager

## Common Mistakes to Avoid

- ❌ Doing predictive modeling first, then clustering - **Feature discovery comes FIRST**
- ❌ Not explaining what your clusters/components mean or how they'll help predictions - Numbers aren't insights
- ❌ Building predictive models without using Phase 1 discovered features - You must integrate the features you discovered
- ❌ Writing your report like a technical paper - Your audience doesn't know statistics
- ❌ Rambling in your video - Practice to stay within 3 minutes
- ❌ Using a dataset that's too clean - Real data is messy, show you can handle it
- ❌ Forgetting to show if your discoveries actually helped - Always compare before/after
- ❌ Skipping required visualizations - You need all 4+ for Phase 1
- ❌ Not including an ensemble method - Random Forest, Bagging, or Gradient Boosting is required
- ❌ Not setting random seeds - Your code should be reproducible
- ❌ Using different train/test splits for comparison - Use the same split for fair comparison
- ❌ Not quantifying improvements - Say "accuracy improved by 5%" not just "it got better"

## Ethical Considerations

Consider the ethical implications of your analysis:

- If working with personal data, discuss privacy considerations
- If making recommendations, consider potential biases or unintended consequences
- Acknowledge limitations of your data and methods

## Submission Instructions

Submit via GitHub:

- Repository must be named: `final-project-unsupervised-[YourLastName]`
- Include: notebook (.ipynb), data files or link to data, stakeholder report (PDF)
- In README file: include link to your video

---

## Quick Reference Checklist

Use this checklist to ensure you've completed all requirements:

### Dataset & Setup:
- [ ] Dataset selected and approved (1000+ rows, 8+ variables, career-relevant, real-world data)
- [ ] Dataset meets originality requirement (not used in previous assignments)

### Phase 1: Feature Discovery Using Unsupervised Learning
- [ ] 5+ data quality issues documented and fixed
- [ ] 4-6+ EDA visualizations created (distributions, relationships, patterns)
- [ ] Unsupervised method completed (clustering OR PCA, or both)
- [ ] For clustering: Tried 3-4+ different k values, used elbow/silhouette method
- [ ] For clustering: 4+ required visualizations (elbow/silhouette plot, scatter plot, 2+ comparison visualizations)
- [ ] For PCA: 4+ required visualizations (scree plot, cumulative variance, biplot/loadings, PC space scatter)
- [ ] Discovered features interpreted in plain language with meaningful names
- [ ] Clusters/components connected to real-world meaning and explained how they'll help predictions

### Phase 2: Building Predictive Models with Discovered Features
- [ ] Phase 1 discovered features integrated into predictive models (as features, separate models, or engineered features)
- [ ] 3+ predictive models built (including required baseline and ensemble method)
- [ ] Appropriate evaluation metrics reported (R²/MAE/RMSE for regression, accuracy/precision/recall/F1 for classification)
- [ ] Before/after comparison completed (same train/test split, baseline model without Phase 1 features included)
- [ ] Prediction improvement quantified and explained (improvement percentages, or explanation if no improvement)

### Notebook Quality:
- [ ] Well-commented code
- [ ] Clear markdown sections explaining thought process
- [ ] Random seeds set for reproducibility
- [ ] Final reflection section included

### Stakeholder Report:
- [ ] 2-3 pages (brief and focused)
- [ ] All required sections present (Executive Summary, Feature Discovery, Predictive Models, Business Recommendations, Limitations & Next Steps)
- [ ] No code, no jargon (or jargon defined)
- [ ] 3-5 specific, actionable recommendations
- [ ] Visualizations included with clear labels and titles

### Video:
- [ ] 2:45-3:15 minutes in length
- [ ] All 4 required elements covered (Setup, Discovery, Impact, Recommendation)
- [ ] Clear audio and visuals
- [ ] Link included in GitHub README

### Submission:
- [ ] GitHub repository properly named: `final-project-unsupervised-[YourLastName]`
- [ ] All files included (notebook, data or data link, stakeholder report PDF)
- [ ] README includes video link
