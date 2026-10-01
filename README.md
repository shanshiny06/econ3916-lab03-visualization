# econ3916-lab03-visualization
# Honest vs. Misleading Visualizations

## Objective

This project demonstrates how identical data can be made to tell completely different stories depending on chart design choices, using a quantitative measure (the Lie Factor) to expose and correct misleading visualizations.

## Methodology

- Recreated Anscombe's Quartet, four datasets that share identical means, variances, correlation, and even the same least-squares regression line, despite having completely different underlying shapes
- Computed a Lie Factor of 49.0 for a truncated-axis revenue chart, showing that a true 4.1% revenue increase was visually distorted to look like a 200% jump, then redesigned the chart honestly as a zero-based dot plot with labeled values
- Drew four different versions of real average hourly earnings, pulled from FRED's AHETPI series and deflated to 2020 dollars, each using a different axis choice (full honest range, truncated axis, cherry-picked recent window, and log scale) to show how the same data can support four different narratives
- Ran a four-step exploratory data analysis checklist, structure, distributions, relationships, and anomalies, on World Bank GDP data covering 262 economies across 1960 to 2023, including a missing-data heatmap that revealed coverage gaps concentrated at the start and end of the time period rather than scattered randomly
- Built an interactive chart toggler with adjustable axis floor, year window, and log/linear scale, paired with a live Lie Factor readout that updates with every setting

## Key Findings

- A chart's summary statistics can be completely honest while its visual design is completely misleading; a Lie Factor of 49.0 on the revenue chart showed that truncating the y-axis turned a modest 4.1% increase into something that looked 49 times more dramatic than it actually was
- Anscombe's Quartet proved that identical means, variances, and correlations can hide a straight line, a curve, a near-perfect fit disrupted by one outlier, and a relationship driven entirely by a single data point, which is why visualization must happen before trusting any summary statistic
- The same real wage series can be used to argue completely opposite narratives depending on the axis choice: a full, honest view shows decades of stagnation followed by recent gains, while a cherry-picked recent window alone makes it look like uninterrupted progress
- Missing GDP data in the World Bank panel was not random; gaps clustered heavily at the earliest and most recent years, consistent with limited historical statistical capacity and reporting lag rather than any random process
