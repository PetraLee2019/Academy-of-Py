Analysis - Academy of Py
As per the District and School Summary, students are doing better in reading rather than math. But the overall passing rate is not very satisfactory for all the schools. Going forward, more attention is required for getting better scores in Math to improve the overall scores and performance of the schools.

Top performing schools are mostly charter schools. There is a significant difference in overall passing rates of the charter and district schools - Overall passing rate : Charter -> 91% & District -> 71%

The overall performance of students is very good from the schools which have less budget (<585) as compared to the schools which are spending more on students.

The smaller and medium sized school's performance is much better than the large sized schools in Math. Performance in Math: Small and medium size -> 89% - 91% whereas large size -> 67%. This may be due to the reason that the student population in charter schools is less than the district schools.

# Dependencies
import pandas as pd
import numpy as np

# Load csv files
schools = 'Resources/schools_complete.csv'
students = 'Resources/students_complete.csv'

# Read school file with pandas
school_df = pd.read_csv(schools)

# Check columns of schools data 
school_df.columns

# Rename columns in school dataset
school = school_df.rename(columns={'name' : 'School','type' : 'Type','size' : 'Size','budget' : 'Budget'})
school.head()

<style> .dataframe thead tr:only-child th { text-align: right; }
.dataframe thead th {
    text-align: left;
}

.dataframe tbody tr th {
    vertical-align: top;
}
