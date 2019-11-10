# project2
Black Friday Sales to Gun Violence Comparison

* The sources of data that you will extract from.
	-We pulled our 2 data sets from:
https://www.kaggle.com/jameslko/gun-violence-data/download, https://www.thebalance.com/what-is-black-friday-3305710

* The type of transformation needed for this data (cleaning, joining, filtering, aggregating, etc).
	-We had a lot of cleaning to do as the gun violence data was 147mb. We were able to shorten it and get rid of a lot of the mess. We brute force typed out the years of financial data. Once we cleaned the 2 data sets, we merged them on year and added the other columns. We aggregated the gun violence data, since it was of all 50 states, into the sum of total killed and injured.

* The type of final production database to load the data into (relational or non-relational).
	-Relational.

* The final tables or collections that will be used in the production database.
	-

You will be required to submit a final technical report with the above information and steps required to reproduce your ETL process.

## Project Report

At the end of the week, your team will submit a Final Report that describes the following:

* **E**xtract: your original data sources and how the data was formatted (CSV, JSON, pgAdmin 4, etc).

	-We used 2 methods to extract from our source. We extracted the gun violence data from the provided csv from: https://www.kaggle.com/jameslko/gun-violence-data/download
	-We brute force extracted by typing out the small amount of data we pulled from https://www.thebalance.com/what-is-black-friday-3305710

* **T**ransform: what data cleaning or transformation was required.
	-Changed the names of the some of the columns
	-Reset the index
	-Dropped the previos idex
	-Aggregated the number killed and injured since the sum compared to year was all we cared about but there were all 50 states reports.

* **L**oad: the final database, tables/collections, and why this was chosen.
	-We only used the total sales and gun violence data for the columns and the common key was the year. Now this new beautifully ETL'd data is ready for a data warehouse for other data scientists to use.

Please upload the report to Github and submit a link to Bootcampspot.
