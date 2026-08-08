# GoldPsychR Expansion: Quick Start Guide

**Last Updated:** August 8, 2026

---

## 📖 Read This First

You have a well-designed **4-session R course**. This guide helps you extend it to a **12-16 week comprehensive programme**.

### Where to Start

1. **Quick Overview** → Read this page (5 minutes)
2. **Executive Summary** → [EXPANSION_SUMMARY.md](EXPANSION_SUMMARY.md) (10 minutes)
3. **Full Details** → [EXPANSION_PLAN.md](EXPANSION_PLAN.md) (60+ minutes)

---

## 🎯 The Big Picture

### Current: 4 Labs (8 hours total)
```
Lab 1: Descriptives → Lab 2: T-Tests → Lab 3: ANOVA → Lab 4: Regression
```

### Proposed: 12 Weeks (24+ hours + projects)
```
Weeks 1-3: Foundations (NEW)
    ↓
Weeks 4-7: Inference (EXPANDED from Labs 1-3)
    ↓
Week 8: Mid-Term Project (NEW)
    ↓
Weeks 9-10: Regression (EXPANDED from Lab 4)
    ↓
Week 11: Communication (NEW)
    ↓
Week 12: Capstone Project (NEW)
```

**Plus Optional:** Weeks 13-16 for advanced topics

---

## 🆕 What's Being Added?

### 6 New Weeks
1. **Week 1: R Foundations** - RStudio basics, R programming fundamentals
2. **Week 2: Data Wrangling** - tidyverse, dplyr, cleaning data
3. **Week 3: Visualization I** - ggplot2 comprehensive introduction
4. **Week 5: Probability** - Distributions, sampling, confidence intervals
5. **Week 11: Communication** - Publication figures, Quarto reporting
6. **Weeks 8 & 12: Projects** - Integrative assessments

### Enhanced Resources
- ✅ Complete **R Toolbox** (12 sections instead of 8 placeholders)
- ✅ Expand **Boil in the Bag** (15 templates instead of 9)
- ✅ Create **Example Reports** (4 model papers)
- ✅ Design **Cheat Sheets** (5 reference cards)
- ✅ Record **Videos** (6 essential screencasts)
- ✅ Build **Instructor Guide** (teaching notes, rubrics)

---

## 🗓️ Development Timeline

| Phase | Time | What You'll Build |
|-------|------|-------------------|
| **Phase 1** | 3 weeks | Weeks 1-3 (new foundation) + reorganize Week 4 |
| **Phase 2** | 4 weeks | Week 5 (probability) + enhance Weeks 6-7 + Week 8 project |
| **Phase 3** | 3 weeks | Split into Weeks 9-10 + Week 11 + Week 12 + complete Toolbox |
| **Phase 4** | 2 weeks | Optional Weeks 13-16 (advanced topics) |
| **Phase 5** | 2 weeks | Videos, QA, polish |

**Total:** 14-16 weeks of development (200-300 hours)

---

## 💰 Budget Options

### DIY (£0-500)
- Your time embedded in role
- Open-source tools only
- Create videos yourself
- Student pilots from current cohort
- **Viable for full programme**

### Professional (£2,000-5,000)
- Student assistant (£500-1000)
- Video production (£500-1000)
- Graphic design (£500-1000)
- Accessibility audit (£500)

### Premium (£8,000-15,000)
- Development buyout time (£5,000-8,000)
- Full production team
- Multiple pilots with stipends
- External consultants

**Recommendation:** Start DIY, seek funding for polish later

---

## 🎓 Teaching Formats

### 1. Semester Course (Recommended)
- 12 weeks × 2 hours in-person lab
- Weekly exercises (graded)
- Mid-term project (Week 8)
- Final capstone (Week 12)
- **Best for:** Credit-bearing university course

### 2. Extended Programme
- 16 weeks with advanced topics
- **Best for:** MSc students, professional development

### 3. Intensive Workshop
- 5 days, 9am-5pm
- Core content only
- **Best for:** Summer school, bootcamp

### 4. Self-Paced Online
- All materials available
- Flexible timeline
- **Best for:** Open educational resource, MOOCs

---

## ✅ Decision Checklist

Before starting development, decide:

- [ ] **Scope:** 12 weeks or 16 weeks?
- [ ] **Timeline:** When do you want to pilot?
- [ ] **Resources:** How much development time do you have?
- [ ] **Budget:** Any funding available?
- [ ] **Format:** In-person, online, or hybrid?
- [ ] **Assessment:** Graded course or resource library?
- [ ] **Team:** Solo or collaborative development?
- [ ] **Pilot:** Who will test materials?

---

## 🚀 Start Developing (Phase 1)

Once you've made key decisions, begin with **Week 1: R Foundations**:

### Week 1 Components to Create

1. **weeks/week01/index.qmd** - Week overview
2. **weeks/week01/part1.qmd** - RStudio tour (with WebR practice)
3. **weeks/week01/part1-slides.qmd** - Instructor demo slides
4. **weeks/week01/part2.qmd** - R basics (with WebR practice)
5. **weeks/week01/part2-slides.qmd** - R programming slides
6. **templates/week01-exercise.qmd** - RStudio practice workbook
7. **data/week01/** - Practice datasets
8. **toolbox/setup.qmd** - Installation guide (expand from placeholder)

### Content Topics for Week 1

**Part 1: RStudio Tour**
- Interface orientation (4 panes)
- Console vs. Script
- Working directory
- Basic workflow

**Part 2: R Basics**
- Variables and assignment (`<-`)
- Data types (numeric, character, logical, factor)
- Vectors with `c()`
- Basic functions (`mean()`, `sd()`, `length()`)
- Getting help (`?`, `help()`)
- Installing packages

### Time Estimate
- Content writing: 8 hours
- Code examples: 4 hours
- WebR integration: 2 hours
- Testing: 2 hours
- **Total: ~16 hours**

### Then Repeat for Weeks 2-3
- Week 2: Data Wrangling (~20 hours)
- Week 3: Visualization I (~20 hours)

---

## 📊 Success Indicators

### After Phase 1 Pilot
- ✅ Students can navigate RStudio confidently
- ✅ Students can import and wrangle data
- ✅ Students can create basic plots
- ✅ > 80% positive feedback on new weeks
- ✅ Identified issues addressed

### After Full 12-Week Pilot
- ✅ Pre-to-post test improvement > 30%
- ✅ > 80% students complete capstone successfully
- ✅ > 80% report confidence using R independently
- ✅ Materials ready for external adoption

---

## 📚 Module Structure Reference

Each week follows consistent structure:

```
weeks/weekXX/
├── index.qmd           # Week overview with learning objectives
├── part1.qmd           # Interactive page with slides + WebR
├── part1-slides.qmd    # RevealJS slides for Part 1
├── part2.qmd           # Interactive page with slides + WebR
├── part2-slides.qmd    # RevealJS slides for Part 2
└── [... more parts as needed ...]

templates/
└── weekXX-exercise.qmd # Downloadable practice workbook

data/weekXX/
└── *.csv              # Datasets for this week

toolbox/
└── [relevant-topic].qmd # Reference guide
```

---

## 🔗 Related Documents

| Document | Purpose | Time to Read |
|----------|---------|--------------|
| [EXPANSION_SUMMARY.md](EXPANSION_SUMMARY.md) | Executive overview | 10 min |
| [EXPANSION_PLAN.md](EXPANSION_PLAN.md) | Comprehensive detailed plan | 60+ min |
| [Current _quarto.yml](_quarto.yml) | Existing site configuration | 5 min |
| [Current index.qmd](index.qmd) | Current course homepage | 5 min |

---

## 💡 Pro Tips

### 1. Start Small
Don't try to build everything at once. Complete Week 1, pilot it, then move to Week 2.

### 2. Reuse Structure
Copy the pattern from existing labs. Students benefit from consistency.

### 3. Test Early
Have 2-3 students try Week 1 before building Week 2. Catch issues early.

### 4. Version Control
Commit after each major milestone. Makes it easy to revert if needed.

### 5. Document Decisions
Keep notes on why you made certain choices. Helps future you and collaborators.

### 6. Build Community
Share progress on social media. Other R educators can provide feedback and encouragement.

---

## 🤔 Common Questions

### "Isn't 12 weeks too ambitious?"
The current 4 labs are excellent but assume a lot of prior knowledge. The new weeks fill those gaps, making the full programme more accessible.

### "Can I do this solo?"
Yes! The DIY budget assumes solo development. Expect 200-300 hours total (about 15-20 hours/week for 15 weeks).

### "What if I don't have 15 weeks?"
Prioritize Phases 1-3 (12-week core). Skip Phase 4 (extended weeks) and minimize Phase 5 (polish).

### "Do I need to record videos?"
No. Videos enhance the experience but aren't essential. Focus on text/interactive content first.

### "Can others use these materials?"
Yes! Open Educational Resource (OER). Others can adapt, remix, and share with attribution.

### "What if I get stuck?"
- Check the detailed [EXPANSION_PLAN.md](EXPANSION_PLAN.md) (has examples for each week)
- Review existing labs for patterns
- Ask R education community (RStudio Community, Twitter #rstats)
- Look at similar courses (R for Data Science, ModernDive)

---

## 📞 Next Actions

1. **Read** [EXPANSION_SUMMARY.md](EXPANSION_SUMMARY.md) for full context
2. **Decide** on scope (12 or 16 weeks?)
3. **Schedule** development time
4. **Identify** pilot testers
5. **Start** Week 1 development
6. **Share** progress and gather feedback

---

## 🎉 You've Got This!

You've already built a high-quality 4-session course. This plan helps you scale that excellence to a comprehensive programme. 

**Key Mindset:** You're not starting from scratch. You're thoughtfully expanding what already works.

**Remember:** Done is better than perfect. Get Week 1 out there, get feedback, iterate.

---

**Questions or need support?** Document created by Cloud Agent on August 8, 2026.

For implementation support, consult the detailed [EXPANSION_PLAN.md](EXPANSION_PLAN.md).
