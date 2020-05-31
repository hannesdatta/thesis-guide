---
title: "Prepare your final data set"
date: 2020-05-11T09:00:00+02:00
weight: 10
---

* Typically, it really does not make sense to analyze the **raw data** that you have collected.
  * raw data may not be at the unit of analysis of other relevant variables (e.g., you collected data at the SKU-level,
  while your dependent variable is at the brand level),
  * raw data may not yet contain the independent variables you are actually interested in, and you need to prepare for merging,
  * raw data may be too messy (e.g., contains outliers), and
  * raw data may be too fine grained (e.g., recorded per minute, while a weekly level of analysis may be warranted).

**How to arrive at a final (cleaned) data set?**

* Data cleaning

    * E.g., refine your sample (e.g., “shops that sell at least 1 item per week”; “brands that are in the Top 3 for at least three con secutive years”,etc.
    * E.g., define rules how to deal with missing values and outliers

* Data aggregation

    * E.g., aggregate from minutes to weeks; aggregate from sales per user per shop, to sales per shop (“same primary key”)

* Data merging

    * E.g., merge different sources (which have previously been aggregated to the same primary key); e.g., temperature data (record ed per day),to your sales data set for swimming equipment ;) (per shop, and day)

* Operationalize your variables

    * Which are the variables you want to use for your analyze, and how do you operationalize them? (e.g., think of raw data that stores the names of products sold in a given month -> you could convert this to a measure of how many products are sold in a given month, simply by counting them. So from your raw data, you get to a real variable that you can use (e.g., note the previous variable was text, an d now you have a count, e.g., number of SKUs)
    * Typically, you provide a table with <ins>**variable names, and your operationalization.**</ins>
    * Look at the literature and how previous researchers have defined variables that you are looking for.
