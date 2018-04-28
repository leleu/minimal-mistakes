---
published: false
---

* [What's the Difference Between a Data Scientist, Data Engineer, and Data Wrangler?](/data-scientist-versus-data-engineer-versus-data-wrangle)






* They don't like doing it
> Cleaning and organizing data, as it turns out, is also data scientists' least favorite part of the job, according to more than half of CrowdFlower's respondents. https://www.infoworld.com/article/3047584/big-data/hottest-job-data-scientists-say-theyre-still-mostly-digital-janitors.html
> While data munging is an extremely useful and critical skill to have, most data scientists, many of whom have spent years learning complex math and machine learning, and have earned PhDs, do not want to spend time as data janitors. - 

## What Solutions Exist?

Article's points:
* Before data scientists can extract insights, data must be cleaned and pre-processed.  AKA data wrangling / data engineering / data janitorial services.


## Disparate data sources
a growing amount of analysis occurs in environments where the schema of data is not defined or known ahead of time. This means the analyst doing the wrangling is determining how the data can be leveraged for analysis as well as the schema required to perform that analysis https://tdwi.org/articles/2017/02/10/data-wrangling-and-etl-differences.aspx

* This takes up a lot of data scientists time
> Data scientists, according to interviews and expert estimates, spend from 50 percent to 80 percent of their time mired in this more mundane labor of collecting and preparing unruly digital data, before it can be explored for useful nuggets.  NYTimes.com - https://www.nytimes.com/2014/08/18/technology/for-big-data-scientists-hurdle-to-insights-is-janitor-work.html
> Cleaning Big Data: Most Time-Consuming, Least Enjoyable Data Science Task, Survey Says - https://www.forbes.com/sites/gilpress/2016/03/23/data-preparation-most-time-consuming-least-enjoyable-data-science-task-survey-says/#31189ab36f63

## (It's a lot of time)
* 53% have major involvement in data cleaning tasks
* 38% spend 1-4 hours/day on data cleaning tasks
* 30% have major involvement in ETL tasks, although this is decreasing as companies are hiring for a dedicated data engineer
* 25% spend 1-4 hours/day on ETL tasks




# Inefficient Use of Data Science Resources
> "You have your hardest-to-hire resource spending most of their time cleaning data," said Lukas Biewald, CrowdFlower's CEO. "It's a humongous waste for organizations." https://www.infoworld.com/article/3047584/big-data/hottest-job-data-scientists-say-theyre-still-mostly-digital-janitors.html


* Big data teams are trying to automate this
> Data experts try to automate as many steps in the process as possible. “But practically, because of the diversity of data, you spend a lot of your time being a data janitor, before you can get to the cool, sexy things that got you into the field in the first place,” said Matt Mohebbi, a data scientist and co-founder of Iodine.
> Plenty of progress is still to be made in easing the analysis of data. “We really need better tools so we can spend less time on data wrangling and get to the sexy stuff,” said Michael Cavaretta, a data scientist at Ford Motor, which has used big data analysis to trim inventory levels and guide changes in car design.
> “We’re trying to liberate people from data-wrangling,” Mr. Nanduri said. “We want to free up their time and save them from going blind.”
> Data requests are tedious


Data scienctists spend significant time doing preparation and cleaning tasks.  They don't enjoy these "data janitor" tasks and aren't trained to perform them efficiently.

Emotionally charged words
* liberate your data science team
* data janitors
* hardest to hire resources spending most of their time doing low impact low satisfaction work
* tedium


## Data Science != Data Engineering
<a href="http://community.datacamp.com.s3.amazonaws.com/community/production/ckeditor_assets/pictures/393/content_infographic_fixed.jpg" style="font-size: .8em">See Full Infographic from DataCamp.com</a>
{% include figure image_path="/assets/images/data-engineer-versus-data-scientist.png" alt="Data Scientists and Data Engineers Have Different Tasks" caption="Data Engineer != Data Scientist" %}

## Data Preparation is Dirty Work
Data preparation requires a different set of skills, and is the boring yet important grunt work required before value can be extracted from data.  Think of it like janitorial work -- wouldn't you rather your data scientists do what you hired them for, rather than cleaning the floor?

## Let Data Scientists do Data Science
You hired a data science team to add value to your product by processing data.  Organizations inevitably discover significant up-front requirements to bring in and clean disparate data sources before analysis can begin.
