# Module 5: Exploratory Data Analysis (EDA)

This module provides comprehensive training in Exploratory Data Analysis, covering fundamental concepts, statistical techniques, and data storytelling. The module consists of five interactive Jupyter notebooks designed to build expertise in understanding and communicating data insights.

## 📚 Module Overview

**Learning Objectives:**
- Master systematic EDA workflows and best practices
- Apply statistical analysis techniques for pattern detection
- Create compelling data visualizations and stories
- Understand the critical importance of visualization in data analysis

**Prerequisites:**
- Basic Python programming knowledge
- Familiarity with pandas and matplotlib
- Understanding of basic statistical concepts

## Getting Started

### Option 1: GitHub
Click on any of the GitHub links above to view the notebooks directly in GitHub's notebook viewer.

### Option 2: Google Colab
1. Click on any "Open in Colab" link above
2. The notebook will open in Google Colab
3. You can run, edit, and save your work in the cloud

### Option 3: Local Development
1. Clone this repository: `git clone https://github.com/scottalanturner/predictive-analytics.git`
2. Install Jupyter: `pip install jupyter`
3. Navigate to the Module 5 EDA directory and run: `jupyter notebook`

## 📖 Notebook Contents

### 1. [EDA Section 1: Fundamentals](eda-section1-fundamentals.ipynb)
- **GitHub**: [eda-section1-fundamentals.ipynb](eda-section1-fundamentals.ipynb)
- **Google Colab**: [Open in Colab](https://colab.research.google.com/github/scottalanturner/predictive-analytics/blob/main/Module%205%20EDA/eda-section1-fundamentals.ipynb)

**Focus:** EDA Workflow and Visualization Templates

**Key Topics:**
- Complete 5-step EDA workflow demonstration
- Setting up reusable visualization templates
- Custom style configuration and color palettes
- Template functions for numeric and categorical analysis

**Learning Outcomes:**
- Understand systematic approach to exploring any dataset
- Create professional, consistent visualizations
- Build reusable analysis templates for efficiency

### 2. [EDA Section 2: Core Analysis Techniques](eda-section2-notebook.ipynb)
- **GitHub**: [eda-section2-notebook.ipynb](eda-section2-notebook.ipynb)
- **Google Colab**: [Open in Colab](https://colab.research.google.com/github/scottalanturner/predictive-analytics/blob/main/Module%205%20EDA/eda-section2-notebook.ipynb)

**Focus:** Univariate and Bivariate Analysis

**Key Topics:**
- Univariate analysis for numeric and categorical variables
- Distribution analysis (skewness, kurtosis, normality testing)
- Bivariate analysis and correlation techniques
- Correlation matrix analysis and heatmap visualization

**Learning Outcomes:**
- Master visualization methods for different data types
- Understand distribution characteristics and statistical tests
- Identify relationships between variables

### 3. [EDA Section 3: Statistical Analysis & Pattern Detection](eda-section3-notebook.ipynb)
- **GitHub**: [eda-section3-notebook.ipynb](eda-section3-notebook.ipynb)
- **Google Colab**: [Open in Colab](https://colab.research.google.com/github/scottalanturner/predictive-analytics/blob/main/Module%205%20EDA/eda-section3-notebook.ipynb)

**Focus:** Advanced Statistical Techniques

**Key Topics:**
- Normality testing and assumption checking
- Group comparison methods (t-tests, ANOVA, non-parametric alternatives)
- Confidence intervals and effect size calculations
- Outlier detection techniques
- Principal Component Analysis (PCA) for pattern detection

**Learning Outcomes:**
- Choose appropriate statistical tests based on data characteristics
- Understand the importance of effect size beyond p-values
- Detect anomalies and hidden patterns in data

### 4. [EDA Section 4: Communication & Storytelling](eda-section4-notebook.ipynb)
- **GitHub**: [eda-section4-notebook.ipynb](eda-section4-notebook.ipynb)
- **Google Colab**: [Open in Colab](https://colab.research.google.com/github/scottalanturner/predictive-analytics/blob/main/Module%205%20EDA/eda-section4-notebook.ipynb)

**Focus:** Data Visualization and Storytelling

**Key Topics:**
- Data storytelling fundamentals and narrative structure
- Audience-specific communication strategies
- Visual hierarchy and chart selection principles
- Color best practices and accessibility
- Dashboard design and annotation techniques
- Avoiding misleading visualizations

**Learning Outcomes:**
- Transform analysis into compelling data stories
- Create audience-appropriate visualizations
- Apply ethical visualization practices
- Design effective dashboards and reports

### 5. [Anscombe's Quartet: Why Visualization Matters](anscombes_quartet_notebook.ipynb)
- **GitHub**: [anscombes_quartet_notebook.ipynb](anscombes_quartet_notebook.ipynb)
- **Google Colab**: [Open in Colab](https://colab.research.google.com/github/scottalanturner/predictive-analytics/blob/main/Module%205%20EDA/anscombes_quartet_notebook.ipynb)

**Focus:** The Critical Importance of Data Visualization

**Key Topics:**
- Anscombe's Quartet demonstration
- Statistical properties vs. visual patterns
- Real-world implications of visualization neglect
- Interactive comparison of identical statistics with different patterns

**Learning Outcomes:**
- Understand why summary statistics alone are insufficient
- Recognize different data patterns that produce identical statistics
- Appreciate the critical role of visualization in data analysis

## 🎯 Module Structure

Each notebook follows a consistent structure:
- **Learning Objectives** clearly stated at the beginning
- **Interactive Demonstrations** with live code examples
- **Practice Exercises** to reinforce concepts
- **Key Takeaways** summaries for each section
- **Real-world Applications** and business context

## 🛠️ Technical Requirements

**Required Libraries:**
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy import stats
from sklearn.preprocessing import StandardScaler
from sklearn.decomposition import PCA
import plotly.graph_objects as go
import plotly.express as px
```

**Installation:**
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn plotly
```

## 📊 Key Concepts Covered

### EDA Workflow
1. **First Look** - Dataset dimensions, preview, memory usage
2. **Data Types & Structure** - Understanding variable types
3. **Basic Statistics** - Summary statistics and distributions
4. **Data Quality** - Missing values, duplicates, consistency checks
5. **Quick Visualizations** - Initial pattern exploration

### Statistical Analysis
- **Normality Testing:** Shapiro-Wilk, D'Agostino-Pearson, Anderson-Darling
- **Group Comparisons:** t-tests, ANOVA, Mann-Whitney U, Kruskal-Wallis
- **Effect Size:** Cohen's d, R-squared, practical significance
- **Outlier Detection:** IQR method, Z-score analysis
- **Pattern Detection:** PCA, correlation analysis

### Visualization Best Practices
- **Chart Selection:** Matching visualization type to data and question
- **Color Theory:** Categorical, sequential, and diverging palettes
- **Visual Hierarchy:** Size, grouping, contrast, and flow
- **Accessibility:** Colorblind-friendly palettes and design
- **Ethics:** Honest representation and avoiding misleading charts

### Data Storytelling
- **Narrative Structure:** Setup → Conflict → Resolution → Action
- **Audience Adaptation:** Executive, technical, and operational perspectives
- **Dashboard Design:** 5-second rule, F-pattern layout, progressive disclosure
- **Annotation:** Clear titles, labels, sources, and context

## 🎓 Learning Path

**Recommended Sequence:**
1. Start with **Section 1** to understand the fundamental EDA workflow
2. Progress to **Section 2** for core analysis techniques
3. Advance to **Section 3** for statistical analysis skills
4. Complete **Section 4** for communication and storytelling
5. Review **Anscombe's Quartet** to reinforce the importance of visualization

**Time Investment:**
- Section 1: 2-3 hours
- Section 2: 2-3 hours  
- Section 3: 3-4 hours
- Section 4: 2-3 hours
- Anscombe's Quartet: 1 hour
- **Total:** 10-14 hours

## 💡 Key Takeaways

### Why EDA Matters
- **Discovery:** Uncover hidden patterns and relationships
- **Validation:** Check assumptions before modeling
- **Communication:** Make data insights accessible to stakeholders
- **Quality:** Identify data issues early in the process

### Best Practices
- **Always visualize** before analyzing statistically
- **Start with the big picture** then drill down to details
- **Document your process** for reproducibility
- **Consider your audience** when presenting findings
- **Question everything** - outliers, patterns, and assumptions

### Common Pitfalls to Avoid
- Relying solely on summary statistics
- Using inappropriate chart types
- Ignoring outliers without investigation
- Cherry-picking favorable time periods
- Confusing correlation with causation

## 🔗 Additional Resources

**Further Reading:**
- "The Visual Display of Quantitative Information" by Edward Tufte
- "Storytelling with Data" by Cole Nussbaumer Knaflic
- "Exploratory Data Analysis" by John Tukey

**Online Resources:**
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/)
- [Seaborn Examples](https://seaborn.pydata.org/examples/)
- [Plotly Chart Types](https://plotly.com/python/)

## 📝 Assessment

**Practice Exercises** are included in each notebook to reinforce learning:
- Apply EDA workflow to new datasets
- Create custom visualization templates
- Perform statistical analysis with proper test selection
- Build compelling data stories with appropriate visualizations

**Final Project Suggestion:**
Choose a real dataset and perform a complete EDA analysis, including:
1. Systematic exploration following the 5-step workflow
2. Statistical analysis with appropriate tests
3. Multiple visualizations with proper design principles
4. A data story presentation for a specific audience

---

**Module 5** provides the foundation for becoming an effective data analyst who can not only extract insights from data but also communicate those insights in ways that drive action and decision-making.
