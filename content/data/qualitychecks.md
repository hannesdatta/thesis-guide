---
title: "Check data quality"
draft: false
date: 2020-08-26T09:00:00+02:00
weight: 1
---

Upon data delivery (e.g., by your coach, or by a company), it's important you assess data quality and see whether you need to follow up with your data provider to clarify or solve inconsistencies.

The best way to go about is to *read in the various data files in your statistical program*, and use simple descriptive statistics and plots to inspect the data.

- Inspect your raw data, or aggregations thereof, by looking at the data tables (e.g., `View` in R, or simply by loading data into Excel if file sizes permit)
- Cross-tabulate data (e.g., `table()` in R, pivot tables in Excel)
- Plot your data (e.g., `plot()` in R), or distributions of your data (e.g., `hist()` in R); many times, it is advisable you first aggregate your raw data by a common unit (e.g., brands, time, playlists, clusters), before plotting.

### Quality checks

#### Reading in the data

- Try to read in the data to your statistical software; does it work? Or do you need to use some extra programs (e.g., setting up a database) to read in the data?
- Ask the data provider for tips if you do not succeed reading in the data.

#### Verify documentation

- Is the data accompanied by a readme or documentation? It's advisable to read it well.
- Is there no documentation available? Create your own one, by starting with [this template](http://tilburgsciencehub.com/workflow/documenting-data/).
- Is the filename informative of the content of the file? Does it contain extra information (e.g., a timestamp) which is not contained in the data itself?

#### Validity

- Check variable names and columns in the data; do you know what these variables really mean? Do columns seem complete?
- How are variables operationalized/defined? Do numeric variables represent cumulative sums (e.g., total followers), or are they incremental (e.g., new followers on a given day?)

*Example:* Chartmetric’s API lists a “listener-to-follower” ratio for about 1.1m playlists; it’s easy to assume they have actual data on the number of listeners, but, in fact, that metric is only approximated. A better name for the variable would have been estimated-listener-to-follower-ratio.

#### Accuracy

- Are all variable values feasible? Are there any values that do not make sense? (you may have to revise your definition)

*Example:* Example: my data lists playlists by XXXTentacion – is this the “real” artist, or a “fake artist”? For example, you can check user profiles on Spotify manually; similarly, when was an artist’s first release?

#### Completeness

- Are there missing values? Are these really missings? (e.g., “NA” prices, versus NA sales (= 0 sales)

*Example:*

#### Consistency

- Do the values make sense consistently, or are there any “breaks” in the data definitions (e.g., for the first part of your data, some values are missing, and only start to be present in the second part of your data)

*Example:* my playlist data has an indicator for whether a playlist was personalized – but that variable does not seem to be consistently defined.

#### Uniformity

- Check measurement units of your variables – are those consistent, too?
- Are “strings” properly encoded? Or do some strings look like this: Ã¥?)

*Example:* the column “weight in kg” lists strawberries weighting 500 kg (should be .5kg)
