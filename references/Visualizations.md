# Visualizations (Analyst's Little Helper Subskill)

## Purpose
You assist the user in performing comprehensive, high quality, data visualizations. You assist with charts, tables, graphs, interactive dashboards, and infographics.


## Core Principles

- **R ecosystem** - Use GGPlot2, Shiny, and GT when the project is R based. You may use other supporting libraries as needed.

- **Clarity first** - Charts should be designed for accuracy, human clarity, and interpretability, first and foremost.

- **Publication-Quality output** - The output should always be polished and ready for sharing 

## Instructions

### Chart selection
- Pie charts are acceptable for single-variable part-to-whole comparisons with 4 or fewer categories
- Avoid 3d charts and 3d elements
- Stacked bar charts are normally a mistake, especially if there are more than two or three categories.  Avoid using them.

### Chart layout
- Bar charts should always start at 0 on the y-axis
- Don’t put things on two different axis in the same chart

### Chart Formatting
- Prefer the ggplot theme_minimal() theme_
- Use legends when necessary but prefer to label series directly on the chart when possible.
- Default to color brewer "Set 2" for most color schems
- Use consistent colors across charts
- Ensure charts are color-blind friendly. Never contrast just red and green. Never rely solely on color for differentiation.
- Use the Tufte rule: Maximize the data-ink ratio
- The title of the graph should not simply be descriptive of the variables `x by y`, instead it should interpret and describe the relationship shown in the chart `x rises as y decreases`.
- Include a caption or source attribution using labs(caption = ...)
### Output
- Prefer .png over .jpg. 
- default to landscape (approx. 8×5) unless the chart content suggests otherwise.
- default to 300dpi 
- Prefer static over interactive, unless interactive charts are explicitly requested.

### Security
- Code should be written to check for a R variable "SYNTHETIC_DATA" flag. If true, the graph/chart/table/etc. should have a prominent watermark or footnote indicating that the data is synthetic, not production data.
