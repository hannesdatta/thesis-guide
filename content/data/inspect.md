---
title: "Inspect your data"
draft: false
date: 2022-07-18T09:00:00+02:00
weight: 1
---

Upon data delivery (e.g., by your coach, by a company, or when you collected the data using web scraping or APIs), it's important you try opening the data to assess its quality. This gives you a chance to follow up with your data provider or debug your extraction code before it's too late.

The best way to go about is to *read in the various data files in your statistical program*, and use simple descriptive statistics and plots to inspect the data.

- Inspect your raw data, or aggregations thereof, by looking at the data tables (e.g., `View` in R, or simply by loading data into Excel if file sizes permit)
- Cross-tabulate data (e.g., `table()` in R, pivot tables in Excel)
- Plot your data (e.g., `plot()` in R), or distributions of your data (e.g., `hist()` in R); many times, it is advisable you first aggregate your raw data by a common unit (e.g., brands, time, playlists, clusters), before plotting.
