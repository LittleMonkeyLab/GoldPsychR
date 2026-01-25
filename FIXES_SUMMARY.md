# Fixes Applied & Advice

## ✅ Fixed Issues

### 1. Lab Overview - Week 1 Link
**Fixed:** `labs/index.qmd` - Changed "Lab Overview" to a live link: `[Lab Overview](lab01.qmd)`

### 2. Part 1 Slides - Removed Weeks 2-4 & Made Grit Scale Callout Minimal
**Fixed:** `chapters/lab1/part1-slides.qmd`
- Removed the "4 weeks" overview section with weeks 2-4
- Changed the Grit Scale callout from a full callout box to a simple italicized link:
  - Old: Full callout-note with icon and header
  - New: `*[Learn more about the Grit Scale](url)*`

### 3. Part 5 - Fixed knitr Errors
**Fixed:** `chapters/lab1/part5.qmd`
- Removed `knitr::opts_chunk$set(echo = FALSE)` - not needed in WebR/Quarto
- Replaced `knitr::kable()` with simple `summary_stats` display (kable not available in WebR)

---

## 💡 Advice (Not Implemented)

### Part 2 - curl Package Warning

**The Error:**
```
`curl` package not installed, falling back to using `url()`
```

**Why it happens:**
- `read.csv()` in R tries to use the `curl` package first for HTTPS URLs
- If `curl` isn't available, it falls back to base R's `url()` function
- This is just a warning, not an error - the code still works

**Options to fix:**

1. **Suppress the warning** (easiest):
   ```r
   options(warn = -1)  # Suppress warnings temporarily
   data <- read.csv(data_url, stringsAsFactors = FALSE)
   options(warn = 0)   # Restore warnings
   ```

2. **Use `url()` explicitly** (more explicit):
   ```r
   con <- url(data_url)
   data <- read.csv(con, stringsAsFactors = FALSE)
   close(con)
   ```

3. **Add curl to webr packages** (if WebR supports it):
   ```yaml
   webr:
     packages: ['curl']
   ```
   However, WebR may not support `curl` package, so this might not work.

4. **Use `readr::read_csv()` instead** (if WebR supports it):
   ```r
   library(readr)
   data <- read_csv(data_url, show_col_types = FALSE)
   ```
   But you mentioned you switched to `read.csv()` for WebR compatibility, so this might not work either.

5. **Best approach for WebR slides**: Accept the warning as harmless. It's informational, not an error. The data still loads correctly. You could add a note in the slides explaining that this warning is normal and can be ignored.

**Recommendation:** Option 5 - just accept it as a harmless warning. If you want to suppress it, use Option 1 with `suppressWarnings()`:
```r
data <- suppressWarnings(read.csv(data_url, stringsAsFactors = FALSE))
```

---

## 📐 Iframe Differences

### Part 4 vs Parts 1-3

**Part 4** uses a simple fixed-height iframe:
```html
<iframe src="part4-slides.html" width="100%" height="500px" style="border: 1px solid #ccc; border-radius: 8px;"></iframe>
```

**Parts 1-3** use a responsive wrapper:
```html
<div style="position: relative; padding-top: 56.25%; height: 0; overflow: hidden; border: 1px solid #ccc; border-radius: 8px;">
  <iframe src="part1-slides.html" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none;" allowfullscreen>
  </iframe>
</div>
```

**Why Part 4 looks better:**
- Fixed height (`500px`) prevents initial sizing issues
- No responsive calculation needed, so it renders immediately at the correct size
- The responsive wrapper (56.25% padding-top = 16:9 aspect ratio) can cause initial narrow sizing before WebR renders

**Recommendation:** Consider updating Parts 1-3 to use the same fixed-height approach as Part 4 for consistency and better initial rendering.

---

## Summary

All requested fixes have been applied. The curl warning is harmless and can be left as-is, or suppressed if desired. The iframe difference explains why Part 4 looks better - consider standardizing on the fixed-height approach.
