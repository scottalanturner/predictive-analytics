# Career-Focused Data Investigation
## Comprehensive Data Analytics Assignment
**Submission Format: GitHub Repository with Jupyter Notebook**

---

## Project Overview

In this comprehensive assignment, you will demonstrate mastery of concepts from Modules 1-6 by conducting a complete data analytics investigation on a real-world dataset relevant to your career field. This project challenges you to tackle the complex, messy reality of real-world data while demonstrating both technical proficiency and analytical thinking.

Unlike simple visualization exercises, this assignment requires you to make thoughtful decisions about data quality, engineer meaningful features from domain knowledge, and communicate insights that could inform actual business or research decisions in your field of interest.

---

## Learning Objectives

Upon completion of this assignment, you will demonstrate your ability to:

1. **Execute the Complete Data Analytics Process**: Apply the Ask-Prepare-Process-Analyze-Share-Act framework on a complex, real-world dataset
2. **Navigate Data Quality Challenges**: Identify, document, and address multiple data quality issues using appropriate cleaning techniques
3. **Engineer Meaningful Features**: Create derived variables that enhance analytical value using domain knowledge
4. **Conduct Rigorous Exploratory Analysis**: Uncover patterns, relationships, and insights through systematic visual and statistical exploration
5. **Communicate Professional Insights**: Present findings in a clear, compelling manner suitable for stakeholders in your chosen field

---

## Assignment Requirements

### 1. Dataset Selection and Justification (15 points)

**Requirements:**
- Choose a dataset from Kaggle with **minimum 500 rows and 8 variables**
- Dataset must be relevant to your intended career field (business, healthcare, finance, marketing, sports, technology, etc.)
- Include at least 3 categorical variables and 4 numerical variables
- Should contain realistic data quality issues (missing values, outliers, inconsistencies)

**Deliverables:**
- **Career Relevance Justification** (200-300 words): Explain why this dataset is relevant to your career goals and what business/research questions it could help answer
- **Data Dictionary**: Create a comprehensive table describing each variable, its type, expected range/categories, and business meaning
- **Source Documentation**: Include Kaggle URL, dataset creator, original collection methodology, and any known limitations

### 2. Data Quality Assessment and Documentation (20 points)

**Requirements:**
- Conduct a systematic examination of data quality issues
- Document problems found with specific examples and counts
- Assess completeness, accuracy, consistency, and validity

**Deliverables:**
- **Data Quality Report**: Create a structured assessment covering:
  - Missing data patterns (which variables, how much, any patterns?)
  - Duplicate records (exact duplicates vs. potential duplicates)
  - Outliers and anomalies (statistical and logical outliers)
  - Inconsistencies (formatting, categories, data entry errors)
  - Data type issues (incorrect types, mixed formats)
- **Impact Analysis**: For each issue found, briefly explain its potential impact on analysis

### 3. Comprehensive Data Cleaning (25 points)

**Requirements:**
- Address all identified data quality issues with documented rationale
- Use appropriate techniques from Modules 3-4
- Make decisions that preserve analytical value while improving data quality

**Deliverables:**
- **Cleaning Implementation**: Clean code with clear comments explaining each decision
- **Decision Justification**: For each major cleaning decision, explain:
  - What method you chose (e.g., mean imputation vs. deletion)
  - Why you chose it over alternatives
  - What assumptions you're making
- **Before/After Comparison**: Show summary statistics or counts demonstrating the impact of cleaning

### 4. Strategic Feature Engineering (20 points)

**Requirements:**
- Create **4-5 meaningful derived variables** using domain knowledge
- Go beyond simple calculations to features that provide business insight
- Use techniques from Module 4 (date extractions, ratios, categorical groupings, etc.)

**Deliverables:**
- **Feature Creation**: Clean, commented code creating new variables
- **Business Rationale**: For each engineered feature, explain:
  - What business insight it captures
  - How it might be useful for decision-making in your field
  - Any domain knowledge that informed its creation
- **Feature Documentation**: Update your data dictionary to include new variables

### 5. Thorough Exploratory Data Analysis (30 points)

**Requirements:**
- Create **6-8 high-quality visualizations** exploring different aspects of the data
- Include both univariate and bivariate analysis
- Follow visualization best practices from Module 5

**Deliverables:**
- **Distribution Analysis**: Explore the distribution of key variables (histograms, box plots, etc.)
- **Relationship Exploration**: Investigate relationships between variables (scatter plots, correlation analysis, grouped comparisons)
- **Pattern Detection**: Look for interesting patterns, trends, or anomalies in the data
- **Professional Visualizations**: Each chart should have:
  - Clear, descriptive titles
  - Proper axis labels and units
  - Appropriate chart types for the data
  - Clean formatting and readable fonts
- **Interpretation**: For each visualization, provide 2-3 sentences explaining what insights it reveals

### 6. Business Insights Report (25 points)

**Requirements:**
- Synthesize your analysis into actionable insights for stakeholders in your career field
- Focus on findings that could inform real business or research decisions
- Write for a professional audience

**Deliverables:**
- **Executive Summary** (300-400 words): High-level overview of key findings suitable for busy executives
- **Detailed Findings** (600-800 words): Deeper dive into 3-4 major insights with supporting evidence
- **Recommendations** (200-300 words): Specific, actionable recommendations based on your analysis
- **Limitations and Next Steps** (150-200 words): Acknowledge limitations of your analysis and suggest future research directions

---

## Technical Requirements

### Jupyter Notebook Organization
- **Clear section headers** using markdown cells
- **Professional formatting** with consistent style
- **Code cells** with appropriate comments
- **Markdown explanations** before major code sections
- **Logical flow** from data loading through final insights

### Code Quality Standards
- Use descriptive variable names
- Include comments for complex operations
- Follow PEP 8 style guidelines where possible
- Handle errors gracefully (e.g., file not found)
- Use appropriate pandas/numpy methods efficiently

### Documentation Standards
- All text should be professional and free of grammatical errors
- Use proper markdown formatting (headers, lists, emphasis)
- Include in-line citations for any external sources referenced
- Maintain consistent tone throughout the document

---

## Evaluation Rubric

### Excellent (A: 90-100%)
- Demonstrates mastery of all concepts with sophisticated application
- Shows creative and insightful feature engineering using domain knowledge
- Produces publication-quality visualizations with deep insights
- Provides compelling business recommendations supported by evidence
- Code is efficient, well-documented, and error-free

### Proficient (B: 80-89%)
- Shows solid understanding of concepts with competent application
- Creates meaningful features with clear business rationale
- Produces clear visualizations with appropriate interpretations
- Provides reasonable recommendations based on analysis
- Code is functional and adequately documented

### Developing (C: 70-79%)
- Demonstrates basic understanding with some gaps in application
- Attempts feature engineering but may lack strong business connection
- Creates adequate visualizations but interpretations may be superficial
- Provides basic recommendations with limited supporting evidence
- Code works but may have inefficiencies or documentation gaps

### Needs Improvement (D/F: Below 70%)
- Shows limited understanding of concepts or poor application
- Feature engineering is minimal or lacks clear purpose
- Visualizations are basic or poorly interpreted
- Recommendations are weak or unsupported by analysis
- Code has significant issues or poor documentation

---

## Submission Guidelines

### GitHub Repository Requirements
- Create a new public GitHub repository for this assignment
- Name your repository: `data-investigation-lastname-firstname`
- Repository must include:
  - Your Jupyter Notebook file: `data_investigation.ipynb`
  - A README.md file with project description and instructions to reproduce your analysis
  - Your dataset file (if <25MB) or clear instructions for downloading the dataset
  - Any additional documentation files

### Blackboard Submission
- Submit only the URL of your GitHub repository to Blackboard
- Ensure your repository is public and accessible
- Repository must be created and populated before the due date

### Academic Integrity
- This is an individual assignment
- You may discuss general concepts with classmates but not share code or specific solutions
- Properly cite any external resources used beyond course materials
- Plagiarism from Kaggle will result in a grade of zero

---

## Tips for Success

### Getting Started
- Start early! Data cleaning always takes longer than expected
- Choose a dataset you're genuinely interested in - passion shows in the quality of analysis
- Read the dataset documentation thoroughly before beginning

### Data Selection Tips
- Look for datasets with interesting business applications in your field
- Avoid datasets that are already perfectly clean - you need problems to solve
- Consider datasets from domains like:
  - **Business**: Customer data, sales records, employee information
  - **Healthcare**: Patient outcomes, clinical trials, health metrics
  - **Finance**: Market data, loan applications, company financials
  - **Marketing**: Campaign performance, social media metrics, customer behavior
  - **Sports**: Player statistics, team performance, game outcomes
  - **Technology**: User behavior, app performance, system metrics

### Analysis Strategy
- Don't try to analyze everything - focus on the most interesting and important patterns
- Let your domain knowledge guide feature engineering decisions
- Remember your audience - what would actually matter to professionals in your field?

### Common Pitfalls to Avoid
- Don't spend too much time on minor data cleaning issues at the expense of analysis
- Avoid creating features just for the sake of meeting requirements - they should add value
- Don't present findings without interpreting their business significance
- Avoid overly technical language in your business insights section

---

## Resources and Support

### Course Resources
- Review Module 3-6 slide decks for specific techniques
- Reference lab assignments for code examples

### External Resources
- Kaggle dataset documentation and discussions
- Pandas documentation for data manipulation
- Matplotlib/Seaborn documentation for visualization
- Industry blogs and publications relevant to your chosen field

---

## Final Note

This assignment is designed to simulate the type of work you'll do as a data professional. The skills you demonstrate here - cleaning messy data, engineering meaningful features, conducting thorough analysis, and communicating insights - are exactly what employers value most.

Take pride in producing work that showcases not just your technical abilities, but your ability to think critically about data and translate analysis into business value. This assignment can become a cornerstone piece for your professional portfolio.

**Good luck, and remember: great analysis tells a compelling story backed by solid evidence!**