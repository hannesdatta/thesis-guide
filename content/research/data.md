# Data

1. Description of data collection
    * Describe <ins>how</ins> the data was collected (e.g., web scraping, APIs, a cooperation with the       company)
    * Describe <ins>which</ins> data was collected (“the raw data”)
    * E.g., time frame, number of cross sectional units, type of data
    * As an example, see how I describe my own data collections in published papers
2. Data preparation and variable operationalization
    * Describe how you move from the raw data set to the final data set (see next two slides for an
      explanation)
3. Provide descriptive statistics of the <ins>**final data set**</ins>

!!! note ""
    Please have a look at Gordon, Brett R.,Avi Goldfarb, and Yang Li. "Does price elasticity vary with
    economic growth? A cross category analysis." Journal of Marketing Research 50.1 (2013): 4 23. This is
    a very well written description of how the data was prepared. Take it as an example/motivation of how
    you could write up your data section, too.


# Tips: Describe your raw data

* It is crucial that the reader (and your supervisor) understands the format of your data.
* You need to distinguish between your raw data, and your final data set.
* Your raw data
    * is how the data is stored at the company, or how you gathered the data yourself (e.g., using web scraping technology)

    <ins>**You need to know:**</ins>

    * What’s the “primary key” of this data? ( -> what identifies a unique row in this data set?)
          * For example, data may be stored per <ins>**video_id - day**</ins> (e.g., the number of YouTube  views per video per day), or per <ins>**shop - user - day**</ins> (recording sales of a user for an online shop per day)
          * Make explicit the frequency of your data (e.g., per month, week, day, hour, second…)
    * What are the “value” columns?
          * Value columns is data that is recorded per primary key (e.g., video views for YouTube, sales for the online shop).
    * Typically, you may encounter different tables with different primary keys and value columns
          * E.g., a table with user demographics, a table with sales data, a table with clickstream data,    etc.


* Create some summary statistics of this data
    * Always deliver
          * A table of mean, SD, min, max per variable (“descriptive statistics”)
    * Try to be creative
          * E.g., for sales data of a shop, create a summary of how many users buy per shop, or
          * E.g., for panel data (i.e., users/brands/artists observed over time): some time series plots (e.g., line graphs, for each user a line over time)



# Tips: Preparing your final data set

* You will use a statistical program (e.g., SPSS, R, STATA) to transform your raw data to your final data set that you will analyze
    * Note, in many settings, it really does not make sense to analyze the <ins>**raw data**</ins>; it is          <BR>(a) way too fine grained (e.g., recorded per minute, while a weekly level of analysis may                  be warranted), 
            <br>(b) way too messy (e.g., contains outliers), and 
            <br>(c) does not yet contain the independent variables you are actually interested in
* Tasks to arrive at your final data set
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


# Variable Operationalization (Example 1)

![Variable Operationalization Example 1](/assets/Variable_operationalization1.png){: style="width:500px"}
![Variable Operationalization Example 1](/assets/Variable_operationalization2.png){: style="width:500px"}

Datta[^1] 
[^1]:
Datta, H., Knox, G., & Bronnenberg , B. J. (2017). Changing their tune: How consumers’ adoption
of online streaming affects music consumption and discovery. Marketing Science.

# Descriptive statistics (Example 1/2)
![Descriptive statistics Example 1](/assets/Descriptive_statistics_eg1.png){: style="width:600px"}

Hannes[^2] 
[^2]:
Hannes Datta, Kusum L. Ailawadi , and Harald J. van Heerde (2017) How Well Does Consumer Based Brand Equity Align with Sales Based Brand Equity and Marketing Mi x Response?.* Journal of
Marketing:* May 2017, Vol. 81, No. 3, pp. 1 20.


# Descriptive statistics (Example 2/2)
![Descriptive statistics Example 2](/assets/Descriptive_statistics_eg2.png){: style="width:600px"}

Hannes[^3] 
[^3]:
Datta, H., Foubert, B., & Van Heerde, H. J. (2015). The challenge of retaining customers acquired with free trials.* Journal of Marketing Research,* 52(2), 217 234.


# Visualizations

* Also consider plotting interesting aspects of your data, e.g., my paper on Spotify
![Visualizations](/assets/visualization.png){: style="height:300px;width:600px"}

Datta[^4] 
[^4]:
Datta, H., Knox, G., & Bronnenberg , B. J. (2017). Changing their tune: How consumers’ adoption of online streaming affects music consumption and discovery. Marketing Science.