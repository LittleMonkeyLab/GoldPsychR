# GoldPsychR: Course Structure Comparison

**Visual guide to understand the transformation from 4 labs to 12-16 week programme**

---

## 📊 Visual Comparison

### Current Structure (4 Labs × 2 hours = 8 hours)

```
┌─────────────────────────────────────────────────────────────┐
│  LAB 1: DESCRIPTIVE STATISTICS (2 hours)                    │
│  • Load data                                                │
│  • Reverse scoring                                          │
│  • Calculate descriptives                                   │
│  • Create boxplots                                          │
│  • Write APA results                                        │
│  Data: Grit Scale (120 students)                           │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  LAB 2: T-TESTS (2 hours)                                   │
│  • One-sample t-test                                        │
│  • Independent samples t-test                               │
│  • Paired samples t-test                                    │
│  • Calculate Cohen's d                                      │
│  • Write APA results                                        │
│  Data: Test anxiety data                                   │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  LAB 3: ANOVA (2 hours)                                     │
│  • One-way ANOVA                                            │
│  • Two-way ANOVA                                            │
│  • Post-hoc tests (Tukey HSD)                              │
│  • Effect sizes (η²)                                        │
│  • Write APA results                                        │
│  Data: Study techniques experiment                          │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  LAB 4: CORRELATION & REGRESSION (2 hours)                  │
│  • Correlation (Pearson's r)                                │
│  • Simple regression                                        │
│  • Multiple regression                                      │
│  • Diagnostics (brief)                                      │
│  • Write APA results                                        │
│  Data: Cognitive performance data                           │
└─────────────────────────────────────────────────────────────┘
```

**Assumptions:** Students know R basics, can wrangle data, understand ggplot2

---

### Proposed Structure (12 Weeks × 2+ hours = 24+ hours)

```
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 1: R FOUNDATIONS (2 hours)                         │
│  • RStudio interface tour                                   │
│  • Variables and assignment                                 │
│  • Data types and vectors                                   │
│  • Basic functions                                          │
│  • Installing packages                                      │
│  • Reading documentation                                    │
│  NEW CONTENT - Foundation previously assumed                │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 2: DATA WRANGLING (2 hours)                        │
│  • Importing CSV, Excel, SPSS                              │
│  • Introduction to tidyverse                                │
│  • select(), filter(), mutate()                            │
│  • Pipes (%>% and |>)                                      │
│  • group_by() and summarize()                              │
│  • Handling missing data                                    │
│  NEW CONTENT - Critical foundation                          │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 3: DATA VISUALIZATION I (2 hours)                  │
│  • ggplot2 grammar of graphics                             │
│  • geom_point, geom_bar, geom_boxplot                      │
│  • Aesthetics (color, fill, shape)                         │
│  • Themes and customization                                 │
│  • Faceting for grouped plots                               │
│  • Color palettes                                           │
│  NEW CONTENT - ggplot2 properly taught                      │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  ✨ WEEK 4: DESCRIPTIVE STATISTICS (2 hours)                │
│  FROM LAB 1 + ENHANCED:                                     │
│  • Load data (now they know how!)                          │
│  • Reverse scoring (using mutate)                          │
│  • Calculate descriptives                                   │
│  • Create boxplots (they understand ggplot2!)              │
│  🆕 NEW ADDITIONS:                                          │
│  • Distributions and normality                              │
│  • Detecting outliers (IQR, z-scores)                      │
│  • Data transformations                                     │
│  Data: Grit Scale (same)                                   │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 5: PROBABILITY & SAMPLING (2 hours)                │
│  • Probability distributions                                │
│  • Normal distribution and z-scores                         │
│  • Sampling distributions                                   │
│  • Central Limit Theorem (simulation)                       │
│  • Standard error vs. SD                                    │
│  • Confidence intervals                                     │
│  NEW CONTENT - Foundation for inference                     │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  ✨ WEEK 6: HYPOTHESIS TESTING & T-TESTS (2 hours)         │
│  FROM LAB 2 + ENHANCED:                                     │
│  • One-sample t-test                                        │
│  • Independent samples t-test                               │
│  • Paired samples t-test                                    │
│  • Cohen's d effect sizes                                   │
│  🆕 NEW ADDITIONS:                                          │
│  • Null vs. alternative hypotheses                          │
│  • P-values explained (common misinterpretations)          │
│  • Type I and Type II errors                                │
│  • Assumptions checking with plots                          │
│  • Non-parametric alternatives (Mann-Whitney, Wilcoxon)    │
│  Data: Test anxiety (same) + new examples                  │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  ✨ WEEK 7: ANOVA & FACTORIAL DESIGNS (2 hours)            │
│  FROM LAB 3 + ENHANCED:                                     │
│  • One-way ANOVA                                            │
│  • Two-way ANOVA                                            │
│  • Post-hoc tests (Tukey)                                   │
│  • Effect sizes (η²)                                        │
│  🆕 NEW ADDITIONS:                                          │
│  • Detailed assumptions checking                            │
│  • Planned contrasts vs. post-hoc                          │
│  • Partial eta-squared                                      │
│  • Interaction plots and interpretation                     │
│  • Non-parametric alternatives (Kruskal-Wallis)            │
│  Data: Study techniques (same) + new examples              │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 8: MID-TERM PROJECT (2-4 hours)                   │
│  • Provided dataset OR choose from options                  │
│  • Apply skills from Weeks 1-7                             │
│  • Research question → analysis → interpretation            │
│  • Deliverable: Quarto report (3-4 pages)                  │
│  • Peer feedback (formative)                                │
│  NEW CONTENT - Integrative assessment                       │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  ✨ WEEK 9: CORRELATION & SIMPLE REGRESSION (2 hours)      │
│  FROM LAB 4 PART 1 + ENHANCED:                             │
│  • Scatterplots with trend lines                            │
│  • Pearson's r and Spearman's rho                          │
│  • Correlation assumptions                                  │
│  • Simple linear regression (lm)                            │
│  • Interpreting slope and intercept                         │
│  • R² as explained variance                                 │
│  🆕 NEW ADDITIONS:                                          │
│  • Detailed assumptions checking                            │
│  • Residual plots and diagnostics                           │
│  • Prediction and confidence intervals                      │
│  Data: Cognitive performance (same) + expanded              │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  ✨ WEEK 10: MULTIPLE REGRESSION (2 hours)                 │
│  FROM LAB 4 PART 2 + ENHANCED:                             │
│  • Adding multiple predictors                               │
│  • Adjusted R²                                              │
│  • Interpreting coefficients                                │
│  • Model comparison with anova()                            │
│  🆕 NEW ADDITIONS:                                          │
│  • Multicollinearity (VIF)                                  │
│  • Standardized coefficients (beta weights)                 │
│  • Categorical predictors (dummy coding)                    │
│  • Hierarchical regression                                  │
│  • Model selection (AIC, BIC intro)                         │
│  Data: Extended regression examples                         │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 11: VISUALIZATION II & REPORTING (2 hours)        │
│  • Publication-quality figures                              │
│  • Multi-panel figures (patchwork)                          │
│  • Figure legends and captions                              │
│  • Quarto for academic writing                              │
│  • YAML headers and cross-references                        │
│  • Bibliography management                                   │
│  • Exporting for publication                                │
│  • Complete reproducible workflow                           │
│  NEW CONTENT - Professional communication                   │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🆕 WEEK 12: CAPSTONE PROJECT (4+ hours)                   │
│  • Open dataset from your area OR provided options          │
│  • Complete research cycle                                  │
│  • Research question → design → analysis → report           │
│  • Deliverable: Full Quarto report (6-8 pages)             │
│  • All code included and documented                         │
│  • Publication-quality figures                              │
│  • Peer review component                                    │
│  NEW CONTENT - Culminating independent work                 │
└─────────────────────────────────────────────────────────────┘
```

**Result:** Students now have solid foundations, understand the full workflow, and can work independently

---

### Optional Extended Programme (Weeks 13-16)

```
┌─────────────────────────────────────────────────────────────┐
│  🎓 WEEK 13: REPEATED MEASURES & MIXED DESIGNS (2 hours)   │
│  • Within-subjects designs                                  │
│  • Repeated measures ANOVA                                  │
│  • Sphericity assumption (Mauchly's test)                  │
│  • Greenhouse-Geisser correction                           │
│  • Mixed (split-plot) ANOVA                                │
│  • Using afex or ez package                                │
│  ADVANCED CONTENT - Complex designs                         │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🎓 WEEK 14: LOGISTIC REGRESSION (2 hours)                 │
│  • Binary outcomes                                          │
│  • Logit transformation                                     │
│  • Odds ratios interpretation                               │
│  • glm() for logistic regression                           │
│  • Predicted probabilities                                  │
│  • Model fit and ROC curves                                │
│  ADVANCED CONTENT - Categorical outcomes                    │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🎓 WEEK 15: ADVANCED TOPICS I (2 hours)                   │
│  CHOOSE ONE:                                                │
│  A) Moderation and Mediation                               │
│     • Conceptual frameworks                                 │
│     • Testing moderation with interactions                  │
│     • Mediation analysis (lavaan or mediation pkg)         │
│  B) Non-Parametric Tests                                   │
│     • When parametric assumptions fail                      │
│     • Rank-based methods                                    │
│     • Mann-Whitney, Wilcoxon, Kruskal-Wallis              │
│  C) Power Analysis                                          │
│     • Statistical power concepts                            │
│     • Using pwr package                                     │
│     • Sample size planning                                  │
│  ADVANCED CONTENT - Specialized topics                      │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  🎓 WEEK 16: ADVANCED TOPICS II (2 hours)                  │
│  CHOOSE ONE:                                                │
│  A) Introduction to Mixed-Effects Models                   │
│     • Hierarchical/nested data                              │
│     • Fixed vs. random effects                              │
│     • Using lme4::lmer()                                    │
│  B) Reproducible Research & Open Science                   │
│     • Git and GitHub basics                                 │
│     • Project organization                                  │
│     • Sharing on OSF                                        │
│     • Preregistration                                       │
│  C) Data Ethics and Privacy                                │
│     • GDPR and data protection                             │
│     • Anonymization techniques                              │
│     • Ethical visualization                                 │
│  ADVANCED CONTENT - Professional practice                   │
└─────────────────────────────────────────────────────────────┘
```

---

## 📊 Content Growth Comparison

### Coverage Matrix

| Topic Area | Current (4 Labs) | Proposed (12 Weeks) | Extended (16 Weeks) |
|------------|------------------|---------------------|---------------------|
| **R Basics** | Assumed | ✅ Week 1 (Full) | ✅ Week 1 |
| **Data Wrangling** | Brief | ✅ Week 2 (Full) | ✅ Week 2 |
| **Visualization** | Intro only | ✅ Weeks 3 & 11 (Full) | ✅ Weeks 3 & 11 |
| **Descriptives** | ✅ Lab 1 | ✅ Week 4 (Enhanced) | ✅ Week 4 |
| **Probability** | Not covered | ✅ Week 5 (New) | ✅ Week 5 |
| **T-Tests** | ✅ Lab 2 | ✅ Week 6 (Enhanced) | ✅ Week 6 |
| **ANOVA** | ✅ Lab 3 | ✅ Week 7 (Enhanced) | ✅ Week 7 |
| **Correlation** | ✅ Lab 4 Part | ✅ Week 9 (Enhanced) | ✅ Week 9 |
| **Regression** | ✅ Lab 4 Part | ✅ Weeks 9-10 (Full) | ✅ Weeks 9-10 |
| **Projects** | None | ✅ Weeks 8 & 12 (New) | ✅ Weeks 8 & 12 |
| **Reporting** | Brief | ✅ Week 11 (Full) | ✅ Week 11 |
| **RM/Mixed ANOVA** | Not covered | Template only | ✅ Week 13 |
| **Logistic Reg** | Not covered | Template only | ✅ Week 14 |
| **Advanced Topics** | Not covered | Not covered | ✅ Weeks 15-16 |

### Skill Development Comparison

| Skill | Current | After 12 Weeks | After 16 Weeks |
|-------|---------|----------------|----------------|
| **Navigate RStudio** | Assumed | ✅ Confident | ✅ Expert |
| **Import/Clean Data** | Basic | ✅ Proficient | ✅ Expert |
| **Create Plots** | Basic | ✅ Proficient | ✅ Expert |
| **Run Basic Tests** | ✅ Can do | ✅ Can do + understand | ✅ Can do + extend |
| **Check Assumptions** | Limited | ✅ Proficient | ✅ Expert |
| **Interpret Results** | ✅ Can do | ✅ Confident | ✅ Expert |
| **Write Reports** | Basic | ✅ Proficient (Quarto) | ✅ Expert |
| **Independent Analysis** | ❌ Not ready | ✅ Ready | ✅ Highly skilled |
| **Learn New Techniques** | ❌ Difficult | ✅ Can do | ✅ Confident |

---

## 🎯 Learning Progression

### Current 4-Lab Progression

```
Week 1: Descriptives → Week 2: T-Tests → Week 3: ANOVA → Week 4: Regression
        ↓                    ↓                   ↓                ↓
     Can run            Can compare         Can compare      Can predict
   descriptives          2 groups          3+ groups       with variables
```

**Gap:** Students know HOW to run analyses but may not understand:
- R fundamentals
- Data preparation steps
- Statistical foundations
- How to create good visualizations
- How to work independently

### Proposed 12-Week Progression

```
Phase 1: FOUNDATIONS (Weeks 1-3)
Learn R → Learn data skills → Learn visualization
    ↓
Phase 2: DESCRIPTIVE & EXPLORATORY (Weeks 4-5)
Describe data → Understand distributions and probability
    ↓
Phase 3: INFERENCE (Weeks 6-7)
Hypothesis testing → Compare groups → Test interactions
    ↓
Phase 4: INTEGRATION (Week 8)
Apply all skills in mid-term project
    ↓
Phase 5: PREDICTION (Weeks 9-10)
Model relationships → Predict outcomes → Multiple predictors
    ↓
Phase 6: COMMUNICATION (Week 11)
Create publication figures → Write reproducible reports
    ↓
Phase 7: SYNTHESIS (Week 12)
Independent analysis from start to finish
```

**Result:** Students understand not just HOW but WHY, can work independently, and can learn new techniques

---

## 📈 Assessment Evolution

### Current Assessment (Implied)

```
Weekly exercises (informal)
    ↓
No formal integration
    ↓
Minimal independent application
```

### Proposed Assessment Structure

```
┌─────────────────────────────────────────────────────────────┐
│  FORMATIVE ASSESSMENT (Throughout)                          │
│  • Self-check quizzes (after each part)                    │
│  • WebR interactive practice (immediate feedback)           │
│  • Discussion forum participation                           │
│  • Code review activities                                   │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  WEEKLY EXERCISES (30% of grade)                            │
│  • Best 8 of 10 exercises                                   │
│  • Guided practice with real data                           │
│  • Build skills incrementally                               │
│  • Automated checks where possible                          │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  MID-TERM PROJECT (30% of grade) - Week 8                   │
│  • Analyze provided dataset                                 │
│  • Test group differences                                   │
│  • 3-4 page Quarto report                                   │
│  • Apply Weeks 1-7 skills                                   │
│  Assessment: Code (25%) + Analysis (25%) +                  │
│             Interpretation (25%) + Report (25%)             │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│  CAPSTONE PROJECT (40% of grade) - Week 12                  │
│  • Choose from dataset options OR own data                  │
│  • Complete research cycle                                  │
│  • 6-8 page Quarto report                                   │
│  • All skills integrated                                    │
│  Assessment: Code quality (25%) + Statistical accuracy (25%)│
│             Interpretation (25%) + Communication (25%)      │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎓 Student Journey Comparison

### Current Experience (4 Labs)

```
Weeks 1-2: Setup R, struggle with basics
            ↓
Week 3-4: Lab 1 - "What's dplyr? What's ggplot2?"
            ↓
Week 5-6: Lab 2 - "How do I import my data again?"
            ↓
Week 7-8: Lab 3 - "I can follow the code but couldn't do it alone"
            ↓
Week 9-10: Lab 4 - "I'm lost with regression"
            ↓
End: "I can follow tutorials but not work independently"
```

### Proposed Experience (12 Weeks)

```
Week 1: "RStudio makes sense! I can write R code!"
        ↓
Week 2: "I can import and clean data like a pro"
        ↓
Week 3: "I can make beautiful plots!"
        ↓
Week 4: "I understand distributions and descriptives"
        ↓
Week 5: "I get how sampling and probability work"
        ↓
Week 6: "I understand hypothesis testing now!"
        ↓
Week 7: "ANOVA interactions make sense"
        ↓
Week 8: MID-TERM PROJECT - "I can analyze data independently!"
        ↓
Week 9: "Correlation and regression click"
        ↓
Week 10: "I can build complex models"
        ↓
Week 11: "I can make publication-quality figures and reports"
        ↓
Week 12: CAPSTONE - "I'm a confident R user!"
        ↓
End: "I can design and conduct my own analyses"
```

---

## 📚 Resource Ecosystem Comparison

### Current Resources

```
Labs (4)
    ├── Interactive chapters with WebR
    ├── Embedded slides
    ├── Exercise templates
    └── Follow-on exercises

R Toolbox (8 sections, mostly placeholders)

Boil in the Bag (9 templates)

R Handbook (single page)
```

### Proposed Resources

```
Weeks (12-16)
    ├── Interactive chapters with WebR
    ├── Embedded slides
    ├── Exercise templates
    ├── Follow-on exercises
    └── NEW: Mid-term & Capstone projects

R Toolbox (12 comprehensive sections)
    ├── Setup, Import, Wrangle (EXPANDED)
    ├── Plots, Tests, Models (EXPANDED)
    ├── Reporting, Troubleshooting (EXPANDED)
    └── NEW: Functions, Projects, Git, Packages

Boil in the Bag (15 templates)
    ├── Existing 9 templates
    └── NEW: 6 advanced templates

Examples (NEW)
    ├── Descriptive report
    ├── Experiment report
    ├── Correlational report
    └── Full APA paper

Cheat Sheets (NEW)
    ├── dplyr for psychologists
    ├── ggplot2 for psychologists
    ├── Statistical test decision tree
    ├── APA reporting guide
    └── R basics reference

Videos (NEW)
    ├── RStudio tour
    ├── First R script
    ├── Troubleshooting errors
    ├── Creating Quarto reports
    ├── Git basics
    └── Test-specific walkthroughs

Instructor Materials (NEW)
    ├── Teaching notes (all weeks)
    ├── Rubrics (exercises, projects)
    ├── Solutions (password-protected)
    └── Setup guide
```

---

## 💡 Key Insights

### Why 12 Weeks Instead of 4?

1. **Fills knowledge gaps:** Current version assumes R basics, data wrangling, and ggplot2
2. **Builds foundations:** Statistics needs probability and sampling theory
3. **Enables independence:** More practice and integration time
4. **Professional skills:** Quarto, reproducibility, communication
5. **Realistic pacing:** Less cognitive overload, better retention

### Why Keep It Modular?

1. **Flexible adoption:** Use all 12, or just the new weeks, or 16 weeks
2. **Backwards compatible:** Current 4-lab users not disrupted
3. **Pick and choose:** Instructors can select relevant weeks
4. **Self-paced friendly:** Students can progress at own speed
5. **Future-proof:** Easy to add/update individual modules

### What Makes This Feasible?

1. **Builds on existing excellence:** Not starting from scratch
2. **Reuses pedagogical approach:** Same three-stage learning
3. **Open-source tools:** No licensing costs
4. **Modular development:** Can build incrementally
5. **Community contribution:** Others can help improve

---

## 🎯 Bottom Line

### Current: Good Introduction
- Gets students started with R
- Covers essential statistical tests
- Assumes a lot of prior knowledge
- Limited independent application

### Proposed: Comprehensive Training
- ✅ No assumptions (starts from scratch)
- ✅ Full research workflow (import → report)
- ✅ Strong foundations (R, data, viz, stats)
- ✅ Independent capability (projects, troubleshooting)
- ✅ Professional skills (Quarto, reproducibility)
- ✅ Transfer ready (can learn new techniques)

### The Transformation

```
FROM: "I can follow R tutorials"
  TO: "I can design and conduct analyses independently"

FROM: "I know some statistical tests"
  TO: "I understand statistics and can choose appropriate tests"

FROM: "I can copy-paste code"
  TO: "I can write and debug R code"

FROM: "I need help with everything"
  TO: "I can troubleshoot and learn on my own"
```

---

**This visual comparison shows WHY the expansion is valuable and HOW it builds on existing strengths.**

For implementation details, see:
- [QUICK_START_GUIDE.md](QUICK_START_GUIDE.md) - How to start
- [EXPANSION_SUMMARY.md](EXPANSION_SUMMARY.md) - Executive overview
- [EXPANSION_PLAN.md](EXPANSION_PLAN.md) - Complete details
