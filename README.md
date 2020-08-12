# Salary-Analysis
# Salary-data-analysis-portfolio
Salary data analysis project (Python)
## Define the problem

Let's say we are the job seeker who's gotten our very first offer and has no clue on negotiation, or maybe we are HR who has to decide how much to pay this person in his/her new job, here comes this project where we define and analyse the features which get you the salary expected, across several aspects such as position,degree and the industry you work in etc. 


## Objective
Analyse the salary dataset and determine which feature has great impact and least impact on salary.

## Data:
The data is part of an existing data set that includes employee information.The actual size of the dataset is 1,000,000 rows.

**Description of features:**  
• **JobId**: Job Identifier Used to track the jobs.(Unique key)  
•	**CompanyId** : Company identifier.  
•	**JobType** : Position within the company(Categorical)  
•	**Industry** : Industry of the job.(Categorical)  
•	**Degree** : Level of degree of candidate in the job.(Categorical)  
•	**Major** : Major of the degree in.(Categorical)  
•	**Years of Experience** : Experience of candidate in years.(Numerical continuous)  
•	**Miles from metropolis** : Distance from the nearest metropolis.(Numerical continuous)  
•	**Salary** : The annual salary .(Numerical continuous) Also defined in thousands.  

### Preprocessing:
* Merged two datasets - train and salary- into single dataset. 
* For the data cleaning process, I removed 5 rows, where salary =0, which indicates missing/corrupted value.
### Issues with data:
* *Lower bound outliers:* We have 5 entries with salaries =0, and while examining those entries, it seems like they are not volunteer jobs. So might be a missing/ corrupted entries.
* *Upper bound outliers:* We have few entries with some junior level people getting C-level salaries. But while analysing we figured out that most of them are from highly paid industries like  Oil /Finance industries. So no chance of that being corrupted data, so we are keeping them in the dataset.

## A few results from analysis:

* From our analysis, we found that companyId is not an important feature affecting the salary, as the average salary for each company seem to be across the same range.
* There is a high correlation between industry, degree and salary.
* When the experience increases, the salary also increases.
* There is a negative coreelation between Miles from Metropolis and salary.

## Conclusion:
One key take away from this project was to see how an individual's industry significantly influences their salary. For example, one could have a PhD, but are likely to earn more in the Oil and Finance industry than Service or Education. Perhaps students looking to invest in student loans could make a more informed decision about the level of education they might pursue while considering the potential salary earnings they could expect based on their desired industry.

**Language:** Python  
**Libraries used :** sklearn, pandas, seaborn, matplotlib, numpy
