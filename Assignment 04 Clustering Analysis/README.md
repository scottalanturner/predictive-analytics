# Assignment 4: Clustering Analysis & Industry Segmentation

## Assignment Overview
You will apply clustering analysis to segment entities (customers, products, companies, markets, etc.) from your industry and develop actionable personas and strategies for each segment. This assignment focuses on **unsupervised learning**—finding patterns in data without predefined labels—and translating those patterns into business insights.

The goal is to understand how clustering can reveal natural groupings in your industry data and how to communicate those findings to decision-makers through personas and action plans.

---

## Dataset Options

You have two choices for this assignment:

### Option A: Continue with Your Industry Dataset (Recommended)
- Use the same dataset and target variable from a previous supervised assignment (e.g., decision trees, ensembles)
- This allows you to compare labeled outcomes with your new clustering results
- You already understand the business context and features

### Option B: Choose a New Industry Dataset
- Select a dataset from your current or target industry
- Must have at least 500 observations, 5+ features, **and a clear label/target column** that represents the business outcome you originally care about
- Must be appropriate for clustering analysis (entities that can be grouped)
- Document why this dataset is relevant to your field and how the original label is used in practice

**Approved Dataset Sources:**
- Your organization's data (with permission and proper anonymization)
- Kaggle datasets related to your industry
- UCI Machine Learning Repository
- Industry-specific public datasets (healthcare.gov, SEC filings, etc.)

**Important:** Avoid overused datasets (Iris, Wine, etc.). Choose something that reflects real work in your field.

---

## Assignment Structure: Single Jupyter Notebook

Your notebook should contain these sections in order:

### Section 1: Data Preparation & Setup

**Required elements:**
- Load your dataset
- Basic data exploration (shape, columns, data types)
- Brief explanation of what entities you're clustering, what the original label represents, and why segmentation matters for your industry
- Handle missing values and select relevant features for clustering
- Standardize/normalize features (required for K-means)
- Brief explanation of why standardization is necessary

---

### Section 2: Labeled Baseline Review

Because most industry datasets already contain labeled outcomes, start by grounding your clustering work in the existing supervised problem.

**Required elements:**
- Describe the original target variable and why it matters
- Summarize the features/engineering choices you used (or would use) for the supervised task
- Reproduce or cite performance metrics from your earlier supervised model (accuracy, F1, RMSE, etc.)
- Provide a confusion matrix or error analysis snippet that highlights where the supervised model succeeds/fails
- 150-word reflection on how well the labeled model captures the business reality and where it falls short (motivation for clustering)

---

### Section 3: Optimal K Selection

**3.1 Elbow Method**
- Plot the within-cluster sum of squares (WCSS) for K values from 2 to 10 (or appropriate range)
- Identify the "elbow" point
- Explain what the elbow method shows and what you observe

**3.2 Silhouette Score Analysis**
- Calculate silhouette scores for the same range of K values
- Plot silhouette scores vs. K
- Identify the K with the highest silhouette score
- Explain what silhouette score measures and what your results indicate

**3.3 K Selection Decision** (100-150 words)
- Compare the results from both methods
- Document which K value you chose and why
- If the methods disagree, explain your reasoning for choosing one over the other
- Consider business context: Is the chosen K practical for your industry application?

**Note:** Gap statistic is optional for extra credit. If you use it, include it in this section.

---

### Section 4: K-Means Clustering

**4.1 Build Final Model**
- Apply K-means with your chosen K value
- Fit the model to your standardized data
- Assign cluster labels to your data

**4.2 Cluster Characterization**
- For each cluster, create a summary including:
  - **Size**: Number of entities in the cluster (count and percentage)
  - **Key Characteristics**: Statistical summary (mean, median) of each feature for this cluster
  - **Distinguishing Factors**: What makes this cluster unique compared to others? Which features are notably higher/lower?
- Present this as a clear table or summary statistics

**4.3 Representative Examples**
- Show 2-3 actual entities (rows) from each cluster
- Explain why these examples are representative of their cluster

---

### Section 5: PCA Visualization

**5.1 Apply PCA**
- Use PCA to reduce your features to 2-3 principal components
- Explain what PCA does and why it's useful for visualization
- Report the explained variance ratio for your principal components

**5.2 Visualize Clusters**
- Create a 2D scatter plot (or 3D if using 3 components) showing:
  - Each point colored by its cluster assignment
  - Clear legend and labels
  - Title explaining what the visualization shows
- Interpret the plot: Do clusters appear well-separated? Are there any overlapping regions?

**5.3 PCA Interpretation** (100-150 words)
- What does the visualization tell you about your clusters?
- How well does the 2D/3D representation capture the true cluster structure?
- Are there any surprises or patterns visible in the plot?

---

### Section 6: Compare Clusters to Original Labels

Clustering is most powerful when you can articulate how the unsupervised structure aligns (or conflicts) with your labeled outcomes.

**6.1 Alignment Analysis**
- Create a crosstab/heatmap showing the distribution of original labels across clusters
- Calculate at least one alignment metric (e.g., purity, adjusted Rand index, normalized mutual information)
- Identify where clusters reinforce or contradict the original labeling

**6.2 Interpretation** (200-250 words)
- What new patterns emerge that the original labeled approach missed?
- Are there labeled categories that split into multiple meaningful clusters?
- Where do clusters mix multiple labels, and what might that mean operationally?
- Discuss at least one business decision that would change based on the clustering insight.

---

### Section 7: Segment Personas & Action Plans

For each cluster, create:

**7.1 Persona** (200-250 words per cluster)
- Give the cluster a memorable, descriptive name (e.g., "High-Value Loyalists," "Price-Sensitive Explorers")
- Describe a "typical" member of this segment as if you're creating a marketing persona
- Include key characteristics, behaviors, and what makes them distinct
- Write this in a way that a business manager could understand and use

**7.2 Action Plan** (150 words per cluster)
- Develop specific strategies or actions relevant to your industry for this segment
- Be concrete and actionable—what should the organization do differently for this segment?
- Connect back to the distinguishing characteristics you identified

**Career-Specific Examples:**
- **Healthcare**: Patient segments with different care needs and intervention strategies
- **Retail**: Customer segments with tailored marketing and product recommendations
- **Finance**: Client segments with different service offerings and risk profiles
- **Manufacturing**: Product clusters with different production/distribution strategies
- **Education**: Student segments requiring different support interventions

---

### Section 8: Reflection

Write 2-3 paragraphs (200-300 words) answering:
- What was most surprising about the clusters you discovered?
- How well do the clusters align with your prior understanding of your industry?
- What business value does this segmentation provide?
- What limitations or challenges did you encounter with clustering?
- How might you use clustering in your future work?

---

## Submission Requirements

Submit via Blackboard with GitHub repository URL containing:

### Required Files:

1. **`clustering_analysis.ipynb`** - Single Jupyter notebook containing all eight sections:
   - All code cells executed with outputs visible
   - Clear markdown cells explaining your process and findings
   - All sections completed in order, including personas/action plans within the notebook

2. **`README.md`** - Brief description including:
   - Your industry/domain
   - Dataset description and source
   - Brief summary of your findings (2-3 sentences)

### GitHub Repository Structure:
```
your-portfolio-repo/
├── Assignment 04 Clustering Analysis/
│   ├── README.md
│   ├── clustering_analysis.ipynb
│   └── data/
│       └── your_dataset.csv (if not too large and permissible)
```

### Submission Process:
1. Push all files to your GitHub repository
2. Ensure repository is public or add instructor as collaborator
3. Submit repository URL via Blackboard assignment link
4. Include a comment with your industry/domain

---

## Tips for Success

- **Focus on interpretation, not just clustering** - The technical clustering is important, but showing you understand what the clusters mean is crucial
- **Be specific about your industry** - Generic personas won't earn full credit. Connect everything back to your field
- **Keep clusters manageable** - 2-4 clusters is usually ideal. Too many clusters become hard to interpret and act upon
- **Use PCA visualization effectively** - The plot should help tell the story of your clusters, not just be a requirement
- **Make personas actionable** - A good persona helps decision-makers understand who they're targeting. Be concrete
- **Test everything** - Restart your kernel and run all cells before submitting. Broken code earns zero credit
- **Write for clarity** - Your explanations should be understandable to someone who doesn't know machine learning
- **Connect analysis to business value** - Always ask: "So what?" Why does this segmentation matter for your industry?

