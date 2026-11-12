proposal
================

# Violations Across NYC Restaurants

### Group Members

\[Name, UNI\], \[Name, UNI\], \[Chen Li, cl4946\], \[Name, UNI\], \[Name,
UNI\]

### Motivation

Since the semester began, many students in Manhattan, particularly near
Columbia University, have reported gastrointestinal illness after eating
at restaurants along 116th Street, and concerns have also been raised
about campus dining. Letter grades are the main food safety signal
available to diners, but they reveal little about the types or severity
of the violations behind them. Using NYC restaurant inspection data in
R, we examine whether critical food safety violations are common across
Manhattan and other neighborhoods, and whether restaurants with the same
letter grade differ in meaningful ways. Our goal is to give diners a
clearer and more accessible picture of inspection outcomes and to
identify safer options for lunch.

### Research Questions

1.  How does the proportion of restaurants with critical violations
    differ across NYC neighborhoods and boroughs?
2.  How do critical violation patterns and inspection scores vary among
    restaurants receiving the same letter grade?
3.  What are the most frequently reported types of critical violations,
    and how do their distributions vary across geographic areas?

### Intended Final Products

We plan to develop an interactive project website featuring a geographic
visualization of critical violation patterns and a side-by-side
restaurant comparison tool. Users will be able to explore
neighborhood-level differences and compare two restaurants based on
their inspection grades, scores, and recorded violations. The website
will also include exploratory visualizations, a comprehensive
reproducible report, and a two-minute narrated screencast.

### Anticipated Data Sources

We will use the publicly available [NYC Department of Health and Mental
Hygiene Restaurant Inspection
Results](https://data.cityofnewyork.us/d/43nn-pn8j) dataset from NYC
Open Data. The dataset contains restaurant identifiers, geographic
information, inspection dates and types, letter grades, inspection
scores, and violation details, including indicators of critical
violations.

### Planned Analyses and Visualizations

- **Exploratory Data Analysis:** Report how many restaurants have at
  least one critical violation at their most recent graded inspection,
  and examine the distributions of grades, scores, and critical
  violations overall and by borough. We will document how many
  restaurants are excluded for lacking a grade or valid location.
- **Geographic Analysis:** Use leaflet to build an interactive map in
  which each restaurant is a circle marker colored by its inspection
  score or critical violation status, in the same way we colored Airbnb
  listings by review score. We will add a neighborhood layer based on
  the NTA codes in the data, showing the percentage of restaurants with
  at least one critical violation together with restaurant counts.
  Neighborhoods with very few restaurants will be flagged or merged. We
  will examine Manhattan in detail, including the area around 116th
  Street.
- **Within-Grade Comparisons:** Use plotly to create interactive
  boxplots and scatter plots of inspection scores and critical violation
  rates among restaurants with the same letter grade, with hover text
  showing the restaurant name, grade, score, and violation count.
  Summary tables will accompany the plots.
- **Violation Pattern Analysis:** Group violation descriptions into
  broader categories, such as temperature control, vermin, and hygiene
  practices, and compare their frequencies across boroughs and
  neighborhoods using interactive bar charts.
- **Interactive Comparison:** Allow users to select two restaurants and
  view their most recent inspection date, grade, score, and cited
  violations side by side. This tool will also help identify safer lunch
  options in areas of interest.

### Coding Challenges

Key coding challenges include converting inspection dates from text to
date format, excluding placeholder dates such as 01/01/1900, and
consolidating multiple violation records into one record per inspection
without double-counting scores. We will distinguish inspection types and
define a consistent rule for selecting each restaurant’s most recent
eligible graded inspection. We will also distinguish inspections
explicitly reporting no violations from records with missing
information. For mapping, we will validate coordinates, document
exclusions due to missing locations, and create an interactive map with
filters for borough, cuisine, and grade. Large data files will be kept
outside GitHub, with reproducible download and cleaning instructions
provided.

Planned Timeline - **November 13–20:** Adding the data to GitHub
repository, meet with the teaching team and check the feasibility of our
plan, confirm the challenge part and divide the work. - **November
21–27:** Consolidate inspection records, and conduct preliminary
exploratory analyses. - **November 28–December 4:** Complete geographic
and within-grade analyses, develop the interactive map and restaurant
comparison tool. - **December 5–9:** Integrate visualizations, complete
the written report, and finalize the project website. - **December
10–12:** Test interactive features, review reproducibility, record the
screencast, and submit
