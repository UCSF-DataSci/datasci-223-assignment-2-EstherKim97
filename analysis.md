# Patient Cohort Analysis Report

## Analysis Approach
The patient cohort analysis is conducted by loading the patient data from a CSV file, which was converted to a Parquet file for efficient processing. Then, Polar's lazy API was applied to build an efficient data pipeline. 

For the data, BMI outliers were filtered out (values < 10 or > 60) and patients were grouped by BMI ranges manually. The average glucose level, patient count, and average age were calculated for each BMI range.

## Patterns and Insights
The cohort analysis summary shows that there is a clear increasing trend in the average glucose from underweight to obese. Also, for the number of patients for each BMI range, the number of patients increases from underweight to obese. The average age also increases from underweight to obese. For all average glucose, patient counts, and the average age, the values increase from underweight to obese.

## Use of Polars for Efficiency
The CSV file was converted to a Parquet file for efficient processing and the Polars were applied. Also, filtering out outliers and grouping patients by BMI ranges were done using the Polar. 
