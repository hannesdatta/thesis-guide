---
title: "Data quality checks"
draft: false
date: 2022-07-18T09:00:00+02:00
weight: 2
---

#### Importing the data

- Try to import the data to your statistical software; does it work? Or do you need to use some extra programs (e.g., setting up a database) to import the data?
- Ask the data provider for tips if you do not succeed reading in the data.

#### Verify documentation

- Is the data accompanied by a readme or documentation? It's advisable to read it well.
- Is there no documentation available? Create your own by starting with [this template](https://tilburgsciencehub.com/document/new-data/?utm_campaign=referral-short).
- Is the filename informative of the content of the file? Does it contain extra information (e.g., a timestamp) not included in the data?

#### Validity

- Check variable names and columns in the data; do you know what these variables mean? Do columns seem complete?
- How are variables operationalized/defined? Do numeric variables represent cumulative sums (e.g., total followers), or are they incremental (e.g., new followers on a given day?)

*Example:* Chartmetric's API lists a "listener-to-follower" ratio for about 1.1m playlists; it's easy to assume they have actual data on the number of listeners, but that metric is only approximated. A better name for the variable would have been estimated-listener-to-follower-ratio.

#### Accuracy

- Are all variable values feasible? Are there any values that do not make sense? (you may have to revise your definition)

*Example:* My data lists playlists by XXXTentacion – is this the "real" artist or a "fake artist"? For example, you can manually check user profiles on Spotify; similarly, when was an artist's first release?

#### Completeness

- Are there missing values? Are these really missings? (e.g., "NA" prices, versus NA sales (= 0 sales)

*Example:*

#### Consistency

- Do the values make sense consistently, or are there any "breaks" in the data definitions (e.g., for the first part of your data, some values are missing and only start to be present in the second part of your data)

*Example:* my playlist data has an indicator for whether a playlist was personalized – but that variable does not seem to be consistently defined.

#### Uniformity

- Check the measurement units of your variables – are those consistent, too?
- Are "strings" properly encoded? Or do some strings look like this: Ã¥?)

*Example:* the column "weight in kg" lists strawberries weighing 500 kg (should be .5kg)
