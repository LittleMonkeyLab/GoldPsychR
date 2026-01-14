# Five-Component R Teaching Workflow

## Overview

A pedagogical system for teaching introductory R in research methods labs. Each component reinforces the same worked examples, cycled through section-by-section rather than completed linearly.

---

## Component 1: Instructor Demo Slides

**Format:** Quarto revealjs presentation

**Purpose:** Live demonstration of key "moves" with deliberate errors fixed in real time.

### Features
- Code annotations (Quarto hover annotations) explain every line
- Deliberate errors shown and debugged live to normalise mistakes
- Speaker notes flag common misconceptions
- Progressive complexity from basic operations to grouped summaries

### The Seven Moves

| Move | Content | Key Skill |
|------|---------|-----------|
| 1 | RStudio Tour | Console, Environment, assignment |
| 2 | Vectors & Functions | `c()`, `mean()`, `sd()` |
| 3 | Loading Data | `read_csv()`, `head()`, `str()` |
| 4 | Reverse Scoring | Formula: `(max + min) - item` |
| 5 | Descriptive Statistics | `group_by()`, `summarise()` |
| 6 | Visualisation | `ggplot2` boxplots |
| 7 | APA Write-Up | Reporting M, SD, n |

### Slide Structure
- Section title slides use `#` (centered, coloured background)
- Content slides use `##`
- Each code block has hover annotations
- Error slides show mistake → fix pattern
- Speaker notes in `::: {.notes}` blocks

---

## Component 2: WebR Practice Chapter

**Format:** Quarto HTML document with `webr` filter

**Purpose:** Independent browser-based practice with self-assessment questions.

### Features
- Executable code cells (no R installation required)
- Self-assessment using webexercises (`mcq()`, `fitb()`, `torf()`)
- Progressive scaffolding: early cells complete, later cells have blanks
- Immediate feedback without grading pressure

### Pedagogical Pattern (repeat for each section)

1. **Explanation** — Brief context for the skill
2. **Demonstration** — Read-only code showing the pattern (`#| read-only: true`)
3. **Practice** — Editable code with `___` blanks to complete
4. **Self-check** — MCQ or fill-in-the-blank question

### Technical Requirements
- YAML filter: `filters: [webr]`
- webexercises JS/CSS in header
- Setup chunk with `#| context: setup` for simulated data
- Packages specified in YAML: `webr: packages: ['dplyr', 'ggplot2']`

---

## Component 3: Scaffolded Student Template

**Format:** Quarto HTML document (rendered locally in RStudio)

**Purpose:** Consolidation and submission; students complete exercises and render clean output.

### Features
- Fully annotated code with `#| code-annotations: below`
- Exercise prompts in callout boxes
- Submission checklist at the end
- Session info for reproducibility

### Scaffolding Levels by Section

| Section | Scaffolding | Student Task |
|---------|-------------|--------------|
| Load Data | Complete | Run and observe |
| Reverse Score | Complete with annotations | Understand each step |
| Descriptives | Complete | Fill in interpretation |
| Visualisation | Partial (one plot provided) | Create custom plot |
| APA Write-Up | Template paragraph only | Write full paragraph with statistics |
| Reflection | Blank | Answer open-ended questions |

### Structure
- YAML with `code-annotations: below`
- Each section has: explanation → code chunk → exercise callout
- Exercises numbered (1.1, 2.1, etc.) for easy reference
- Final checklist uses task list format: `- [ ] Item`

---

## Component 4: Follow-On Exercise

**Format:** Quarto HTML document (like template, but less scaffolded)

**Purpose:** Transfer learning with a different dataset to confirm skill generalisation.

### Features
- **Different dataset** (e.g., wellbeing study instead of personality)
- **Different scale** (e.g., 1–7 instead of 1–5, requiring adapted reverse-scoring formula)
- Reduced scaffolding — more blanks, fewer complete examples
- Collapsible solutions for self-checking (`::: {.callout-caution collapse="true"}`)

### Key Differences from Main Template

| Aspect | Main Template | Follow-On |
|--------|---------------|-----------|
| Dataset | Primary teaching dataset | New dataset, same structure |
| Scale | e.g., 1–5 | e.g., 1–7 |
| Code provided | ~80% complete | ~40% complete |
| Solutions | None | Hidden, expandable |
| Submission | Required | Optional |

### Purpose
Tests whether students can adapt skills to new context—if they can only analyse the original dataset, they haven't truly learned.

---

## Component 5: R Handbook

**Format:** Quarto HTML document (reference, not instructional)

**Purpose:** Persistent searchable reference organised by skill area.

### Features
- All code chunks set to `#| eval: false` (display only)
- Searchable with browser find
- Dark mode support (theme toggle)
- Copy-paste friendly examples
- Common errors section with fixes

### Sections

1. **R Basics** — Assignment, data types, vectors, operations
2. **Working with Data** — Loading CSVs, inspecting, accessing columns
3. **Data Wrangling** — dplyr verbs (select, filter, mutate, group_by, summarise, arrange)
4. **Descriptive Statistics** — Central tendency, variability, grouped summaries
5. **Questionnaire Scoring** — Reverse scoring formulas, scale score creation
6. **Visualisation** — ggplot2 templates (histogram, boxplot, bar chart, scatterplot)
7. **Common Errors** — Object not found, function not found, NA results, closure errors
8. **Useful Patterns** — Complete workflow template, APA reporting format
9. **Keyboard Shortcuts** — RStudio shortcuts table

### Style
- Minimal prose, maximum code examples
- Each pattern shows the general form, then a concrete example
- Error section shows error message → cause → fix

---

## Cycling Structure (Recommended)

Rather than completing all of one component before starting the next, cycle through each section:

```
Slides Move 1 → WebR Section 1 → Template Section 1
Slides Move 2 → WebR Section 2 → Template Section 2
...and so on
```

### Rationale
- Immediate reinforcement while concept is fresh
- Shorter feedback loops
- Reduces cognitive load vs. watching 40 mins of slides then trying to recall details

### Timing Example (2-hour lab)

| Time | Activity |
|------|----------|
| 0:00 | Slides: Intro + RStudio tour |
| 0:10 | WebR: Basics practice |
| 0:20 | Slides: Load & inspect data |
| 0:30 | WebR + Template: Data loading |
| 0:45 | Slides: Reverse scoring |
| 0:55 | WebR + Template: Scoring practice |
| 1:10 | Slides: Descriptives + visualisation |
| 1:25 | WebR + Template: Analysis practice |
| 1:45 | Template: APA write-up |
| 1:55 | Wrap-up |

---

## Technical Stack

### Required
- Quarto (latest)
- quarto-webr extension: `quarto add coatless/quarto-webr`
- R packages: readr, dplyr, ggplot2
- webexercises R package (for self-assessment questions)

### YAML Patterns

**Slides:**
```yaml
format:
  revealjs:
    code-annotations: hover
    slide-number: true
```

**WebR Chapter:**
```yaml
filters:
  - webr
webr:
  packages: ['dplyr', 'ggplot2']
include-in-header:
  - text: |
      <script src="https://debruine.github.io/webexercises/webexercises.js"></script>
      <link rel="stylesheet" href="https://debruine.github.io/webexercises/webexercises.css" />
```

**Template/Follow-on:**
```yaml
format:
  html:
    code-annotations: below
    code-fold: false
```

**Handbook:**
```yaml
format:
  html:
    toc: true
    toc-depth: 3
    code-tools: true
```

---

## Parallel Section Structure

All components should have parallel sections so cycling is seamless:

| Slides Move | WebR Section | Template Section |
|-------------|--------------|------------------|
| Move 1: RStudio Tour | Section 1: Getting Started | Section 1: Load Data |
| Move 2: Vectors | Section 1 (continued) | — |
| Move 3: Loading Data | Section 2: Loading Data | Section 1: Load Data |
| Move 4: Reverse Scoring | Section 3: Reverse Scoring | Section 2: Reverse Scoring |
| Move 5: Descriptives | Section 4: Descriptives | Section 3: Descriptives |
| Move 6: Visualisation | Section 5: Visualisation | Section 4: Visualisation |
| Move 7: APA Write-Up | Section 6: Write-Up | Section 5: APA Write-Up |

---

## Design Principles

1. **Same worked example throughout** — Consistency reduces cognitive load
2. **Code annotations on every block** — Students read code AND explanation together
3. **Deliberate errors normalised** — Show mistakes, then fixes; errors are information
4. **Immediate practice** — Cycle through formats rather than linear completion
5. **Transfer tested** — Follow-on uses different data to confirm generalisation
6. **Persistent reference** — Handbook available throughout course, not just this lab
7. **Browser-first practice** — WebR removes installation barriers for initial learning
8. **Ownership through rendering** — Students produce clean HTML output they can keep
