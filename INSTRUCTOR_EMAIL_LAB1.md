# Email: Lab 1 Resources for Instructors

**To:** Stacey, Maria, Pete  
**Subject:** Lab 1 Resources - Grit Scale Descriptive Statistics

---

Hi Stacey, Maria, and Pete,

I've prepared all the materials for **Lab 1: Descriptive Statistics** (Grit Scale). Here's everything you need to know about the resources and how to use them.

## 🎯 What We're Teaching

**Topic:** Descriptive Statistics using the Short Grit Scale (8 items)  
**Dataset:** 120 university students (First Year vs Final Year)  
**Skills:** Loading data, reverse-scoring, calculating subscales, descriptive stats, boxplots, APA write-up

## 📚 The 3-Step Workflow (Every Part)

Each of the 5 parts follows the same structure:

1. **Watch** - You demonstrate using embedded slides
2. **Try** - Students practice with interactive code in their browser (WebR)
3. **Do** - Students complete exercises in their downloaded notebook (RStudio Server)

**Important:** Students download ONE notebook in Part 1, then use it for all 5 parts.

## 🗂️ Resource Structure

### Main Entry Point
**`labs/lab01.qmd`** - This is the main landing page students will see. It includes:
- Overview and data story
- Quick navigation links to all 5 parts
- Download buttons for the exercise notebook and follow-on
- Schedule and key concepts

### Integrated Lab Experience (Primary Resource)
**`chapters/lab1/index.qmd`** - This is where students should start. It links to all 5 parts.

**Each Part Has:**
- **Slides** (`part1-slides.qmd`, `part2-slides.qmd`, etc.) - Embedded RevealJS slides for you to present
- **Practice Page** (`part1.qmd`, `part2.qmd`, etc.) - WebR interactive practice for students
- **Notebook Sections** - Students work in ONE downloadable notebook (`templates/lab1-exercise.qmd`)

### The 5 Parts

| Part | Focus | Key Activities |
|------|-------|----------------|
| **Part 1** | RStudio Tour | Variables, vectors, functions, **download notebook**, change name, render |
| **Part 2** | Loading Data | `read_csv()`, `head()`, `str()`, `dim()` |
| **Part 3** | Reverse Scoring | Formula: `6 - original` (items G1, G3, G5, G6) |
| **Part 4** | Descriptives & Plots | `group_by()`, `summarise()`, `ggplot()` boxplots |
| **Part 5** | APA Write-Up | Reporting M, SD, n, proactive coding |

## 🎓 How to Run the Lab

### Before the Lab
1. **Open the main page:** `labs/lab01.qmd` (or direct students to the integrated experience at `chapters/lab1/index.qmd`)
2. **Familiarize yourself with Part 1 slides** - especially the "Change Your Name and Render" section (this is their first success!)
3. **Test RStudio Server access:** `https://psy909.gold.ac.uk/rstudioserver/`

### During the Lab (2 hours: 13:00-15:00)

**Part 1 (13:00-13:20):**
- Present slides embedded in `part1.qmd`
- Students practice with WebR code cells on the same page
- **Critical:** Guide students to download the notebook and set it up in RStudio Server
- Their first task: Change "YOUR NAME HERE" to their actual name and **Render** (this confirms everything works!)

**Parts 2-5:**
- Same pattern: Slides → WebR practice → Notebook exercises
- Students continue working in the SAME notebook they downloaded in Part 1
- Each part has embedded slides you can present directly from the page

### Key Technical Details

**RStudio Server:**
- URL: `https://psy909.gold.ac.uk/rstudioserver/`
- Login format: `username@campus.goldsmiths.ac.uk` (full email)
- Students create a folder, upload the `.qmd` file, and work there

**WebR (Browser Practice):**
- Students can edit and run code directly in the browser
- No RStudio needed for practice sections
- Great for experimentation before moving to RStudio Server

**The Notebook:**
- Location: `templates/lab1-exercise.qmd`
- Students download it once in Part 1
- It renders successfully if untouched (good for testing)
- Code is hidden by default in rendered HTML (`code-fold: true`)
- Students fill in code sections marked with `# YOUR CODE:`

## 📋 Schedule Breakdown

| Time | Activity | What Happens |
|------|----------|--------------|
| 13:00-13:10 | Part 1 Slides | You present RStudio basics |
| 13:10-13:20 | Part 1 Practice | Students try WebR, download notebook, set up RStudio Server, change name, render |
| 13:20-13:35 | Part 2 Slides | Data loading concepts |
| 13:35-13:50 | Part 2 Practice | Students practice loading data (WebR + notebook) |
| 13:50-14:05 | Part 3 Slides | Reverse scoring explanation |
| 14:05-14:20 | Part 3 Practice | Students practice reverse scoring |
| 14:20-14:40 | Part 4 Slides | Descriptives and visualisation |
| 14:40-14:55 | Part 4 Practice | Students create plots and analyze |
| 14:55-15:00 | Wrap-up | Part 5 (APA write-up) can be completed independently |

## 🎬 Alternative Resources (If Needed)

If students want to access components separately:

- **Full Slides:** `slides/lab1-slides.qmd` (standalone slide deck)
- **WebR Practice Only:** `chapters/lab1-webr.qmd` (all interactive practice in one page)
- **Follow-On Exercise:** `followon/lab1-followon.qmd` (optional extra practice)

## ⚠️ Common Issues to Watch For

1. **RStudio Server Login:** Students must use full email format (`@campus.goldsmiths.ac.uk`)
2. **Render Button:** First-time users might not find it - it's in the top toolbar (knitting needle icon)
3. **Notebook Download:** Make sure students download in Part 1, not later
4. **Code Visibility:** Remind students that code is hidden in rendered HTML - that's intentional!
5. **WebR vs RStudio:** WebR is for practice, RStudio Server is for their actual work/submission

## 📖 Additional Context

**The Grit Scale:**
- Short Grit Scale (Grit-S) - 8 items
- Two subscales: Consistency of Interest (G1, G3, G5, G6 - reverse-scored) and Perseverance of Effort (G2, G4, G7, G8)
- Source article link is included in materials for interested students

**Data:**
- Hosted on GitHub: `https://raw.githubusercontent.com/LittleMonkeyLab/datarepo/main/Y1_Week13_Lab1_grit_data.csv`
- Loads automatically when students run the first code chunk

## 🆘 Support Resources

- **R Toolbox:** `toolbox/index.qmd` - Code examples and reference
- **Troubleshooting:** `toolbox/troubleshooting.qmd` - Common errors and fixes
- **Module Structure Guide:** `MODULE_STRUCTURE.md` - Full documentation of the lab structure

## ✅ Quick Checklist for Instructors

- [ ] Test RStudio Server access before lab
- [ ] Open `chapters/lab1/index.qmd` or `labs/lab01.qmd` 
- [ ] Navigate through Part 1 slides to familiarize yourself
- [ ] Test the download button for the notebook
- [ ] Be ready to help with RStudio Server setup (login, folder creation, upload)
- [ ] Emphasize the "Change Name and Render" task as their first success
- [ ] Remind students they use ONE notebook for all 5 parts

## 📧 Questions?

If anything is unclear or you'd like to discuss the materials, just let me know. The website should render everything automatically - just open the `.qmd` files or view the rendered HTML in the `docs/` folder.

Thanks, and good luck with the lab!

---

**P.S.** All materials are designed to work together seamlessly. Students should primarily use the integrated experience (`chapters/lab1/index.qmd`), but alternative resources are available if needed. The 3-step cycle (Watch → Try → Do) repeats for each part, so once students understand it in Part 1, they'll know what to expect.
