# Higher Education Assessment Score Prediction, R

Analyzed large-scale education data in R to examine whether submission timing predicts assessment performance. Conducted data cleaning, visualization, correlation analysis, and linear regression on 170k+ records. Found that timing has a statistically significant but negligible effect on scores.

---

## Research Question
Does the number of days between the start of a learning module and assessment submission predict a student’s score?

Conclusion
- The results of the correlation and linear model suggest that timing alone is a weak predictor of student performance.
- Assessment submission timing showed a small, negative correlation with student assessment scores.
- Linear Regression indicated that each additional day a student submitted their assessment, from the first day of the module, could decrease their assessment score by .009 points (per day). 
- Submission timing explained approximately 0.1% of score variation

---

## Challenges
- There were no other independent variables included with the initial dataset, which limited further analysis.
- The dataset contained over 173,000 observations, which resulted in overplotting of the scatterplot. 
- To address this, I had to conduct research, outside of my learned skills, to determine the best way to generate a readable scatterplot. 

## Cool Techniques
- Though I was presented with a visualization challenge, due to the large data set, I learned valuable new ways to visualize using ggplot. For example, I learned to experiment with bins, in order to create a readable and interpretable scatterplot. 

## If I had more time
- If I had more time I would test other independent variables such as, students' education level, gender. I would use different statistical tests such as T-test or ANOVA. 


**Source:** Knowledge Media Institute, The Open University
https://analyse.kmi.open.ac.uk/open-dataset


## Data acquisition

I read in the CSV dataset ("studentAssessment.csv") from the Knowledge Media Institute, The Open University website

---

## Data Techniques
- Removed missing values, NAs
- Renamed dataframe columns to improve readability and analysis 
- Transformed the “score” variable from character to numeric in order to run the correlation test and linear model.
- Created a new dataframe using setseed(42) and a random sample of 5000, in order to reduce overplotting on the scatterplot, thus improving readability and interpretation. 
- Bins for the scatterplot

---

## Analytical Techniques
- Exploratory visualization using ggplot
- Diagnostic analysis
-   Spearman Correlation
-    Pearson's product-moment correlation
-   Simple Linear Regression Model

## Data Visualization
- scatterplot using ggplot

