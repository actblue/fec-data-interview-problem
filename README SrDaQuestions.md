# Senior Data Analyst / Data Scientist II Technical Assessment

## Expectations

1. We don’t expect you to spend more than 120 minutes on these two exercises, so just work through the questions within the time limit and see what you complete 
2. In the interest of respecting your free time, we suggest limiting any packages or modules imported to those referenced in the job description
3. We think the provided data is sufficient to answer some really interesting questions and do not expect you to incorporate any additional data sources 
4. We don’t expect you to be familiar with our filing data - please make assumptions, but be sure to document them in your code so that we can follow your thought process.
5. When you’re ready, send us back a text file with the refined SQL query (for exercise 1) and an attached file containing the data visualization you generated and the corresponding analysis (for exercise 2). 



### Exercise One: SQL Refactor
**Objective**: Refactor [this SQL Query](https://docs.google.com/document/d/17gBXAvGRIXUl9up7S794oHpLBQK6gIQw73u8eJSAB9M/edit?usp=sharing) so that it is easily readable by your teammates and fix any syntax errors you come across. 

**Background**: 
  - We store our data in a redshift database, and while we’ve done a lot of good work modeling this raw resource to help ourselves and teams across the organization quickly answer basic questions about fundraising patterns on our site through a BI tool, many of the deeper explorations our team does for the organization starts with manipulating the data stored in our redshift cluster using SQL. 
  - This query is a messy version of the query we used to pull the data used in exercise two of this take home. All of the where clauses, and table sources are correct and don’t need to be updated, but this is obviously not a great work product to share with colleagues - it’s hard to scan for quick understanding of the work, has inconsistent syntax, and there are some syntactical errors that would cause this query run to fail. 

**Suggested Time**: 30 minutes 

**Notes**:
  - If you are not familiar with Common Table Expressions (CTEs) check out [this resource](https://learnsql.com/blog/what-is-common-table-expression/)
  - Everyone has different SQL styles and we are intentionally not sharing our internal style guide, so prioritize consistency over a specific style 
  - Highly suggested that you leave comments throughout the file to explain your work, express uncertainty, or ask questions


### Exercise Two: Storytelling using a BI Tool 
**Objective**: Draw insights from ActBlue’s (publicly available) FEC filing using a BI tool of your choice e.g Tableau Public, Looker Data Studio, etc. 


**Materials**:

Dataset #1: A sample of contribution data from ActBlue’s FEC filings:
  - [`Data_Science_Technical_FEC_Filing_Sample.csv`](https://drive.google.com/file/d/1mHS1k9xC1JKcjrjtqCGvrEj14YzuDsLn/view?usp=drive_link) is a sample of records derived from 3 of [ActBlue's monthly filings](https://www.fec.gov/data/committee/C00401224/?tab=filings&cycle=2020) in the 2020 cycle: [February Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1385527/), [March Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1391686/), [April Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1402724/).
  
Dataset #2: FEC committee data from the 2020 cycle:
  - [`Data Science_Technical_FEC_Committee_Data_2020.csv`](https://drive.google.com/file/d/1oCMfdRZVSyFuhjIhtEMlq4a9upXbMDWp/view?usp=drive_link) is derived from the Committee Master file for 2019-2020 provided on the [FEC Bulk Data page](https://www.fec.gov/data/browse-data/?tab=bulk-data).


**Tools**:
Python or R (required) and BI tool 


**Instructions**:

- Execute and present the data integrity checks you run before analyzing a new data set. Additionally, include details about ways that you cleaned the data before analyzing it.  
- Merge the `Data_Science_Technical_FEC_Filing_Sample` data with the `Data Science_Technical_FEC_Committee_Data_2020` data
- Document and present any statistical analysis that you performed on this data (e.g cohort analysis). **For data science candidates, we do expect some demonstration of statistical knowledge, modeling, or machine learning**
- Using a BI tool of your choice visualize the FEC datasets. Then, ask and answer one to two questions of your own to tell us an interesting story with this data! 
- When using a BI tool to build your dashboard, include screenshot along with dashboard attached to ensure we can open it upon delivery 

**Suggested Time**: 90 minutes 
