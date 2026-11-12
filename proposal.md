What’s Behind the Grade?
================
P8105 Final Project Group

### Group Members

Xinying Zou (xz3593) · Chen Li (cl4946) · Rachel Liu (rl3721) · Fan Bu
(fb2731) · Yihui Luo (yl6378)

### Motivation

NYC restaurant letter grades offer diners a quick summary of inspection
outcomes, but they do not show which violations were recorded. Even
restaurants with the same grade can differ in inspection scores and
critical violations. We will examine how critical violations vary across
NYC neighborhoods and what diners can learn by comparing restaurants
within the same grade.

### Research Questions

1.  How does the proportion of restaurants with at least one critical
    violation differ across neighborhoods and boroughs?
2.  How do inspection scores and critical violations differ among
    restaurants with the same letter grade?
3.  Which types of critical violations are most common, and do their
    patterns vary by location?

### Intended Final Products

We will create a project website with an interactive map of inspection
outcomes and a side-by-side tool for comparing two restaurants’ grades,
scores, and cited violations. The website will also feature a
reproducible report, supporting visualizations, and a two-minute
narrated screencast.

### Anticipated Data Source

We will use the public [NYC DOHMH Restaurant Inspection
Results](https://data.cityofnewyork.us/d/43nn-pn8j) dataset, which
includes restaurant identifiers, inspection dates, grades, scores,
violation descriptions, critical-violation flags, and location
information.

### Planned Analyses and Visualizations

- **Data preparation and EDA:** Combine violation-level rows into
  inspection-level records; select each restaurant’s most recent
  eligible graded inspection; summarize grade, score, and
  critical-violation distributions.
- **Geographic patterns:** Use `leaflet` to map restaurants and display
  neighborhood-level percentages of restaurants with critical
  violations, alongside restaurant counts. We will use borough-level
  summaries if neighborhood samples are too small.
- **Within-grade comparisons:** Use `ggplot2` or `plotly` to compare
  scores and critical-violation patterns among restaurants with the same
  grade.
- **Violation types and restaurant comparison:** Summarize common
  critical violations by area and allow users to compare two
  restaurants’ inspection records side by side.

### Coding Challenges

\<\<\<\<\<\<\< HEAD Key coding challenges include converting inspection
dates from text to date format, excluding placeholder dates such as
01/01/1900, and consolidating multiple violation records into one record
per inspection without double-counting scores. We will distinguish
inspection types and define a consistent rule for selecting each
restaurant’s most recent eligible graded inspection. We will also
distinguish inspections explicitly reporting no violations from records
with missing information. For mapping, we will validate coordinates,
document exclusions due to missing locations, and create an interactive
map with filters for borough, cuisine, and grade. Large data files will
be kept outside GitHub, with reproducible download and cleaning
instructions provided.

### Planned Timeline

- **November 13–20:** Adding the data to GitHub repository, meet with
  the teaching team and check the feasibility of our plan, confirm the
  challenge part and divide the work.
- **November 21–27:** Consolidate inspection records, and conduct
  preliminary exploratory analyses.
- **November 28–December 4:** Complete geographic and within-grade
  analyses, develop the interactive map and restaurant comparison tool.
- **December 5–9:** Integrate visualizations, complete the written
  report, and finalize the project website.
- **December 10–12:** Test interactive features, review reproducibility,
  record the screencast, and submit

We will avoid double-counting violations from the same inspection,
distinguish restaurants using unique IDs, handle missing grades and
locations, and check whether neighborhood boundaries can be matched
reliably. Building a responsive interactive map and restaurant
comparison tool will be an additional challenge. We will document
exclusions and maintain a reproducible data-cleaning workflow.

### Planned Timeline

- **Nov 13–20:** Finalize scope, meet with the teaching team, and assess
  data quality.
- **Nov 21–27:** Clean and consolidate inspection records; complete
  initial EDA.
- **Nov 28–Dec 4:** Build visualizations, the map, and the restaurant
  comparison tool.
- **Dec 5–9:** Draft the report and integrate the project website.
- **Dec 10–12:** Test features, check reproducibility, record the
  screencast, and submit.
