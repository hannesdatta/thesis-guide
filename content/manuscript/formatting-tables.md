---
title: "Formatting tables and figures"
date: 2020-05-20T09:00:00+02:00
weight: 60
---

* Tables need to be formatted yourself, e.g., in Word or Excel, or Latex (put differently, do not merely paste the output from your statistical program in the main text - these are often too elaborate, or do not efficiently combine the results of multiple models)
    * Statistical packages like R have fantastic packages (e.g., `stargazer`), which allow you to generate publication-ready HTML or Latex tables that you can include in your manuscripts.
    * The same holds for figures; the R package `ggplot2` is recommended, but also R's regular plotting functionality is great.
* Tables and figures should be understandable without reading the
  corresponding sections in the manuscript
    * Use a clear title: easy to understand, and comprehensive (e.g., *summarize* the main point in the title (e.g., "X increases Y"), rather than using generic titles ("Results").
    * Provide comprehensive table notes wherever necessary.
    * Use clear labels, e.g., for variables
* Note that you can also combine tables into larger ones, and thereby save space (e.g.,
  tables with the same explanatory variables but different coefficients)
* Avoid colors, also in figures. Most readers will print your thesis in greyscale.
