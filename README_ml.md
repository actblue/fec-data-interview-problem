# Data Scientist Technical Assessment

## Expectations

1. We don’t expect you to spend more than 120 minutes on these exercises, so just work through the questions within the time limit and see what you complete 
2. In the interest of respecting your free time, we suggest limiting any packages or modules imported to those referenced in the job description
3. We’re not looking for award-winning visualizations, if you chose to generate a visualization feel free to use the default plot style
4. We think the provided data is sufficient to answer some really interesting questions and do not expect you to incorporate any additional data sources 
5. We don’t expect you to be familiar with our filing data - please make assumptions, but be sure to document them in your code so that we can follow your thought process.
6. When you’re ready, send us back a markdown file with your work (either RMarkdown or Jupyter notebook) or an R or Python file with your code  + comments to help us follow your work


### Exercise One: SQL Refactor
**Objective**: Refactor [this SQL Query](https://docs.google.com/document/d/1idPKfrhwhuw5C5qDMwWun0MI5wQaBI288RFMafcTDos/edit?usp=sharing) so that it is easily readable by your teammates and fix any syntax errors you come across. 

**Background**: 
  - We store our data in a redshift database, and while we’ve done a lot of good work modeling this raw resource to help ourselves and teams across the organization quickly answer basic questions about fundraising patterns on our site through a BI tool, many of the deeper explorations our team does for the organization starts with manipulating the data stored in our redshift cluster using SQL. 
  - This query is a messy version of the query we used to pull the data used in exercise two of this take home. All of the where clauses, and table sources are correct and don’t need to be updated, but this is obviously not a great work product to share with colleagues - it’s hard to scan for quick understanding of the work, has inconsistent syntax, and there are some syntactical errors that would cause this query run to fail. 

**Suggested Time**: 30 minutes 

**Notes**:
  - If you are not familiar with Common Table Expressions (CTEs) check out [this resource](https://learnsql.com/blog/what-is-common-table-expression/)
  - Everyone has different SQL styles and we are intentionally not sharing our internal style guide, so prioritize consistency over a specific style 
  - Highly suggested that you leave comments throughout the file to explain your work, express uncertainty, or ask questions


### Exercise Two: Model Building and Deployment
**Objective**: Build a predictive model from ActBlue’s (publicly available) FEC filing

**Materials**:
A sample of contribution data from ActBlue’s FEC filings:
  - [`Data_Science_Technical_FEC_Filing_Sample.csv`](https://drive.google.com/file/d/1IO8Tpzip90NwAKdA-VU0soaj2RyNFIk4/view?usp=sharing) is a sample of records derived from 3 of [ActBlue's monthly filings](https://www.fec.gov/data/committee/C00401224/?tab=filings&cycle=2020) in the 2020 cycle: [February Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1385527/), [March Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1391686/), [April Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1402724/).
  
FEC committee data from the 2020 cycle:
  - [`Data Science_Technical_FEC_Committee_Data_2020.csv`](https://drive.google.com/file/d/1qQ-tAEW9VVH-hyafndohCMQ87AKmhL6U/view?usp=sharing) is derived from the Committee Master file for 2019-2020 provided on the [FEC Bulk Data page](https://www.fec.gov/data/browse-data/?tab=bulk-data).

**Suggested Time**: 90 minutes

**Tools**:
R or Python preferred 


**Instructions**:
- Execute and present the data integrity checks you run before analyzing a new data set 
- Merge the `Data_Science_Technical_FEC_Filing_Sample` data with the `Data Science_Technical_FEC_Committee_Data_2020` data
- Create a feature set
- Choose an appropriate predictive model
- Train the model and evaluate its performance
- (Optional for all, required for Sr. level) Wrap the model in a very simple API (e.g. Flask, Docker)
