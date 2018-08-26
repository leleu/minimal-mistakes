---
title: "Benefits of Strong Data Foundations"
layout: single
permalink: /strong-data-foundations
author_profile: true
published: true
---

<blockquote>
	Data Scientists are only as good as the data they have access to. 
	<a style="font-size: .8em" href="https://www.dataquest.io/blog/what-is-a-data-engineer/">source</a>
</blockquote>

# The Dirty Underbelly of Data Science

With a nod to the quotation above, it's worth considering the tedius time-consuming tasks that most data scientists dislike.  Surveys regularly show that data wrangling (derisively called "data janitor work") takes up 25-75% of data scientists time.  Most data scientists are highly educated, often receiving graduate degrees or doctorates, and this type of work is more "hands dirty" than they are prepared for.

Here are a few problems commonly faced by data scientists.


<a name="clean-data"></a>
## Dirty Data
Data sources vary significantly in quality.  The gap between training (professor-provided data) and reality (dirty data) forces data scientists to spend a good chunk of their day doing tasks they're not well-trained for.

Real world data usually comes from multiple sources and has at least one difficult set.  Common problems include [inconsistent encoding](http://bitboost.com/ref/international-address-formats/united_states/), [awful specifications](https://www.dfas.mil/contractorsvendors/irapt/holdswawf/edi.html), or [whatever Excel file that's been (ab)used as a database](http://wyorock.com/excelasadatabase.htm) for the past 3 years.

Most of these tasks are tedious, although there are some libraries and services that can speed things up.

### Additional Reading
* Example of how much cleaning needs to be done, even on public/"clean" datasets ([NY City Taxi Data Cleanup](http://dracodoc.github.io/2016/01/31/data-cleaning/))

### Inconsistent Encoding
Addresses data is a common example.  ZIP Codes can be encoded as 92037, or 92037-1445.  Imagine the work required to standardize addresses, so you can compare the following values: `1445 Main St. Unit 1700` `1445 Main Street Unit 1700` `1445 Main Street, Suite 1700`.

### Awful Specifications
The US Government uses a format called EDI that has a recursive self-defined structure.  Data Scientists aren't making good use of their time learning specifications just to unroll and redefine the schema into something more useful.  That's to say nothing of how many [different file formats](http://opendatahandbook.org/guide/en/appendices/file-formats/) there are.

> The more uniform the data presented to the data scientist, the easier the analysis.

![image-right](/assets/images/excel-database.png){: .align-right}
### Excel/MS Access
Excel (or access) is a very common way to store structured data.  Most companies have important data in this format, so it's crucial to integrate as a source in most analyses.

Commonly, sales and finance teams use Excel to run their departments.  Until they can afford a switch to a CRM, they need to keep using spreadsheets.  That means the data used for analysis needs to be updated automatically, or data science efforts will be using out-of-date information.

<a name="deduplicating-data-for-data-scientists"></a>
## Deduplicated Data
Duplicate data frequently happens when combining multiple data sources.  Frequently, the data format and encoding ("Street" vs. "St") complicate simple comparisons.  If records aren't unique, you might end up counting James Smith and Jim Smith as two different customers (or something worse).

### [How Duplicate Data Harms Businesses](https://www.qgate.co.uk/blog/10-reasons-why-duplicate-data-is-harming-your-business/)


<a name="engineering-support-for-data-scientists"></a>
## Engineering Support
Organizations without the resources for fulltime data engineers should still provide some engineering support.
1. It frees up data scientist time to work on high value analyses
1. Many data scientists aren't skilled at engineering tasks
1. A strong data foundation supports repeatability, accuracy, and accelerates analysis efforts