# Oral-Insulin-Phase-II-Clinical-Trial-Data-Analysis using Python

# Introduction

> What is Insulin?
Insulin is a naturally occurring hormone your pancreas makes that’s essential for allowing your body to use sugar (glucose) for energy. If your pancreas doesn’t make enough insulin or your body doesn’t use insulin properly, it leads to high blood sugar levels (hyperglycemia). This results in diabetes.

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

### Quality Issues
They are issues with the data content like missing data, Inaccurate data, Inconsistent data etc. It is also known as dirty data.
Some of the issues:
<i> Patients table </i>
- Inconsistent data in the zip code column. Zip code should be string not float
- Height column: Tim Neudorf height is 27 inches instead of 72 inches
- Default John Doe data
- Given name column: Inaccurate data for Dsvid instead of David
- State column: Inconsistent data, using full and abbreviation names.


