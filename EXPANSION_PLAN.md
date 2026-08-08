# R Statistics Training Programme: Expansion Plan

**Document Date:** August 8, 2026  
**Prepared for:** GoldPsychR Programme Extension  
**Current Version:** 4-session intensive course

---

## Executive Summary

This document reviews the current **GoldPsychR** four-session R statistics course and presents a detailed plan to extend it into a comprehensive training programme suitable for semester-long instruction or professional development.

**Current Scope:** 4 labs covering fundamentals (descriptives, t-tests, ANOVA, regression)  
**Proposed Scope:** 12-16 week comprehensive programme with progressive skill building

---

## Part 1: Current Course Review

### 1.1 Existing Structure

The current **GoldPsychR** course consists of:

#### **Course Architecture**
- **Platform:** Quarto-based website with WebR integration
- **Duration:** 4 lab sessions (2 hours each, 13:00-15:00)
- **Target Audience:** Psychology students at Goldsmiths, University of London
- **Delivery:** Hybrid approach with RStudio Server and browser-based WebR
- **Repository:** https://github.com/LittleMonkeyLab/GoldPsychR

#### **Current Content Breakdown**

| Lab | Topic | Content Coverage | Skills Taught |
|-----|-------|------------------|---------------|
| **Lab 1** | Descriptive Statistics | Grit Scale analysis | Data loading, reverse scoring, descriptives, ggplot2, APA reporting |
| **Lab 2** | T-Tests | Test anxiety data | One-sample, independent, paired t-tests, effect sizes (Cohen's d) |
| **Lab 3** | ANOVA | Study techniques experiment | One-way ANOVA, two-way ANOVA, post-hoc tests (Tukey HSD), η² |
| **Lab 4** | Correlation & Regression | Linear models | Correlation, simple regression, multiple regression, diagnostics |

#### **Pedagogical Approach**

The course employs a **three-stage learning pathway**:

1. **Instructor Demo** (Slides embedded in pages)
   - Live demonstration with real psychology data
   - RevealJS slides with animated code examples
   
2. **WebR Practice** (Browser-based interactive coding)
   - Immediate hands-on practice without installation
   - Interactive code cells with instant feedback
   - Self-assessment quizzes using webex

3. **RStudio Exercise** (Real environment practice)
   - Downloadable .qmd templates
   - Work in actual RStudio Server environment
   - Submission-ready assignments

4. **Follow-On Exercises** (Transfer learning)
   - Additional datasets for skill reinforcement
   - Different research contexts

#### **Supporting Resources**

1. **R Toolbox**
   - Quick reference guides organized by task
   - Topics: Setup, Import, Wrangle, Plots, Tests, Models, Reporting, Troubleshooting
   - Currently mostly placeholder sections

2. **Boil in the Bag Templates**
   - 9 ready-to-run statistical analysis templates
   - Covers: t-tests (2), ANOVA (4), regression (3)
   - Generic dummy datasets with clear variable naming
   - Complete analysis workflows: descriptives → assumptions → analysis → interpretation

3. **R Handbook**
   - Single-page comprehensive reference (r-handbook.qmd)
   - Consolidated guide for quick lookup

### 1.2 Technical Infrastructure

#### **Technology Stack**
- **Quarto:** Website and document generation
- **WebR:** Browser-based R execution (no installation required)
- **RStudio Server:** https://psy909.gold.ac.uk/rstudioserver/
- **Version Control:** Git/GitHub
- **Package Management:** renv for reproducibility
- **Key R Packages:** tidyverse, ggplot2

#### **Content Management**
- Modular structure with chapters separated into parts
- Each part has: slides version + interactive version
- Freeze execution for faster rebuilds
- Downloadthis integration for exercise distribution
- Custom SCSS theming (Goldsmiths branding)

### 1.3 Strengths of Current Programme

1. **Pedagogical Excellence**
   - Progressive difficulty with scaffolded learning
   - Multiple practice opportunities (WebR → RStudio)
   - Real psychology research contexts
   - Immediate feedback mechanisms

2. **Accessibility**
   - Browser-based practice removes installation barriers
   - Clear visual design with intuitive navigation
   - Embedded slides eliminate window-switching
   - Mobile-friendly responsive design

3. **Practical Focus**
   - APA-style reporting emphasized throughout
   - Publication-quality visualizations
   - Real research scenarios (grit, test anxiety, study techniques)
   - Reproducible research workflow with Quarto

4. **Resource Richness**
   - Boil in the Bag templates for quick analyses
   - Multiple entry points for different learning styles
   - Follow-on exercises for reinforcement

5. **Production Quality**
   - Professional branding and design
   - Consistent visual language
   - Well-organized file structure
   - Version controlled with CI/CD

### 1.4 Current Gaps & Limitations

#### **Content Coverage Gaps**
1. Data manipulation and tidyverse fundamentals (limited coverage)
2. No dedicated data visualization module (ggplot2 introduced but not comprehensive)
3. Missing intermediate/advanced topics:
   - Mixed effects models
   - Logistic regression
   - Non-parametric tests
   - Power analysis
   - Mediation/moderation
   - Factor analysis/PCA
   - Structural equation modeling basics

4. Limited programming fundamentals:
   - Functions and loops not covered
   - Debugging strategies minimal
   - Package management not taught
   - R Markdown/Quarto only introduced contextually

5. No data ethics or open science practices
6. Missing reproducibility best practices (beyond Quarto)
7. No version control (Git) instruction
8. Limited data cleaning and preprocessing

#### **Pedagogical Gaps**
1. No capstone/integrative project
2. Limited peer collaboration opportunities
3. No formative assessment beyond self-check quizzes
4. Missing learning outcomes assessment rubrics

#### **Resource Gaps**
1. Toolbox sections mostly placeholders
2. No video tutorials or screencasts
3. Limited troubleshooting resources
4. No cheat sheets or quick reference cards
5. No example research reports

---

## Part 2: Extension Strategy

### 2.1 Programme Vision

**Transform GoldPsychR into a comprehensive, semester-long R statistics training programme that:**

1. Takes learners from complete beginners to confident independent analysts
2. Covers full research workflow: design → data → analysis → reporting → sharing
3. Emphasizes reproducible, ethical, and open research practices
4. Provides domain-specific applications for psychology research
5. Builds both statistical understanding AND programming competency
6. Prepares students for real-world research and industry applications

### 2.2 Proposed Structure

#### **Option A: 12-Week Semester Programme (Undergraduate)**

**Target:** Psychology undergraduate students, 2 hours/week labs + self-study

| Week | Module | Topics | Builds On |
|------|--------|--------|-----------|
| **1** | R Foundations | RStudio, R basics, data types, vectors | NEW |
| **2** | Data Import & Wrangling | Reading data, tidyverse, pipes, select/filter/mutate | Week 1 |
| **3** | Data Visualization I | ggplot2 grammar, geoms, aesthetics | Week 2 |
| **4** | Descriptive Statistics | Measures of central tendency, spread, distributions | Current Lab 1 (expanded) |
| **5** | Probability & Sampling | Distributions, sampling theory, simulation | NEW |
| **6** | Hypothesis Testing & T-Tests | Null hypothesis, p-values, t-tests | Current Lab 2 (expanded) |
| **7** | ANOVA & Factorial Designs | One-way, factorial, interactions | Current Lab 3 (expanded) |
| **8** | **READING WEEK / MID-TERM PROJECT** | Data analysis mini-project | Weeks 1-7 |
| **9** | Correlation & Simple Regression | Relationships, prediction, assumptions | Current Lab 4 (Part 1) |
| **10** | Multiple Regression | Multiple predictors, adjusted R², model comparison | Current Lab 4 (Part 2) |
| **11** | Data Visualization II & Reporting | Publication figures, RMarkdown/Quarto reports | Weeks 3 + all |
| **12** | **CAPSTONE PROJECT** | Complete analysis with report | All skills |

#### **Option B: 16-Week Extended Programme (Postgraduate/Professional)**

**Target:** MSc students, researchers, professionals seeking advanced skills

Expands the 12-week programme with:

| Week | Module | Topics |
|------|--------|--------|
| **13** | Repeated Measures & Mixed Designs | Within-subjects ANOVA, mixed ANOVA |
| **14** | Logistic Regression | Binary outcomes, odds ratios, classification |
| **15** | Advanced Topics I | Moderation, mediation, or non-parametric tests |
| **16** | Advanced Topics II | Mixed-effects models intro OR power analysis |

#### **Option C: Modular Self-Paced Programme**

**Structure:** 6 modules, each 2-3 weeks of self-paced work

1. **Foundations** (R basics, data wrangling, visualization)
2. **Descriptive & Exploratory Analysis** (Descriptives, visualization)
3. **Hypothesis Testing** (t-tests, ANOVA, post-hocs)
4. **Correlation & Regression** (Linear models)
5. **Advanced Statistical Methods** (Mixed models, logistic regression)
6. **Reproducible Research** (Quarto, Git, open science)

---

## Part 3: Detailed Content Plan

### 3.1 New Modules to Develop

#### **Module 1: R Foundations (NEW)**
*Replaces implicit assumptions in current Lab 1*

**Learning Objectives:**
- Navigate RStudio interface confidently
- Understand R data types and structures
- Use functions and read documentation
- Install and load packages
- Understand the R ecosystem

**Content:**
- RStudio panes and workflow
- Objects, vectors, data frames, lists
- Data types: numeric, character, factor, logical
- Functions: arguments, help files, examples
- Installing packages (CRAN, GitHub)
- R scripts vs. R Markdown/Quarto
- Workspace management

**Exercises:**
- Interactive WebR practice (basic calculations, variables, vectors)
- RStudio orientation scavenger hunt
- Build your first R script
- Help file exploration challenge

**Deliverables to Create:**
- part1-slides.qmd: RStudio tour and R basics
- part1.qmd: Interactive WebR exercises
- templates/week01-exercise.qmd: RStudio practice workbook
- toolbox/rstudio-tour.qmd: Reference guide

---

#### **Module 2: Data Import & Wrangling (NEW)**
*Foundation for all subsequent analyses*

**Learning Objectives:**
- Import data from CSV, Excel, SPSS
- Use tidyverse pipes (%>% and |>)
- Select, filter, and arrange data
- Create new variables with mutate()
- Group and summarize data
- Handle missing data

**Content:**
- Working directories and file paths
- read_csv(), read_excel(), haven::read_sav()
- Introduction to tidyverse philosophy
- dplyr verbs: select, filter, mutate, arrange, summarize
- group_by() for grouped operations
- Handling NA values
- Data validation and cleaning

**Psychology Examples:**
- Clean a messy questionnaire dataset
- Reverse score multiple items efficiently
- Calculate scale scores with rowMeans()
- Filter for participants who completed study

**Exercises:**
- Import multiple data formats
- Clean a messy dataset (missing values, duplicates)
- Create derived variables (age groups, sum scores)
- Group-wise summaries by condition

**Deliverables to Create:**
- chapters/week02/part1.qmd: Import and inspect
- chapters/week02/part2.qmd: dplyr basics
- chapters/week02/part3.qmd: Pipes and workflows
- data/messy_survey_data.csv: Practice dataset
- toolbox/wrangle.qmd: Complete dplyr reference (expand from placeholder)

---

#### **Module 3: Data Visualization I (NEW)**
*Currently scattered across labs; needs dedicated module*

**Learning Objectives:**
- Understand ggplot2 grammar of graphics
- Create basic plots: scatter, bar, box, histogram
- Customize aesthetics and themes
- Use faceting for grouped plots
- Choose appropriate visualizations for data types

**Content:**
- ggplot2 philosophy: data → aesthetics → geometries
- Essential geoms: geom_point, geom_bar, geom_boxplot, geom_histogram
- Aesthetic mappings: x, y, color, fill, shape, size
- Customization: labs(), theme(), scales
- Faceting: facet_wrap(), facet_grid()
- Color palettes (including colorblind-friendly)

**Psychology Examples:**
- Scatter plot: anxiety vs. performance
- Box plot: depression scores by treatment group
- Histogram: distribution of reaction times
- Faceted plots: conditions across multiple measures

**Exercises:**
- Recreate published figures
- Visualization choice challenge (match plot to data type)
- Create a figure panel (multiple plots)
- Customize a theme for your lab

**Deliverables to Create:**
- chapters/week03/part1.qmd: ggplot2 basics
- chapters/week03/part2.qmd: Aesthetics and geoms
- chapters/week03/part3.qmd: Customization and themes
- toolbox/plots.qmd: Complete visualization reference (expand placeholder)
- assets/ggplot2-cheatsheet-psych.pdf: Psychology-focused cheat sheet

---

#### **Module 5: Probability & Sampling (NEW)**
*Missing foundation for inferential statistics*

**Learning Objectives:**
- Understand probability distributions
- Differentiate population vs. sample
- Explain sampling distributions and Central Limit Theorem
- Use simulation to understand statistical concepts
- Calculate confidence intervals

**Content:**
- Probability fundamentals
- Normal distribution and z-scores
- Sampling distributions
- Standard error vs. standard deviation
- Central Limit Theorem (demonstrated via simulation)
- Confidence intervals
- Bootstrap methods (introduction)

**Interactive Elements:**
- Simulate sampling distributions with different n
- Visualize Central Limit Theorem with animations
- Explore effect of sample size on confidence intervals
- Bootstrap a dataset interactively

**Psychology Examples:**
- IQ scores and normal distribution
- Reaction time distributions (often skewed)
- Sample size planning for survey research

**Exercises:**
- Simulate 1000 samples and plot sampling distribution
- Calculate z-scores for psychological test scores
- Construct confidence intervals manually and with R
- Compare bootstrap vs. parametric CIs

**Deliverables to Create:**
- chapters/week05/part1.qmd: Probability basics
- chapters/week05/part2.qmd: Sampling distributions (with animations)
- chapters/week05/part3.qmd: Confidence intervals
- chapters/week05/part4.qmd: Bootstrap simulation
- interactive demos using WebR for CLT visualization

---

#### **Module 11: Data Visualization II & Reporting (NEW)**
*Advanced visualization and complete reporting workflow*

**Learning Objectives:**
- Create publication-quality figures
- Design effective multi-panel figures
- Use patchwork/cowplot for figure composition
- Write complete APA-style research reports in Quarto
- Integrate code, analysis, and narrative
- Export figures for publication

**Content:**
- Publication standards for figures
- Advanced ggplot2: annotation, insets, custom themes
- Multi-panel figures with patchwork
- Figure legends and captions
- Quarto for academic writing
  - YAML headers and options
  - Cross-referencing figures and tables
  - Bibliography management
  - Output formats (PDF, Word, HTML)
- Reproducible reporting workflow
- File organization for projects

**Psychology Examples:**
- Create a journal-ready figure panel
- Write complete Methods and Results sections
- Build a reproducible analysis report
- Create supplementary materials

**Exercises:**
- Recreate a figure from a published paper
- Write a complete analysis report for a provided dataset
- Export figures in multiple formats (TIFF, PDF, PNG)
- Create a supplementary data file

**Deliverables to Create:**
- chapters/week11/part1.qmd: Publication-quality figures
- chapters/week11/part2.qmd: Multi-panel figures with patchwork
- chapters/week11/part3.qmd: Quarto for academic reports
- chapters/week11/part4.qmd: Complete report walkthrough
- templates/apa-report-template.qmd: Full APA-style template
- toolbox/reporting.qmd: Complete reporting reference (expand placeholder)
- examples/example-research-report.qmd: Model report

---

### 3.2 Existing Modules to Expand

#### **Lab 1 → Week 4: Descriptive Statistics (EXPAND)**

**Current State:** Good foundation but assumes data wrangling knowledge

**Additions Needed:**
1. More emphasis on data distributions and checking normality
2. Introduction to skew and kurtosis
3. Detecting outliers (IQR method, z-scores)
4. Data transformation concepts (log, sqrt)
5. Expanded APA reporting with sample write-up examples

**New Content:**
- chapters/week04/part1.qmd: Distributions and normality (NEW)
- chapters/week04/part2.qmd: Outlier detection (NEW)
- Expand existing content with more explanation
- Add formative quiz after each section
- Include common errors troubleshooting

---

#### **Lab 2 → Week 6: Hypothesis Testing & T-Tests (EXPAND)**

**Current State:** Covers t-tests well but lacks hypothesis testing foundation

**Additions Needed:**
1. Null vs. alternative hypotheses
2. Type I and Type II errors
3. P-values explained clearly (common misinterpretations)
4. Effect sizes and practical significance
5. Assumptions checking (normality, homogeneity of variance)
6. Non-parametric alternatives (Mann-Whitney, Wilcoxon) when assumptions violated

**New Content:**
- chapters/week06/part1.qmd: Hypothesis testing framework (NEW)
- chapters/week06/part2.qmd: P-values and statistical significance (NEW)
- chapters/week06/part6.qmd: Non-parametric alternatives (NEW)
- Expand assumptions checking with diagnostic plots
- Add more APA reporting examples with different scenarios

---

#### **Lab 3 → Week 7: ANOVA & Factorial Designs (EXPAND)**

**Current State:** Good coverage but needs more on assumptions and contrasts

**Additions Needed:**
1. Detailed assumptions checking (normality, homogeneity, independence)
2. Planned contrasts vs. post-hoc tests
3. Effect sizes (omega-squared, eta-squared, partial eta-squared)
4. Interpreting interactions with plots
5. Non-parametric alternatives (Kruskal-Wallis, Friedman)
6. More complex factorial designs (3-way ANOVA introduction)

**New Content:**
- Expand assumptions sections with visual diagnostics
- Add chapter on planned contrasts
- Include interaction plot tutorial
- Add more post-hoc comparison methods
- Enhance APA reporting with tables

---

#### **Lab 4 → Weeks 9-10: Correlation & Regression (EXPAND & SPLIT)**

**Current State:** Covers basics but needs to be split into two weeks

**Week 9: Correlation & Simple Regression**
- Scatterplots and relationships
- Pearson's r, Spearman's rho
- Assumptions for correlation
- Simple linear regression
- Interpreting slope and intercept
- Prediction and residuals
- R² as explained variance

**Week 10: Multiple Regression**
- Adding predictors
- Adjusted R²
- Model comparison with anova()
- Multicollinearity (VIF)
- Standardized coefficients
- Categorical predictors (dummy coding)
- Hierarchical regression

**New Content to Add:**
- chapters/week09/part4.qmd: Assumption diagnostics with plots
- chapters/week10/part1.qmd: Introduction to multiple regression
- chapters/week10/part2.qmd: Model comparison strategies
- chapters/week10/part3.qmd: Categorical predictors and interactions
- chapters/week10/part4.qmd: Diagnostics for multiple regression
- Expand residual analysis
- Add multicollinearity detection
- Include model selection strategies (AIC, BIC basics)

---

### 3.3 Advanced Modules (Weeks 13-16 for Extended Programme)

#### **Week 13: Repeated Measures & Mixed Designs**

**Learning Objectives:**
- Understand within-subjects designs
- Run repeated measures ANOVA
- Run mixed (split-plot) ANOVA
- Check sphericity assumption
- Apply Greenhouse-Geisser correction

**Content:**
- Within-subjects vs. between-subjects designs
- Advantages and disadvantages of repeated measures
- Sphericity assumption and Mauchly's test
- Using afex or ez package for ANOVA
- Pairwise comparisons with corrections
- Effect sizes for repeated measures

**Psychology Examples:**
- Pre-post-follow-up treatment study
- Learning curve across multiple trials
- Mixed design: treatment group × time

**Deliverables to Create:**
- chapters/week13/part1.qmd: Introduction to repeated measures
- chapters/week13/part2.qmd: RM ANOVA in R
- chapters/week13/part3.qmd: Mixed designs
- boil_in_the_bag/05_repeated_measures_anova.qmd: Already exists, integrate/expand
- boil_in_the_bag/06_mixed_anova.qmd: Already exists, integrate/expand

---

#### **Week 14: Logistic Regression**

**Learning Objectives:**
- Understand when to use logistic regression
- Interpret odds ratios
- Run binary logistic regression with glm()
- Assess model fit
- Report logistic regression results

**Content:**
- Binary outcome variables
- Logit transformation
- Interpreting coefficients as log-odds
- Converting to odds ratios
- Predicted probabilities
- Model fit: deviance, AIC, confusion matrix
- ROC curves and classification accuracy

**Psychology Examples:**
- Predicting diagnosis (yes/no) from symptoms
- Predicting dropout from study
- Pass/fail on task from cognitive measures

**Deliverables to Create:**
- chapters/week14/part1.qmd: Introduction to logistic regression
- chapters/week14/part2.qmd: Running glm() for binary outcomes
- chapters/week14/part3.qmd: Interpreting odds ratios
- chapters/week14/part4.qmd: Model fit and diagnostics
- boil_in_the_bag/10_logistic_regression.qmd: Template (NEW)

---

#### **Week 15: Advanced Topics I (Choose One)**

**Option A: Moderation and Mediation**

**Learning Objectives:**
- Understand moderation vs. mediation
- Test moderation with interaction terms
- Conduct mediation analysis
- Interpret indirect effects

**Content:**
- Conceptual frameworks
- Testing moderation in regression
- Simple slopes analysis
- Introduction to mediation (using mediation package or lavaan)
- Bootstrapping for indirect effects
- Reporting moderation and mediation

**Option B: Non-Parametric Tests**

**Learning Objectives:**
- Know when parametric assumptions fail
- Select appropriate non-parametric alternatives
- Run Mann-Whitney, Wilcoxon, Kruskal-Wallis tests
- Interpret and report non-parametric results

**Content:**
- Assumptions for parametric tests
- Rank-based methods
- Mann-Whitney U test (alternative to independent t-test)
- Wilcoxon signed-rank test (alternative to paired t-test)
- Kruskal-Wallis test (alternative to one-way ANOVA)
- Effect sizes for non-parametric tests

**Option C: Power Analysis and Sample Size Planning**

**Learning Objectives:**
- Understand statistical power
- Conduct power analysis for common tests
- Plan sample sizes for studies
- Use simulation for power analysis

**Content:**
- Power, effect size, alpha, sample size relationships
- Using pwr package
- Power analysis for t-tests, ANOVA, regression
- Sensitivity analysis
- Simulation-based power analysis

---

#### **Week 16: Advanced Topics II (Choose One)**

**Option A: Introduction to Mixed-Effects Models**

**Learning Objectives:**
- Understand fixed vs. random effects
- Recognize when to use mixed models
- Fit basic mixed models with lme4
- Interpret random effects

**Content:**
- Hierarchical/nested data structures
- Fixed vs. random effects
- Random intercepts and random slopes
- Using lme4::lmer()
- Model comparison for mixed models
- Reporting mixed models

**Option B: Reproducible Research & Open Science**

**Learning Objectives:**
- Understand reproducibility crisis and solutions
- Use version control (Git basics)
- Organize analysis projects
- Share data and code openly
- Preregistration concepts

**Content:**
- Open science practices
- Git and GitHub for version control
- Project organization (folder structure, file naming)
- Sharing on OSF (Open Science Framework)
- Writing README files and data dictionaries
- Preregistration templates
- Quarto projects for reproducibility

**Option C: Data Ethics and Privacy**

**Learning Objectives:**
- Understand ethical considerations in data analysis
- Anonymize data appropriately
- Handle sensitive data
- Recognize algorithmic bias

**Content:**
- GDPR and data protection
- Anonymization techniques
- Secure data storage and sharing
- Ethical visualization practices
- Bias in datasets and algorithms
- Transparency in research

---

### 3.4 Assessment Strategy

#### **Formative Assessment (Throughout)**

1. **Self-Check Quizzes** (After each part)
   - Currently using webex, expand these
   - Multiple choice, fill-in-blank, true/false
   - Immediate feedback with explanations

2. **Weekly Exercises** (Downloadable .qmd files)
   - Practice datasets with guided questions
   - Automated checks where possible (using testthat for answer validation)
   - Model solutions provided after deadline

3. **Discussion Forum Participation**
   - Help peers with troubleshooting
   - Share interesting findings
   - Reflect on learning

4. **Code Review Activities**
   - Peer review of code for clarity
   - Identify errors in provided code
   - Suggest improvements

#### **Summative Assessment**

**For 12-Week Programme:**

1. **Mid-Term Project (Week 8)** - 30%
   - Analyze provided dataset
   - Research question: test group differences
   - Deliverable: Quarto report (3-4 pages)
   - Skills tested: Weeks 1-7

2. **Weekly Exercise Submissions** - 30%
   - Best 8 of 10 exercises
   - Graded on: code functionality, interpretation, APA reporting

3. **Final Capstone Project (Week 12)** - 40%
   - Open dataset from your own area of interest OR provided options
   - Complete research cycle: question → analysis → interpretation → report
   - Deliverable: Full Quarto report (6-8 pages) with code
   - Peer review component (formative)
   - Skills tested: All weeks

**Rubric Components:**
- Code quality and reproducibility (25%)
- Statistical accuracy (25%)
- Interpretation and critical thinking (25%)
- APA-style reporting and communication (25%)

**For 16-Week Programme:**

Add 10% for Advanced Topics Assignment, reduce Final Project to 35%

---

## Part 4: Resource Development Plan

### 4.1 Toolbox Completion

**Currently:** 8 sections, mostly placeholders

**Priority Sections to Develop:**

1. **toolbox/setup.qmd** (Expand from placeholder)
   - Installing R and RStudio
   - RStudio Server access for Goldsmiths students
   - Installing packages
   - Troubleshooting installation issues
   - Setting up RStudio preferences
   - Using R projects

2. **toolbox/import.qmd** (Expand from placeholder)
   - Reading CSV files
   - Reading Excel files
   - Reading SPSS/Stata/SAS files
   - Importing from Google Sheets
   - Connecting to databases (advanced)
   - Handling different encodings

3. **toolbox/wrangle.qmd** (Expand from placeholder)
   - Complete dplyr verb reference
   - tidyr for reshaping (pivot_longer, pivot_wider)
   - stringr for text manipulation
   - lubridate for dates
   - Joining datasets (left_join, inner_join, etc.)
   - Handling missing data

4. **toolbox/plots.qmd** (Expand from placeholder)
   - Complete geom reference with examples
   - Color palette guide (including colorblind-friendly)
   - Theme customization
   - Saving plots (ggsave)
   - Faceting strategies
   - Animation with gganimate (bonus)

5. **toolbox/tests.qmd** (Expand from placeholder)
   - Complete reference for all tests covered
   - Decision tree: which test when?
   - Assumptions for each test
   - Function syntax and key arguments
   - Interpretation guide
   - APA reporting templates

6. **toolbox/models.qmd** (Expand from placeholder)
   - lm() complete reference
   - glm() for logistic regression
   - Model diagnostics (plot.lm)
   - Model comparison (anova, AIC, BIC)
   - Extracting coefficients and predictions

7. **toolbox/reporting.qmd** (Expand from placeholder)
   - APA numbers formatting
   - Statistical notation guide
   - Example results paragraphs for each test
   - Table formatting (kableExtra, gt)
   - Inline code in Quarto
   - Cross-referencing

8. **toolbox/troubleshooting.qmd** (Expand from placeholder)
   - Common error messages decoded
   - Package installation issues
   - Data import problems
   - ggplot2 errors
   - Function not found errors
   - Object not found errors
   - Debugging strategies

**New Toolbox Sections to Add:**

9. **toolbox/functions.qmd** (NEW)
   - Writing custom functions
   - Function arguments and defaults
   - Return values
   - Documenting functions
   - When to write a function

10. **toolbox/projects.qmd** (NEW)
    - R project workflow
    - Folder structure best practices
    - File naming conventions
    - Using here package for paths
    - Organizing analysis scripts

11. **toolbox/git-basics.qmd** (NEW)
    - What is version control?
    - Git basics for R users
    - Using Git in RStudio
    - GitHub for sharing
    - Committing, pushing, pulling

12. **toolbox/packages.qmd** (NEW)
    - Essential packages for psychology research
    - Package installation and loading
    - Managing package versions with renv
    - Finding packages for your needs

---

### 4.2 Additional Templates & Examples

#### **Exercise Templates**

*Complete the templates/ directory*

Currently have:
- lab1-exercise.qmd
- lab2-exercise.qmd (mentioned but check existence)
- lab3-exercise.qmd (mentioned but check existence)
- lab4-exercise.qmd (mentioned but check existence)

Need to create:
- week01-exercise.qmd: R basics practice
- week02-exercise.qmd: Data wrangling challenge
- week03-exercise.qmd: Visualization gallery
- week05-exercise.qmd: Probability simulations
- week08-midterm-project.qmd: Mid-term project template
- week11-exercise.qmd: Report writing
- week12-capstone-project.qmd: Final project template
- Plus exercises for weeks 13-16 if extended programme

#### **Follow-On Exercises**

*Expand the followon/ directory*

Currently mentioned:
- lab1-followon.qmd
- lab2-followon.qmd
- lab3-followon.qmd
- lab4-followon.qmd

Need to verify existence and create for new weeks

Concept: Each follow-on uses a DIFFERENT psychology dataset to practice the same skills, promoting transfer

Ideas for new follow-on datasets:
- Big Five personality and job performance
- Social media use and wellbeing
- Sleep quality and academic performance
- Mindfulness intervention RCT
- Implicit Association Test data
- Eye-tracking reading study
- Memory and aging study

#### **Boil in the Bag Expansion**

*Add templates for new analyses*

Currently have 9 templates (t-tests, ANOVA, regression)

Add:
- 10_logistic_regression.qmd
- 11_repeated_measures_anova_long.qmd (using long format data)
- 12_mediation_analysis.qmd
- 13_moderation_analysis.qmd
- 14_mixed_model_intro.qmd
- 15_non_parametric_tests.qmd

#### **Example Research Reports**

*NEW directory: examples/*

Create model research reports that students can emulate:

- example-descriptive-report.qmd: Lab 1 style
- example-experiment-report.qmd: Lab 3 style with ANOVA
- example-correlational-report.qmd: Lab 4 style
- example-full-paper.qmd: Complete APA paper with all sections
- example-preregistration.qmd: Preregistration template

Include:
- Rendered HTML and PDF versions
- Annotations explaining choices
- Comments in code explaining key decisions

---

### 4.3 Supplementary Materials

#### **Cheat Sheets**

Create psychology-focused cheat sheets:

1. **dplyr-for-psychologists.pdf**
   - Common data wrangling tasks
   - Psychology examples
   - One-page reference

2. **ggplot2-for-psychologists.pdf**
   - Common plot types for psych data
   - Customization quick reference
   - Example code snippets

3. **statistical-tests-decision-tree.pdf**
   - Flowchart for test selection
   - Assumptions checklist
   - Function names

4. **apa-reporting-guide.pdf**
   - Statistical notation reference
   - Example sentences for each test
   - Number formatting rules

5. **r-basics-cheatsheet.pdf**
   - Data types and structures
   - Common functions
   - Operators and syntax

#### **Video Content**

*NEW directory: videos/ (store on external platform, embed in pages)*

Priority videos to create:

1. **RStudio Tour** (5 min)
   - Interface walkthrough
   - Where things are
   - Basic workflow

2. **Your First R Script** (8 min)
   - Creating a script
   - Running code
   - Saving and organizing

3. **Troubleshooting Common Errors** (10 min)
   - Demo of debugging process
   - Reading error messages
   - Using help files

4. **Creating a Quarto Report** (12 min)
   - YAML header
   - Code chunks
   - Rendering to HTML/PDF

5. **Git Basics for R Users** (15 min)
   - Init, commit, push workflow
   - Using Git in RStudio
   - Why version control matters

6. **Test-Specific Videos** (5-8 min each)
   - One video per major test
   - Screencasts of actual analysis
   - Interpretation walkthrough

#### **Data Repository**

*Expand data/ directory*

Organize datasets by module:

```
data/
├── week01/
│   └── practice_vectors.csv
├── week02/
│   ├── messy_survey.csv
│   ├── wellbeing_raw.csv
│   └── questionnaire_codebook.txt
├── week03/
│   ├── visualization_practice.csv
│   └── multiple_conditions.csv
├── week04/
│   ├── grit_scale.csv (existing)
│   └── descriptives_practice.csv
[...continues for each week...]
├── projects/
│   ├── midterm-dataset-optionA.csv
│   ├── midterm-dataset-optionB.csv
│   ├── capstone-dataset-options/ (multiple)
└── README.md (data dictionary for all datasets)
```

**Dataset Characteristics:**
- Real or realistic psychology data
- Variety of research designs
- Different sample sizes (small, medium, large)
- Some with issues (missing data, outliers) for learning
- All include codebooks with variable descriptions

**Potential Data Sources:**
- Open datasets from OSF, published papers
- Simulated data based on realistic parameters
- Anonymized/modified real research data
- Publicly available datasets (e.g., ANES, GSS for US examples)

---

### 4.4 Interactive Elements

#### **WebR Expansions**

Currently using WebR for Part 1 practice in each lab

Expand to:
- Dedicated WebR practice page for each concept
- Self-paced challenges with progressive difficulty
- "Fix this code" exercises
- "Predict the output" quizzes

New interactive features:
- Simulation sliders (e.g., adjust sample size, see effect on CI width)
- Interactive plots (plotly integration)
- Step-by-step guided analysis (reveal next step after completion)

#### **Shiny Apps** (Optional advanced feature)

Develop Shiny apps for concept demonstration:

1. **Central Limit Theorem Explorer**
   - Adjust population distribution shape
   - Adjust sample size
   - See sampling distribution update in real-time

2. **Statistical Power Calculator**
   - Inputs: effect size, alpha, sample size
   - Visualize power curves

3. **P-Value Demonstration**
   - Show distribution under null
   - Mark critical values
   - Shade p-value region

4. **ANOVA Interaction Explorer**
   - Adjust group means
   - See interaction plot update
   - Understand ordinal vs. disordinal interactions

5. **Regression Assumptions Checker**
   - Upload data or use example
   - Generate all diagnostic plots
   - Interpret results

---

## Part 5: Implementation Roadmap

### 5.1 Development Phases

#### **Phase 1: Foundation (Weeks 1-3 of development)**

**Priority:** Create new foundational modules

Deliverables:
- ✅ Complete Week 1: R Foundations module
  - All parts with slides and WebR practice
  - Exercise template
  - Toolbox sections: setup.qmd, rstudio-tour.qmd
  
- ✅ Complete Week 2: Data Import & Wrangling
  - All parts with examples
  - Exercise with messy data
  - Expand toolbox/wrangle.qmd
  - Expand toolbox/import.qmd
  
- ✅ Complete Week 3: Data Visualization I
  - All parts with comprehensive examples
  - Exercise: recreate figures
  - Expand toolbox/plots.qmd
  - Create ggplot2-for-psychologists cheatsheet

- ✅ Reorganize existing Lab 1 as Week 4
  - Update navigation
  - Add new parts (distributions, outliers)
  - Update cross-references

**Testing:** Run pilot with 5-10 students or colleagues

---

#### **Phase 2: Expansion (Weeks 4-7 of development)**

**Priority:** Expand existing content and add new statistical modules

Deliverables:
- ✅ Complete Week 5: Probability & Sampling (NEW)
  - Interactive simulations
  - Bootstrap demonstrations
  - WebR-heavy for experimentation
  
- ✅ Expand Lab 2 → Week 6
  - Add hypothesis testing foundation parts
  - Expand assumptions
  - Add non-parametric alternatives
  - Update exercises
  
- ✅ Expand Lab 3 → Week 7
  - Enhance assumptions checking
  - Add contrasts section
  - More interaction interpretation
  - Update exercises
  
- ✅ Create Week 8 Mid-Term Project
  - Project template
  - Rubric
  - Example solutions
  - Grading guide

**Testing:** Run Weeks 1-8 as cohesive unit

---

#### **Phase 3: Advanced Content (Weeks 8-10 of development)**

**Priority:** Complete core 12-week programme

Deliverables:
- ✅ Split Lab 4 into Weeks 9-10
  - Week 9: Correlation & Simple Regression (enhanced)
  - Week 10: Multiple Regression (enhanced)
  - Add diagnostics sections
  - Update exercises for each week
  
- ✅ Complete Week 11: Data Viz II & Reporting (NEW)
  - Publication figures
  - Patchwork tutorial
  - Complete Quarto reporting guide
  - APA report template
  - Example research reports
  
- ✅ Complete Week 12: Capstone Project
  - Project guidelines
  - Dataset options
  - Rubric
  - Peer review guidelines
  - Example capstone reports

- ✅ Expand Toolbox (all sections from placeholders to full references)
- ✅ Complete all cheat sheets

**Testing:** Run full 12-week programme pilot

---

#### **Phase 4: Extended Content (Weeks 11-14 of development)**

**Priority:** Add weeks 13-16 for extended programme (optional)

Deliverables:
- ✅ Week 13: Repeated Measures & Mixed Designs
  - Integrate existing Boil in the Bag templates
  - Create full chapter materials
  
- ✅ Week 14: Logistic Regression
  - All chapter parts
  - New Boil in the Bag template
  - Exercise
  
- ✅ Week 15: Advanced Topic A (Choose one initially)
  - Recommend starting with Moderation/Mediation
  
- ✅ Week 16: Advanced Topic B
  - Recommend Open Science & Reproducibility
  - Includes Git basics

**Testing:** Pilot weeks 13-16 with advanced students

---

#### **Phase 5: Polish & Production (Weeks 15-16 of development)**

**Priority:** Finalize all materials and prepare for deployment

Deliverables:
- ✅ Video content creation (priority videos)
- ✅ Final quality assurance on all modules
- ✅ Accessibility audit (alt text, color contrast, screen reader compatibility)
- ✅ Student handbook / syllabus template
- ✅ Instructor guide with teaching notes
- ✅ Assessment bank (quiz questions, exam questions)
- ✅ Marketing materials (course description, promotional content)
- ✅ Setup documentation for instructors adopting materials

---

### 5.2 Technical Infrastructure Updates

#### **Repository Structure**

Reorganize to accommodate expansion:

```
GoldPsychR/
├── README.md
├── _quarto.yml (UPDATE with new structure)
├── index.qmd (UPDATE with 12-week structure)
├── pyproject.toml (for uv)
├── renv.lock (R package management)
│
├── weeks/
│   ├── week01/ (R Foundations - NEW)
│   │   ├── index.qmd
│   │   ├── part1.qmd
│   │   ├── part2.qmd
│   │   ├── part1-slides.qmd
│   │   └── part2-slides.qmd
│   ├── week02/ (Data Wrangling - NEW)
│   ├── week03/ (Visualization I - NEW)
│   ├── week04/ (Descriptives - from Lab 1, EXPANDED)
│   ├── week05/ (Probability - NEW)
│   ├── week06/ (T-Tests - from Lab 2, EXPANDED)
│   ├── week07/ (ANOVA - from Lab 3, EXPANDED)
│   ├── week08/ (Mid-Term Project - NEW)
│   ├── week09/ (Correlation - from Lab 4 Part 1, EXPANDED)
│   ├── week10/ (Multiple Regression - from Lab 4 Part 2, EXPANDED)
│   ├── week11/ (Visualization II & Reporting - NEW)
│   ├── week12/ (Capstone - NEW)
│   ├── week13/ (RM/Mixed ANOVA - OPTIONAL EXTENDED)
│   ├── week14/ (Logistic Regression - OPTIONAL EXTENDED)
│   ├── week15/ (Advanced Topics I - OPTIONAL EXTENDED)
│   └── week16/ (Advanced Topics II - OPTIONAL EXTENDED)
│
├── chapters/ (LEGACY - keep for backwards compatibility, redirect to weeks/)
│   └── [symlinks or redirects to weeks/ structure]
│
├── labs/ (LEGACY - keep for current users)
│   └── [existing lab01-04.qmd with notice about new structure]
│
├── toolbox/ (EXPAND all sections)
│   ├── index.qmd
│   ├── setup.qmd (EXPAND)
│   ├── import.qmd (EXPAND)
│   ├── wrangle.qmd (EXPAND)
│   ├── plots.qmd (EXPAND)
│   ├── tests.qmd (EXPAND)
│   ├── models.qmd (EXPAND)
│   ├── reporting.qmd (EXPAND)
│   ├── troubleshooting.qmd (EXPAND)
│   ├── functions.qmd (NEW)
│   ├── projects.qmd (NEW)
│   ├── git-basics.qmd (NEW)
│   └── packages.qmd (NEW)
│
├── boil_in_the_bag/ (EXPAND)
│   ├── 00_index.qmd
│   ├── 01-09 (existing)
│   ├── 10_logistic_regression.qmd (NEW)
│   ├── 11_repeated_measures_long.qmd (NEW)
│   ├── 12_mediation.qmd (NEW)
│   ├── 13_moderation.qmd (NEW)
│   └── data/ (expand with more templates)
│
├── templates/ (Exercise templates)
│   ├── week01-exercise.qmd (NEW)
│   ├── week02-exercise.qmd (NEW)
│   ├── [...weeks 3-12...]
│   ├── midterm-project.qmd (NEW)
│   ├── capstone-project.qmd (NEW)
│   └── apa-report-template.qmd (NEW)
│
├── followon/ (Additional practice exercises)
│   ├── week04-followon.qmd (from lab1)
│   ├── week06-followon.qmd (from lab2)
│   └── [create for more weeks]
│
├── examples/ (NEW - Model reports)
│   ├── example-descriptive-report.qmd
│   ├── example-experiment-report.qmd
│   ├── example-correlational-report.qmd
│   └── example-full-paper.qmd
│
├── data/ (Reorganize by week)
│   ├── week01/
│   ├── week02/
│   ├── [...all weeks...]
│   ├── projects/
│   └── README.md (data dictionary)
│
├── assets/
│   ├── images/
│   ├── css/
│   ├── cheatsheets/ (NEW)
│   │   ├── dplyr-for-psychologists.pdf
│   │   ├── ggplot2-for-psychologists.pdf
│   │   ├── statistical-tests-decision-tree.pdf
│   │   └── apa-reporting-guide.pdf
│   └── videos/ (NEW - or links to external hosting)
│
├── instructor/ (NEW - Instructor materials)
│   ├── syllabus-template.qmd
│   ├── teaching-notes/
│   │   ├── week01-notes.md
│   │   └── [...all weeks...]
│   ├── rubrics/
│   │   ├── exercise-rubric.md
│   │   ├── midterm-rubric.md
│   │   └── capstone-rubric.md
│   ├── solutions/ (password-protected or separate private repo)
│   └── setup-guide.md
│
└── docs/ (rendered website - output directory)
```

#### **_quarto.yml Updates**

Major updates needed:

1. **Navigation restructure:**
   - Change from 4 labs to 12-week structure
   - Nested sidebar with expandable sections
   - Add Instructor Materials section (hidden for students)
   - Add Resources section (toolbox, templates, examples)

2. **New sections:**
   - Weeks 1-12 (core)
   - Weeks 13-16 (advanced, collapsible)
   - Projects (midterm, capstone)
   - Resources (toolbox, boil in the bag, examples)
   - Student handbook
   - Legacy labs (with deprecation notice)

3. **Metadata updates:**
   - Update title if needed
   - Course dates and schedule
   - Instructor information
   - Assessment information

Example structure addition:

```yaml
  sidebar:
    style: docked
    search: true
    contents:
      - section: "Getting Started"
        contents:
          - text: "Course Home"
            href: index.qmd
          - text: "Syllabus"
            href: syllabus.qmd
          - text: "Setup Instructions"
            href: toolbox/setup.qmd
      
      - text: "---"
      
      - section: "📚 Core Programme (Weeks 1-12)"
        contents:
          - section: "Week 1: R Foundations"
            href: weeks/week01/index.qmd
          - section: "Week 2: Data Wrangling"
            href: weeks/week02/index.qmd
          [... continue for all 12 weeks ...]
      
      - text: "---"
      
      - section: "🚀 Advanced Programme (Weeks 13-16)"
        contents:
          [... advanced weeks ...]
      
      - text: "---"
      
      - section: "📊 Projects"
        contents:
          - text: "Mid-Term Project"
            href: projects/midterm.qmd
          - text: "Capstone Project"
            href: projects/capstone.qmd
      
      - text: "---"
      
      - section: "🔧 Resources"
        contents:
          - text: "R Toolbox"
            href: toolbox/index.qmd
          - text: "Boil in the Bag Templates"
            href: boil_in_the_bag/00_index.qmd
          - text: "Example Reports"
            href: examples/index.qmd
          - text: "Cheat Sheets"
            href: resources/cheatsheets.qmd
```

#### **Website Features to Add**

1. **Search Enhancement:**
   - Index all content for better search
   - Add search filters (by week, by topic, by resource type)

2. **Progress Tracking:**
   - Student dashboard (if using LMS integration)
   - Checkboxes for completed modules
   - Personal notes feature

3. **Discussion Integration:**
   - Hypothesis.is for inline commenting
   - Link to discussion forum for each page

4. **Accessibility:**
   - Alt text for all images
   - Keyboard navigation
   - Screen reader compatibility
   - Transcript for videos
   - Color contrast compliance (WCAG AA)

5. **Mobile Optimization:**
   - Ensure responsive design works well
   - Test WebR on mobile devices
   - Optimize for touch interfaces

---

### 5.3 Sustainability & Maintenance

#### **Version Control Strategy**

Use Git branches for development:

- `main`: Current stable 4-lab version
- `develop`: Extended 12-week programme development
- `feature/*`: Individual feature branches
- `release/*`: Version releases

#### **Documentation**

Create comprehensive docs:

1. **CONTRIBUTING.md**: Guide for contributors
2. **CHANGELOG.md**: Version history
3. **instructor/README.md**: Guide for instructors adopting materials
4. **data/README.md**: Complete data dictionary

#### **Community Building**

- Open GitHub Discussions for Q&A
- Create instructor community forum
- Solicit feedback from users
- Annual review and update cycle

#### **Licensing**

Current implicit license: open educational resource

Consider explicit licensing:
- Content: CC BY-SA 4.0 (allow remixing with attribution)
- Code: MIT License (permissive)

#### **Citation**

Provide citation information:
```
Wright, G. (2026). GoldPsychR: R Statistics Training for Psychology. 
Goldsmiths, University of London. 
https://github.com/LittleMonkeyLab/GoldPsychR
```

---

## Part 6: Resource Requirements

### 6.1 Human Resources

#### **Development Team**

**Lead Instructor/Content Developer** (Principal role - likely you)
- Course design and pedagogy
- Content writing
- Code examples and datasets
- Estimated: 200-300 hours total development

**Breakdown by Phase:**
- Phase 1 (Foundation): 60 hours
- Phase 2 (Expansion): 60 hours
- Phase 3 (Advanced): 60 hours
- Phase 4 (Extended): 40 hours
- Phase 5 (Polish): 40 hours

**Supporting Roles** (if available)

- **Instructional Designer** (10-20 hours)
  - Pedagogical review
  - Assessment design
  - Learning objectives alignment

- **Statistical Consultant** (10 hours)
  - Review statistical content for accuracy
  - Suggest additional topics

- **Technical Developer** (20-30 hours)
  - Quarto customization
  - WebR integration enhancements
  - Shiny app development (if pursued)

- **Student Assistants** (30-40 hours)
  - Test exercises
  - Identify unclear instructions
  - Check for errors

- **Graphic Designer** (Optional, 10 hours)
  - Create custom diagrams
  - Design cheat sheets
  - Enhance visual appeal

- **Video Producer** (Optional, 20 hours)
  - Film and edit videos
  - Add captions
  - Optimize for streaming

### 6.2 Technical Resources

#### **Software**

All open source and free:
- ✅ R and RStudio (free)
- ✅ Quarto (free)
- ✅ Git/GitHub (free for public repos)
- ✅ RStudio Server (already have access)

#### **Hosting**

Current: GitHub Pages (free)
Sufficient for expanded programme

Alternatives if needed:
- Netlify (free tier)
- Vercel (free tier)

#### **Data Storage**

- Small datasets: Store in GitHub repo (current approach)
- Larger datasets: OSF, Zenodo, or institutional repository
- Videos: YouTube (free, embed in pages)

#### **Tools for Creation**

- Screen recording: OBS Studio (free), Loom (free tier)
- Graphic design: Canva (education free), Inkscape (free)
- Diagramming: draw.io (free), Mermaid in Quarto
- PDF cheat sheets: R Markdown to PDF or Canva

---

### 6.3 Financial Resources

#### **Minimal Budget Scenario** (All open source, DIY)

Total: £0 - £500

- Domain name (optional): £10/year
- Video hosting: £0 (YouTube)
- Software: £0 (all open source)
- Time: Volunteer/embedded in role
- Student testing: Current students as pilot

#### **Moderate Budget Scenario** (Professional polish)

Total: £2,000 - £5,000

- Development time: £0 (embedded in role)
- Student assistant stipends: £500-1000 (10-20 hrs @ £10-15/hr)
- Professional video editing: £500-1000
- Graphic design for cheat sheets: £500-1000
- Accessibility audit: £500
- Pilot workshop expenses: £500 (refreshments, venue if needed)

#### **Ideal Budget Scenario** (Full production)

Total: £8,000 - £15,000

- Lead developer time: £5,000-8,000 (as buyout or summer salary)
- Student assistants: £1,000-2,000
- Professional video production: £2,000-3,000
- Graphic design: £1,000-2,000
- Accessibility consultant: £1,000
- Pilot workshops: £1,000

---

## Part 7: Evaluation Plan

### 7.1 Formative Evaluation (During Development)

#### **Expert Review**

Recruit 3-5 experts to review materials:
- Statistics education specialist
- R programming expert
- Psychology research methods instructor
- Educational technology specialist

Provide:
- Draft materials
- Review rubric
- Feedback survey

Timeline: After each development phase

#### **Student Pilot Testing**

**Alpha Testing** (Phase 1-2):
- 5-10 students
- Weekly feedback sessions
- Think-aloud protocol while using materials

**Beta Testing** (Phase 3):
- Full cohort (20-40 students)
- Use in actual course
- Pre/post assessments
- Weekly surveys

#### **Iterative Revision**

After each round of testing:
1. Collect feedback
2. Identify issues and confusion points
3. Prioritize revisions
4. Implement changes
5. Document changes in CHANGELOG.md

---

### 7.2 Summative Evaluation (Post-Implementation)

#### **Student Learning Outcomes**

**Quantitative Measures:**

1. **Knowledge Assessment**
   - Pre-test (Week 1)
   - Mid-term exam (Week 8)
   - Post-test (Week 12)
   - Compare gains

2. **Skills Assessment**
   - Exercise scores
   - Project scores
   - Code quality rubric scores

3. **Confidence Survey**
   - Self-efficacy in R programming
   - Self-efficacy in statistical analysis
   - Comfort with data analysis
   - Administered pre/post

**Qualitative Measures:**

1. **Open-Ended Feedback**
   - What worked well?
   - What was confusing?
   - What would you change?
   - Most valuable components?

2. **Focus Groups**
   - End-of-semester focus group (6-8 students)
   - Discuss learning experience
   - Gather suggestions

3. **Reflective Essays**
   - Final reflection on learning journey
   - What skills will you use in future?

#### **Instructor Experience**

If materials used by other instructors:

1. **Instructor Survey**
   - Ease of implementation
   - Student engagement
   - Material quality
   - Needed modifications

2. **Instructor Interviews**
   - Semi-structured interviews
   - Implementation challenges
   - Student response
   - Suggestions for improvement

#### **Usage Analytics**

If website analytics available:

- Page views by section
- Time spent on pages
- Most/least accessed resources
- Search queries
- Bounce rates

Insights:
- Which topics need more explanation?
- Which resources are most valuable?
- Where are students getting stuck?

---

### 7.3 Continuous Improvement

#### **Annual Review Cycle**

**Summer (May-August):**
- Review feedback from previous year
- Update content based on feedback
- Add new examples or datasets
- Update package code for new package versions
- Refresh readings and references

**Autumn (September-October):**
- Prepare for new cohort
- Test all code and links
- Update dates and schedule
- Review and update assessments

**Spring (March-April):**
- Mid-year check-in
- Address any urgent issues
- Collect ongoing feedback

#### **Version Releases**

Use semantic versioning:
- Major version (1.0, 2.0): Significant restructuring
- Minor version (1.1, 1.2): New content or features
- Patch (1.1.1): Bug fixes and small updates

Current: Version 0.9 (4-lab programme)
Target: Version 1.0 (12-week programme complete)
Future: Version 1.1 (with 16-week extended content)

---

## Part 8: Adoption & Dissemination

### 8.1 Internal Adoption (Goldsmiths)

#### **Course Integration**

Potential courses at Goldsmiths:
- PS51020A R Labs (current)
- Research Methods modules across years
- MSc dissertation preparation modules
- Continuing Professional Development workshops

#### **Instructor Training**

Provide training for other instructors:
- Workshop on using materials
- Office hours for questions
- Instructor handbook
- Teaching notes for each week

---

### 8.2 External Dissemination

#### **Open Educational Resource**

Make materials freely available:
- Public GitHub repository (already is)
- Clear licensing (CC BY-SA)
- Easy for others to fork and adapt

#### **Academic Presentations**

Present at conferences:
- Psychology Teaching Conference
- RStudio Conference (now posit::conf)
- Teaching Statistics in Psychology (TSIP) group
- European Association for Research on Learning and Instruction (EARLI)

Possible presentation titles:
- "From Four Sessions to Full Semester: Scaling an R Statistics Course"
- "Integrating WebR for Browser-Based R Learning in Psychology"
- "Teaching Reproducible Research with Quarto: A Case Study"

#### **Publication**

Write article for teaching-focused journal:
- *Teaching of Psychology*
- *Journal of Statistics Education*
- *Psychology Learning & Teaching*

Article focus:
- Pedagogical approach
- Evidence of effectiveness
- Lessons learned
- How others can adopt

#### **Workshops for Other Institutions**

Offer workshops on:
- Adopting GoldPsychR materials
- Teaching R for psychology research
- Building Quarto-based courses

#### **Social Media & Blog**

Share updates and resources:
- Twitter/Mastodon: @GoldPsychR
- Blog posts on LittleMonkeyLab site
- YouTube channel for videos

---

## Part 9: Alternative Configurations

### 9.1 Intensive Workshop Format

**Duration:** 5 days (9am-5pm)

**Use Case:** Summer school, professional development

**Schedule:**

| Day | Morning (9am-12pm) | Afternoon (1pm-5pm) |
|-----|-------------------|-------------------|
| **Monday** | Week 1: R Foundations | Week 2: Data Wrangling |
| **Tuesday** | Week 3: Visualization | Week 4: Descriptives & Week 5: Probability |
| **Wednesday** | Week 6: T-Tests | Week 7: ANOVA |
| **Thursday** | Week 9: Correlation | Week 10: Multiple Regression |
| **Friday** | Week 11: Reporting | Capstone Mini-Project |

**Adaptations Needed:**
- Condensed slides
- Shorter exercises
- Take-home materials for deeper practice
- Focus on essentials only
- Provide resources for continued learning

---

### 9.2 Flipped Classroom Format

**Use Case:** In-person class time is limited

**Structure:**
- Pre-class: Watch slides, complete WebR practice
- In-class: Exercise work time, troubleshooting, discussion
- Post-class: Follow-on exercise, discussion forum

**Benefits:**
- More active learning in class
- Instructor available for help during practice
- Students come prepared

**Adaptations Needed:**
- Clear pre-class expectations
- In-class activity plans for instructors
- Participation tracking

---

### 9.3 Asynchronous Online Format

**Use Case:** Distance learning, self-paced

**Structure:**
- All materials online
- Weekly modules released (or all at once for self-paced)
- Discussion forums for interaction
- Virtual office hours
- Peer review for projects

**Adaptations Needed:**
- More detailed written instructions (less assumed instructor demo)
- Video tutorials for all topics
- Automated code checking where possible
- Strong discussion forum moderation

---

### 9.4 Blended Format

**Use Case:** Hybrid in-person/online

**Structure:**
- Weeks 1, 4, 7, 10, 12: In-person lab sessions
- Other weeks: Asynchronous online
- In-person sessions for key milestones and projects

**Benefits:**
- Balance of personal contact and flexibility
- In-person for complex topics
- Online for practice and reinforcement

---

## Part 10: Risk Assessment & Mitigation

### 10.1 Potential Risks

#### **Risk 1: Scope Creep**

**Description:** Adding too many topics, overwhelming students and delaying completion

**Likelihood:** High  
**Impact:** High

**Mitigation:**
- Stick to development roadmap strictly
- Define "must have" vs. "nice to have" content
- Use modular structure so advanced topics are optional
- Schedule regular scope review meetings

---

#### **Risk 2: Technical Issues**

**Description:** WebR compatibility problems, RStudio Server downtime, package updates breaking code

**Likelihood:** Medium  
**Impact:** Medium-High

**Mitigation:**
- Use renv for package version control
- Test on multiple browsers for WebR
- Have backup plan if RStudio Server down (local RStudio)
- Provide fallback instructions
- Test all code before each semester
- Monitor package updates and deprecations

---

#### **Risk 3: Student Overwhelm**

**Description:** Expanded programme too difficult, students fall behind, high drop-out

**Likelihood:** Medium  
**Impact:** High

**Mitigation:**
- Careful pacing and scaffolding
- Formative feedback to identify struggling students early
- Office hours and support systems
- Clear prerequisites and expectations
- Optional review sessions
- Peer study groups

---

#### **Risk 4: Insufficient Resources**

**Description:** Not enough time or funding to complete development

**Likelihood:** Medium  
**Impact:** High

**Mitigation:**
- Prioritize core 12-week programme first
- Advanced content (13-16) can be added later
- Use minimal budget approach if needed
- Seek internal funding (teaching innovation grants)
- Collaborate with other institutions to share development

---

#### **Risk 5: Low Adoption**

**Description:** Materials developed but not used widely

**Likelihood:** Low (internal use likely)  
**Impact:** Medium

**Mitigation:**
- Ensure materials meet specific institutional needs first
- Active dissemination at conferences
- Provide excellent documentation for adopters
- Build community around materials
- Solicit feedback and incorporate suggestions

---

#### **Risk 6: Outdated Content**

**Description:** R packages update, best practices change, materials become obsolete

**Likelihood:** High (over time)  
**Impact:** Medium

**Mitigation:**
- Annual review and update cycle
- Use renv for reproducibility
- Document package versions in materials
- Assign maintainer role
- GitHub Issues for community to report problems
- Keep materials version controlled

---

## Part 11: Success Metrics

### 11.1 Development Metrics

**Phase Completion:**
- ✅ Phase 1 complete by [target date]
- ✅ Phase 2 complete by [target date]
- ✅ Phase 3 complete by [target date]
- ✅ 12-week programme ready for pilot by [target date]

**Content Completeness:**
- ✅ All 12 weeks have complete materials
- ✅ All toolbox sections expanded from placeholders
- ✅ All exercises have solutions
- ✅ All assessments have rubrics

**Quality Assurance:**
- ✅ All code tested and runs
- ✅ All links functional
- ✅ Accessibility audit passed
- ✅ Peer review completed

---

### 11.2 Student Learning Metrics

**Knowledge Gains:**
- Pre-to-post test score improvement > 30%
- > 80% of students score 70%+ on final project
- Mid-term pass rate > 85%

**Skill Development:**
- > 75% of students complete independent analysis by Week 12
- > 80% report confidence in using R for research
- > 70% report ability to learn new R techniques independently

**Engagement:**
- > 80% completion rate for exercises
- > 70% engagement in discussion forums
- Average course evaluation > 4.0/5.0

**Transfer:**
- > 50% of students use R in subsequent courses/research
- > 30% of students contribute to open science (share code/data)

---

### 11.3 Dissemination Metrics

**Adoption:**
- Materials used by > 3 instructors at Goldsmiths by Year 2
- Materials used by > 5 external institutions by Year 3
- GitHub stars > 100 by Year 2

**Visibility:**
- Presented at > 2 conferences by Year 2
- Published teaching article by Year 3
- > 10,000 website visits per year by Year 2

**Community:**
- Active GitHub discussions/issues
- > 50 GitHub forks by Year 3
- Testimonials from adopting instructors

---

## Part 12: Next Steps & Decision Points

### 12.1 Immediate Actions (Next 1-2 Weeks)

1. **Review this plan** with stakeholders
   - Course coordinator
   - Department head
   - Student representatives

2. **Decide on scope**
   - 12-week programme only, or include 16-week extended?
   - Which optional topics to prioritize?

3. **Confirm resources**
   - Development time available?
   - Any budget available?
   - Student assistants accessible?

4. **Create project timeline**
   - Map development phases to calendar dates
   - Identify critical milestones
   - Set pilot date target

5. **Set up development infrastructure**
   - Create development branch in Git
   - Set up project management (GitHub Projects, Trello, etc.)
   - Establish regular check-in schedule

---

### 12.2 Key Decision Points

#### **Decision 1: Programme Length**

**Options:**
- A) 12-week core programme only (faster development)
- B) 12-week core + 16-week extended (more comprehensive)
- C) Modular self-paced (flexible for different audiences)

**Recommendation:** Start with Option A (12 weeks), add extended content in Phase 4 if resources allow

---

#### **Decision 2: Level of Interactivity**

**Options:**
- A) Keep current WebR approach (good)
- B) Add Shiny apps for demonstrations (better but more time)
- C) Add videos for all topics (better but requires production)

**Recommendation:** Keep WebR (Option A), add priority videos, skip Shiny for now (can add later)

---

#### **Decision 3: Assessment Approach**

**Options:**
- A) Formative only (self-check quizzes, no grading)
- B) Formative + exercises (graded exercises each week)
- C) Formative + exercises + midterm + capstone (full assessment)

**Recommendation:** Option C for formal course, Option A if just providing resources

---

#### **Decision 4: Backwards Compatibility**

**Options:**
- A) Maintain legacy 4-lab structure alongside new structure
- B) Redirect legacy to new structure with mapping
- C) Archive legacy and fully switch to new

**Recommendation:** Option A initially (both available), then Option B after 1 year

---

### 12.3 Consultation Questions

Before proceeding, seek input on:

1. **From students:**
   - What additional topics would be most valuable?
   - What learning resources are most helpful (videos, examples, practice)?
   - How much weekly time can you dedicate to R learning?

2. **From instructors:**
   - What topics do students struggle with most?
   - What resources would make teaching easier?
   - Interest in adopting expanded materials?

3. **From department:**
   - Alignment with curriculum and learning outcomes?
   - Resource availability (time, funding, space)?
   - Strategic fit with department goals?

4. **From university:**
   - Interest in showcasing as OER example?
   - Support for dissemination?
   - Teaching innovation funding available?

---

## Appendices

### Appendix A: Recommended R Packages

**Core tidyverse packages** (already included):
- ggplot2: visualization
- dplyr: data manipulation
- tidyr: data tidying
- readr: data import
- purrr: functional programming
- tibble: modern data frames
- stringr: string manipulation
- forcats: factor handling

**Statistical packages:**
- psych: psychology-specific stats, scale reliability
- afex: ANOVA with proper error terms
- emmeans: estimated marginal means, post-hocs
- effectsize: effect size calculations
- car: Levene's test, VIF for regression
- lme4: mixed-effects models
- lavaan: structural equation modeling
- mediation: mediation analysis
- pwr: power analysis

**Reporting packages:**
- knitr: R Markdown/Quarto engine
- kableExtra: enhanced tables
- gt: grammar of tables
- papaja: APA manuscripts in R Markdown
- report: automated reporting

**Utility packages:**
- here: path management
- janitor: data cleaning
- skimr: data overview
- naniar: missing data visualization

---

### Appendix B: External Resources & Readings

**Books (Free Online):**
- *R for Data Science* (2e) by Wickham, Çetinkaya-Rundel, & Grolemund: https://r4ds.hadley.nz/
- *Learning Statistics with R* by Navarro: https://learningstatisticswithr.com/
- *Statistical Thinking for the 21st Century* by Poldrack: https://statsthinking21.github.io/statsthinking21-core-site/
- *Introduction to Modern Statistics* by Çetinkaya-Rundel & Hardin: https://openintro-ims.netlify.app/

**Websites:**
- RStudio Education: https://education.rstudio.com/
- R-Bloggers: https://www.r-bloggers.com/
- Stack Overflow (R tag): https://stackoverflow.com/questions/tagged/r
- Posit Community: https://community.rstudio.com/

**Papers:**
- Horton et al. (2015). Teaching the next generation of statistics students to "Think with Data"
- Legler & Roback (2019). Broadening perspectives on statistics education
- McNamara (2019). Teaching R to new users

---

### Appendix C: Sample Syllabus Outline

**Course Title:** R for Psychological Research  
**Level:** Undergraduate Year 2 or 3  
**Credits:** 15 credits (UK) / 3 credits (US)  
**Prerequisites:** Introduction to Statistics (descriptives, t-tests, ANOVA, regression)  
**Format:** 12 weeks, 2-hour lab + self-study

**Learning Outcomes:**
By the end of this course, students will be able to:
1. Import, clean, and manipulate psychological research data using R
2. Create publication-quality visualizations using ggplot2
3. Conduct and interpret common statistical tests (t-tests, ANOVA, regression)
4. Check assumptions and diagnose problems in statistical models
5. Write reproducible research reports using Quarto
6. Follow best practices for data ethics and open science

**Assessment:**
- Weekly exercises (30%): Best 8 of 10
- Mid-term project (30%): Analysis of provided dataset
- Final capstone project (40%): Independent analysis with full report

**Weekly Schedule:**
- Week 1: R Foundations
- Week 2: Data Wrangling
- Week 3: Data Visualization
- [... continue for all 12 weeks ...]

**Required Materials:**
- Computer with internet access (RStudio Server provided)
- No textbook required (all materials open access)

**Support:**
- Lab time: [days/times]
- Office hours: [times]
- Discussion forum: [link]
- Email: [email]

---

### Appendix D: Glossary of Terms

**Quarto:** Open-source technical publishing system, successor to R Markdown

**WebR:** R running in the browser via WebAssembly, no installation needed

**Tidyverse:** Collection of R packages for data science with consistent design

**Boil in the Bag:** Ready-made statistical analysis templates, named after convenient prepared meals

**Follow-On:** Additional practice exercises using different datasets to promote transfer

**renv:** R package for managing project-specific package libraries (reproducibility)

**OER:** Open Educational Resource - freely accessible teaching materials

**APA:** American Psychological Association (style guide for psychology writing)

---

## Conclusion

This expansion plan provides a comprehensive roadmap for transforming the current **GoldPsychR** 4-session course into a full semester-long (12-16 week) R statistics training programme. 

**Key Strengths of This Plan:**
1. **Builds on existing excellence:** Retains the effective pedagogical approach while expanding scope
2. **Modular structure:** Allows flexible adoption (12-week, 16-week, or custom configurations)
3. **Practical focus:** Emphasizes real psychology research contexts and reproducible workflows
4. **Resource-conscious:** Can be implemented with minimal budget using open-source tools
5. **Sustainable:** Includes maintenance and continuous improvement plans
6. **Shareable:** Designed as an OER for wider adoption

**Next Steps:**
1. Review this plan with stakeholders and gather feedback
2. Make key decisions on scope and resources
3. Begin Phase 1 development (Weeks 1-3 foundation modules)
4. Pilot test and iterate
5. Expand to full 12-week programme
6. Disseminate and build community

The resulting programme will provide psychology students with comprehensive, practical R skills for modern research while serving as a model for statistics education in other disciplines.

---

**Document Prepared By:** Cloud Agent  
**Date:** August 8, 2026  
**Version:** 1.0  
**Next Review:** After stakeholder feedback
