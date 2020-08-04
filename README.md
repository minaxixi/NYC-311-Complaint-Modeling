# NYC-311-Complaint-Modeling

## Goal
This is a project on modeling and visualizing the New York City 311 Hotline complaint type based on time and users' location.

## Data
The New York City 311 Hotline data are downloaded from [NYC Open Data](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9) and stored on AWS at the time of this project

There are 23.5 MM rows and 41 columns in this dataset in total. I subselect 500k rows from 2014-2019 to perform this analysis.

## Summary and Key Conclusions
- Developed a multi-class classification LightGBM model to predict the top 10 complaint type by count.
- Utilized the top-3 accuracy as metrics due to the nature of this problem (considered to be correct as long as the top-three predictions match).
- Achieved a top-3 accuracy of 0.97, which suggests that the caller's complaint type is correlated with their locations and time of the call.

## Package Dependencies
- Python 3.6.5
- Matplotlib 2.2.2
- Seaborn 0.9.0
- Pandas 0.23.0
- Scikit-Learn 0.19.1
- LightGBM 2.2.1
