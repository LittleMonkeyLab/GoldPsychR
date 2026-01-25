# Week 13 / Lab 1 Dataset Proposal: Big Five Personality

## Learning Objectives
- Navigate RStudio and understand its four panes
- Load CSV data into R
- Reverse-score negatively worded questionnaire items
- Calculate descriptive statistics by group
- Create boxplots using ggplot2
- Write an APA-style results paragraph

## Dataset: Big Five Personality Inventory

### Research Context
The Big Five personality model (Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism) is one of the most widely used frameworks in personality psychology. Many questionnaires include reverse-scored items to reduce response bias.

### Dataset Structure

**Sample**: 120 university students (60 per group)

**Grouping Variable**: 
- **Study_Year**: 1 = First Year, 2 = Final Year
- (Allows comparison: Do personality traits differ between first-year and final-year students?)

**Big Five Domains** (each measured with 4 items, 2 forward-scored, 2 reverse-scored):

1. **Openness** (O)
   - O1: "I have a vivid imagination" (forward)
   - O2: "I am not interested in abstract ideas" (reverse)
   - O3: "I have excellent ideas" (forward)
   - O4: "I do not have a good imagination" (reverse)

2. **Conscientiousness** (C)
   - C1: "I am always prepared" (forward)
   - C2: "I leave my belongings around" (reverse)
   - C3: "I pay attention to details" (forward)
   - C4: "I make a mess of things" (reverse)

3. **Extraversion** (E)
   - E1: "I am the life of the party" (forward)
   - E2: "I don't talk a lot" (reverse)
   - E3: "I feel comfortable around people" (forward)
   - E4: "I keep in the background" (reverse)

4. **Agreeableness** (A)
   - A1: "I am interested in people" (forward)
   - A2: "I feel little concern for others" (reverse)
   - A3: "I have a soft heart" (forward)
   - A4: "I am not really interested in others" (reverse)

5. **Neuroticism** (N)
   - N1: "I get stressed out easily" (forward)
   - N2: "I am relaxed most of the time" (reverse)
   - N3: "I worry about things" (forward)
   - N4: "I seldom feel blue" (reverse)

**Response Scale**: 1-5 Likert scale
- 1 = Disagree strongly
- 2 = Disagree
- 3 = Neutral
- 4 = Agree
- 5 = Agree strongly

### Variables in Dataset

**ID**: Participant identifier (1-120)

**Study_Year**: 
- 1 = First Year
- 2 = Final Year

**O1, O2, O3, O4**: Openness items
**C1, C2, C3, C4**: Conscientiousness items
**E1, E2, E3, E4**: Extraversion items
**A1, A2, A3, A4**: Agreeableness items
**N1, N2, N3, N4**: Neuroticism items

**Age**: Participant age (18-22)

**Gender**: 
- 1 = Female
- 2 = Male
- 3 = Non-binary/Other

### Expected Patterns

- **Reverse-scored items** need recoding: 1→5, 2→4, 3→3, 4→2, 5→1
- **Domain scores**: Sum of 4 items per domain (after reverse-scoring)
- **Group differences**: Final-year students might show higher Conscientiousness (maturity effect)
- **Variability**: Good spread of scores for teaching purposes

## Analysis Tasks

1. **Load data**: Import CSV file
2. **Reverse-score items**: Recode O2, O4, C2, C4, E2, E4, A2, A4, N2, N4
3. **Calculate domain scores**: Sum items for each Big Five domain
4. **Descriptive statistics**: Mean, SD, min, max by Study_Year
5. **Visualization**: Boxplots comparing First Year vs Final Year for each domain
6. **APA results**: Write paragraph describing findings

## Why This Works

✅ **Pedagogically perfect**: 
   - Clear reverse-scoring task (10 items)
   - Multiple groups to compare
   - Five domains = multiple analyses
   - Real psychological measure

✅ **Appropriate complexity**: 
   - Not too simple (20 items total)
   - Not too complex (manageable for Lab 1)
   - Clear structure

✅ **Realistic**: 
   - Based on actual Big Five measures
   - Common research question (year differences)
   - Uses standard scales

✅ **Visualization-friendly**: 
   - Boxplots show group differences well
   - Five domains = five plots (good practice)
   - Clear patterns to interpret

## Alternative Grouping Variables

If Study_Year doesn't work, alternatives:
- **Gender** (though this might be sensitive)
- **Course_Type**: Psychology vs Other subjects
- **Living_Situation**: On-campus vs Off-campus
- **Employment**: Part-time job vs No job

Study_Year is probably best as it's neutral and has a plausible hypothesis (maturity/development effects).
