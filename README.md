# Student Performance Analysis in R

This is a reproducible R mini project using **250 fictional student records**. The synthetic dataset makes richer plots possible without using or presenting invented values as real student records. All analysis uses base R; no package installation is required.

## Run the project

Open `student_performance_analysis.R` in RStudio and click **Source**. The script creates the dataset if it is missing, runs the analysis, displays six plots in the Plots pane, and saves the charts and tables in `output/`.

To recreate the project dataset, run `create_student_performance_dataset.R`. The fixed random seed recreates the same 250 rows.

## Variables in the dataset

| Variable | Meaning |
| --- | --- |
| `Student_ID` | Fictional ID, not a real student identifier |
| `Study_Hours_Per_Week` | Simulated weekly study hours |
| `Attendance_Percent` | Simulated attendance percentage |
| `Assignment_Average` | Simulated assignment score out of 100 |
| `Previous_Term_Average` | Simulated previous-term average out of 100 |
| `Sleep_Hours_Per_Night` | Simulated nightly sleep hours |
| `Final_Exam_Score` | Simulated final exam score out of 100 |

## Analysis included

- Score distribution and score bands
- Score spread across weekly study-time groups
- Attendance and assignment relationships with final scores
- Correlation matrix across the numeric variables
- A simple linear regression model with a reproducible 75/25 train/test split
- Held-out predictions evaluated with RMSE, MAE, and R-squared

## Files written to `output/`

- `student_results.csv`
- `study_group_summary.csv` and `attendance_group_summary.csv`
- `correlation_matrix.csv`
- `model_metrics.csv`, `model_coefficients.csv`, and `held_out_predictions.csv`
- `key_insights.csv`
- Six PNG charts numbered `01` through `06`, plus a six-page `student_performance_charts.pdf`

## Important interpretation note

The values and relationships are simulated for practicing data analysis. They are not evidence about real students, and the model must not be used to evaluate or make decisions about any person. Even with real observational data, correlations alone would not show that a habit causes an exam result.

The initial 10-row example is preserved under `archive/` for reference. The active project uses the reproducible 250-row dataset in `data/`.
