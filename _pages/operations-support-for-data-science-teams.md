---
title: "Notes - Engineering/Operations Support for Data Science Teams"
layout: single
permalink: /data-operations-support-notes
author_profile: false
published: true
---
Investing in support and tools for these teams has compounding returns.  Every hour of their time saved returns the investment because they are freed to focus on high impact activities to help you build a better product.

Data scientists extract value from data.  Before this can be done, it has to be acquired and pre-processed, doing things like augmenting analytics beacons with weather and location data, before standardizing the data models.  This is infrastructure work -- creating data schemas, rollup strategies, provisioning infrastructure, cleaning/deduplicating data, and finally pushing into a data warehouse that makes everything nice and clean for the fancy data scientists to do their thing.

Most data scientists' education focuses on the algorithms, insight, and communications, with very little time put into scraping techniques, deduplication strategies, or the operational approach to keep data flowing through the pre-processing pipelines.

One other thing -- most data scientists don't like doing that work.  It's not sexy -- you don't get flashes of insight.  When it's done well, it's not something that directly improves revenue.  However, when it's done poorly, it hamstrings data science teams.

Finally, the education and training provided by most data science programs trains practicitioners to use pre-processed data.  As a result, data scientists tend to not be experts in the more engineering-y tasks.

<blockquote>
	Data scientists continue to spend the most amount of their time on the work they like the least -- namely collecting, labeling, cleaning, and organizing data.<br />
	<a style="font-size: .8em" href="https://visit.crowdflower.com/WC-2017-Data-Science-Report_LP.html">source</a>
</blockquote>

<blockquote>
	Data Scientists are only as good as the data they have access to.<br />
	<a style="font-size: .8em" href="https://www.dataquest.io/blog/what-is-a-data-engineer/">source</a>
</blockquote>

<blockquote>76% of data scientists say data preparation is the least enjoyable part of their job<br>
<a style="font-size: .8em" href="https://www.forbes.com/sites/gilpress/2016/03/23/data-preparation-most-time-consuming-least-enjoyable-data-science-task-survey-says/#718b613b6f63">source</a>
</blockquote>

Modified Version (original below)
<img src="/assets/images/data-engineer-versus-data-scientist.png">
DataCamp Infographic: https://www.datacamp.com/community/blog/data-engineering-vs-data-science-infographic

## Data Scientist vs. Data Engineer
* *Data Engineering* Extract/Load/Transform.  Input: raw data.  Output: clean data warehouse for data scientists to use.
* *Data Science* Discover/Access/Distill.  Input: clean data.  Output: business value.


## Data Scientists Are Rarely Effective Data Engineers
* Data must be pre-processed and made available before Data Scientists can extract value
* Data Scientists aren't extensively trained in collecting, cleaning, and pre-processing data.
* The work is unsexy, like much infrastructure or foundation work.

Time spend on ETL and data cleaning is time not spent directly extracting value from insights.

<blockquote>
	Data cleaning is also probably one of the longest and most tedious tasks, calling to mind the old quote attributed to Abe Lincoln, “Give me four hours to chop down a tree and I’ll spend the first three sharpening my axe.”<br>
	<a href="http://www.oreilly.com/data/free/2017-data-science-salary-survey.csp" style="font-size: .8em">[O'Reilly 2017 Data Science survey]</a>
</blockquote>

## Data Scientists Spend a Lot of Time Doing Data Engineering Tasks
* 53% have major involvement in data cleaning tasks
* 38% spend 1-4 hours/day on data cleaning tasks
* 30% have major involvement in ETL tasks, although this is decreasing as companies are hiring for a dedicated data engineer
* 25% spend 1-4 hours/day on ETL tasks

Given the value they provide, and the relatively high cost per hire, it's important to maximize the efficiency of data science teams.  <a href="http://www.oreilly.com/data/free/2017-data-science-salary-survey.csp" style="font-size: .8em">[source: O'Reilly 2017 Data Science survey]</a> 

## Why Asking Data Scientists to do engineering tasks is a bad idea
* Lack of experience and low affinity for the work deprioritizes ETL tasks
* Data Engineering tasks take longer and are lower quality
* Data Science teams "limp along", generating technical debt but lacking the expertise to pay it back
* Technical debt in the data systems limit the value of extractable insight
* Data Science teams spend more time doing Engineering tasks, less time doing data science

## In-House vs. Contract
Companies who rely on data in their product, or who operate at a certain scale, are best served by hiring a full time data engineer (or team of engineers).  Many companies, especially those with under 20 software engineers or just a couple data scientists, might not need an engineer full time.  Building a data pipeline is a heavy up-front time investment, but once it's up and running, you don't necessarily need a FTE engineer.




Your business wants to extract valuable information from the raw data you collect.  This necessitates collection, cleaning, processing, and serving of data before any analyses can be performed.



There is significant disagreement as to what constitutes a data scientist.  [https://en.wikipedia.org/wiki/Data_science](Wikipedia) defines it as __an interdisciplinary field of scientific methods, processes, algorithms and systems to extract knowledge or insights from data in various forms__, a definition that