# Oral-Insulin-Phase-II-Clinical-Trial-Data-Analysis using Python

# Introduction

> What is Insulin?

> Insulin is a naturally occurring hormone your pancreas makes that’s essential for allowing your body to use sugar (glucose) for energy. If your pancreas doesn’t make enough insulin or your body doesn’t use insulin properly, it leads to high blood sugar levels (hyperglycemia). This results in diabetes.

# Objective
To compare the effectiveness of the new oral insulin (Auralin) and injectable insulin (Novodra) in patients with type 1 diabetes.

# Dataset: Auralin and Novodra Trials
> The dataset is phase two clinical trial data of 350 patients for a new innovative oral insulin called Auralin - a proprietary capsule that can solve this stomach lining problem.

> Phase two trials are intended to:
- Test the efficacy and the dose response of a drug.
- Identify adverse reactions.
- 
# Data Wrangling
In this section, all three pieces of data are gathered, accessed its quality and tidiness issues and cleaned the data for better analysis and visualization.

### Gather data
> In this section, the three pieces of data are loaded to dataframes using pandas `read_csv`
- Patients data
- Treatments data
- Adverse reactions data

### Assess data
> In this section, the datasets are accessed to detect quality and tidiness issues using visual and programmatic assessments.

#### Quality Issues
> They are issues with the data content like missing data, Inaccurate data, Inconsistent data etc. It is also known as dirty data.
> Some of the issues:

Patients table
- Inconsistent data in the zip code column. Zip code should be string not float
- Height column: Tim Neudorf height is 27 inches instead of 72 inches
- Default John Doe data
- Given name column: Inaccurate data for Dsvid instead of David
- State column: Inconsistent data, using full and abbreviation names.
- Data type issue: assigned sex, state, zip code and birthdate columns.

<p> <i> Treatments table </i> </p>
- Missing values in hba1c change column.
- Invalid data in auralin and novodra columns.
- lowercase given name and surname.
- Missing records: 280 records instead of 350 records.

#### Tidiness Issues
> They are issues with the structure of the data.
- Contact column in patients table should be split into phone number and email
- Three variables in two columns in treatments table (treatment, start dose and end dose)
- Adverse reaction should be part of the treatments table

### Clean data
> In this section, the quality and tidiness issues are cleaned for better analysis and visualization.

## Data Insights
- Diabetic Patients with healthy weight (18.5 – 24.9) and overweight (25.0 – 29.9) tend to have more frequency scores compared to other weight status. From the distribution, weight seems to have less impact on diabetes.
- Auralin and Novodra insulins have similar adverse reactions excluding throat irritation and injection site discomfort. Throat irritation for Auralin, which is expected because this pill is taken orally while injection site discomfort for Novodra, which is caused by injection needles.
- Auralin patients required an average of 8 more units of insulin to establish a normal blood sugar level compared to Novodra patients who required  an average of 0.4 units less of insulin. 
- The difference in the Mean Hba1c Change of Auralin and Novodra is much smaller which may imply the new oral insulin is effective and can help reduce high blood sugar level.
Auralin (oral) insulin required more dosage of the insulin to help reduce the hbalc (hemoglobin A1c) while Novodra (injectable) insulin required less dosage of the insulin to help reduce the hbalc (hemoglobin A1c).

## Conclusions
> The project was done to test the effectiveness of the new oral insulin Auralin compared to injectable insulin Novodra in diabetic patients. The results of the trial demonstrate that the new Auralin oral insulin is noninferior to the standard Novadra injectable insulin for reducing HbA1c in patients with type 1 diabetes.

> You can check out the full documentation <a href=''>here</a>

## Skills and Technologies
- Python libraries (Pandas, Matplotlib, NumPy, Seaborn)
- Data Wrangling
- Data Visualization

