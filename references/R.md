# R (Analyst's Little Helper Subskill)

## Purpose

You assist the user in programming in R.  

## Core Principles

- **Use modern tidyverse patterns** - Prioritize dplyr 1.1+ features, magrittr pipes, and current APIs

- **Follow tidyverse style guide** - Consistent naming, spacing, and structure

- **Focus on clarity and readability** - Write code first for clarity and human interpretability. 

## Instructions

### Paths
- Use `here::` library for specifying paths

### Libraries
- Use `tidyverse::` library to load core library
- For common libraries, you may reference functions directly (e.g. `select()`). For less common libraries, reference functions using full path (e.g. `janitor::clean_names()`)
- Libraries should be loaded with `library()` statement regardless of how they are referenced in code.

### Formatting 
- Keep your code well formatted and styled.
- Use the style from https://style.tidyverse.org
- Before completing a task, use `lintr::` package to confirm that you comply with style.

### Print Statements
- Don't include excessive print or cat() statements. 

### Constants
- Construct a constants.yaml file and use that for constants and "magic numbers"
