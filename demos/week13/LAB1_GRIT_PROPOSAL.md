# Lab 1 Dataset: Short Grit Scale (Grit-S)

## Scale Information
**Citation**: Duckworth, A. L., & Quinn, P. D. (2009). Short Grit Scale (Grit-S) [Database record]. APA PsycTests. https://doi.org/10.1037/t01598-000

**Original Paper**: Duckworth, A. L., & Quinn, P. D. (2009). Development and validation of the Short Grit Scale (Grit-S). *Journal of Personality Assessment*, 91, 166-174.

## Scale Structure

### Total Items: 8
### Response Scale: 5-point Likert 
- 1 = Not like me at all
- 2 = Not much like me  
- 3 = Somewhat like me
- 4 = Mostly like me
- 5 = Very much like me

### Two Subscales:

**1. Consistency of Interest (4 items)**
- Measures ability to maintain interest in long-term goals
- Items: G1, G3, G5, G6
- **All 4 items are REVERSE-SCORED**

**2. Perseverance of Effort (4 items)**  
- Measures ability to work hard despite setbacks
- Items: G2, G4, G7, G8
- **All 4 items are FORWARD-SCORED**

### Reverse-Scoring:
Items G1, G3, G5, G6 need to be reverse-scored: 1→5, 2→4, 3→3, 4→2, 5→1

## The 8 Items

**G1**: "New ideas and projects sometimes distract me from previous ones." *(reverse-scored)*

**G2**: "Setbacks don't discourage me." *(forward-scored)*

**G3**: "I have been obsessed with a certain idea or project for a short time but later lost interest." *(reverse-scored)*

**G4**: "I am a hard worker." *(forward-scored)*

**G5**: "I often set a goal but later choose to pursue a different one." *(reverse-scored)*

**G6**: "I have difficulty maintaining my focus on projects that take more than a few months to complete." *(reverse-scored)*

**G7**: "I finish whatever I begin." *(forward-scored)*

**G8**: "I am diligent." *(forward-scored)*

## Dataset Structure

### Sample: 120 university students

### Variables:

**ID**: Participant identifier (1-120)

**Age**: Participant age (18-25)

**Gender**: 
- 1 = Female
- 2 = Male  
- 3 = Non-binary/Other

**Study_Year**: Grouping variable for comparisons
- 1 = First Year
- 2 = Final Year

**G1-G8**: The 8 Grit Scale items (raw scores, 1-5)

## Scoring

1. **Reverse-score items G1, G3, G5, G6**
2. **Calculate Consistency of Interest**: Mean of G1, G3, G5, G6 (after reverse-scoring)
3. **Calculate Perseverance of Effort**: Mean of G2, G4, G7, G8
4. **Calculate Total Grit**: Mean of all 8 items (after reverse-scoring G1, G3, G5, G6)

## Expected Patterns

- **Consistency of Interest**: Final-year students might show slightly higher scores (better consistency)
- **Perseverance of Effort**: Final-year students might show slightly higher scores
- **Total Grit**: Final-year students might show slightly higher overall grit
- **Gender differences**: May show small differences (men sometimes slightly higher)

## Analysis Tasks for Lab 1

1. **Load CSV data** into R
2. **Reverse-score items** G1, G3, G5, G6
3. **Calculate subscale scores**:
   - Consistency of Interest = mean of G1, G3, G5, G6 (after reverse-scoring)
   - Perseverance of Effort = mean of G2, G4, G7, G8
4. **Calculate total Grit score** = mean of all 8 items (after reverse-scoring)
5. **Descriptive statistics** by Study_Year (mean, SD, min, max)
6. **Create boxplots** using ggplot2 comparing First Year vs Final Year for:
   - Consistency of Interest
   - Perseverance of Effort  
   - Total Grit
7. **Write APA-style results paragraph** describing the findings

## Why This Works for Lab 1

✅ **Real, validated scale** - Widely used in psychology research
✅ **Perfect length** - 8 items (not too short, not too long)
✅ **Clear reverse-scoring** - 4 items need reverse-scoring (good practice)
✅ **Two subscales** - Allows multiple analyses
✅ **Interesting topic** - Grit is relevant and engaging for students
✅ **Group comparisons** - Study_Year provides clear comparison groups
✅ **Demographics included** - Age and Gender (including non-binary option)
