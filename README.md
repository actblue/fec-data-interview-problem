## Data Scientist Technical Assessment

**Objective**: Draw insights from ActBlue’s (publicly available) FEC filing

**Materials**:

A sample of contribution data from ActBlue’s FEC filings:
  - `Data_Science_Technical_FEC_Filing_Sample.csv` is a sample of records derived from 3 of [ActBlue's monthly filings](https://www.fec.gov/data/committee/C00401224/?tab=filings&cycle=2020) in the 2020 cycle: [February Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1385527/), [March Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1391686/), [April Monthly 2020](https://docquery.fec.gov/cgi-bin/forms/C00401224/1402724/).
  
FEC committee data from the 2020 cycle:
  - `Data Science_Technical_FEC_Committee_Data_2020.csv` is derived from the Committee Master file for 2019-2020 provided on the [FEC Bulk Data page](https://www.fec.gov/data/browse-data/?tab=bulk-data).

CSVs are available in google drive [here](https://drive.google.com/drive/folders/1oRlG_vfbuMLvTNzH4foMvRqX_xPjrqIV?usp=sharing)

**Tools**:
R or Python preferred 

**Expectations**:
1. We don’t expect you to spend more than 90 minutes on this exercise, so just work through the questions within the time limit and see what you complete 
2. In the interest of respecting your free time, we suggest limiting any packages or modules imported to those referenced in the job description
3. We’re not looking for award winning visualizations, if you chose to generate a visualization feel free to use the default plot style
4. We think the provided data is sufficient to answer some really interesting questions and do not expect you to incorporate any additional data sources 
5. We don’t expect you to be familiar with our filing data - please make assumptions, but be sure to document them in your code so that we can follow your thought process.
6. When you’re ready, send us back a markdown file with your work (either RMarkdown or Jupyter notebook) or an R or Python file with your code  + comments to help us follow your work 

**Instructions**:

- Execute and present the data integrity checks you run before analyzing a new data set 
- Merge the `Data_Science_Technical_FEC_Filing_Sample` data with the `Data Science_Technical_FEC_Committee_Data_2020` data 
- Calculate how many donors gave to multiple federal committees?
- Calculate how many donors gave multiple contributions 
- Calculate the number of unique donors, committees, contributions in the sample data, along with the total dollars raised, and avg contribution size
- Ask and answer one to two questions of your own 
