---
title: "Describe your raw data"
date: 2022-07-18T09:00:00+02:00
weight: 9
---

* It is crucial that the reader (and your advisor) understands the format of your data.
* You need to distinguish between your raw data, and your final data set.
* Your raw data is how the data is stored at the company, or how you gathered the data yourself (e.g., using web scraping or APIs)

    **You need to know and explain:**

    * What’s the “primary key” of this data? ( -> what identifies a unique row in this data set?)
      * For example, data may be stored per <ins>**video_id - day**</ins> (e.g., the number of YouTube  views per video per day), or per <ins>**shop - user - day**</ins> (recording sales of a user for an online shop per day)
      * Make explicit the frequency of your data (e.g., per month, week, day, hour, second…)
    * What are the “value” columns?
      * Value columns is data that is recorded per primary key (e.g., video views for YouTube, sales for the online shop).
    * Typically, you may encounter different tables with different primary keys and value columns
      * E.g., a table with user demographics, a table with sales data, a table with clickstream data,    etc.

* Create some summary statistics of this data
    * Always have a table of mean, SD, min, max per variable (“descriptive statistics”)

    * Try to be creative
        * E.g., for sales data of a shop, create a summary of how many users buy per shop, or
        * E.g., for panel data (i.e., users/brands/artists observed over time): some time series plots (e.g., line graphs, for each user a line over time)
