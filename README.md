# a1906373_Tran-Huu-Hao-Nguyen_Assignment-1--Part-D
Assignment 1_Part D_Comprehensive Final Report

## Student Habits and Academic Performance Prediction

### **Overview**
The research investigates the connections between student lifestyle choices and academic results together with their mental health markers.  
The analysis uses regression and classification models to forecast:

- **Exam Score** (continuous target)
- **Pass/Fail outcome** (binary target)

The *Student Habits and Academic Performance Dataset* serves as the data source for this analysis, which follows a systematic approach starting with:
1. Data preprocessing  
2. Feature engineering  
3. Model selection  
4. Model training and tuning  
5. Model evaluation  

## **Repository Structure**

├── data/
│ ├── student_habits.csv # Original dataset
│ ├── processed_data.csv # Cleaned & processed dataset
│
├── src/
│ ├── 01_data_preprocessing.R # Missing value check, normalization, outlier treatment
│ ├── 02_feature_engineering.R # Feature creation and transformation
│ ├── 03_model_selection.R # Define models for regression & classification
│ ├── 04_model_training.R # Train & fine-tune models
│ ├── 05_model_evaluation.R # Evaluate model performance
│
├── results/
│ ├── figures/ # Plots & visualisations
│ ├── tables/ # Model metrics & summaries
│
├── reports/
│ ├── Assignment_1_Part_D_Report.pdf # Final report (compiled)
│ ├── Assignment_1_Part_D_Report.Rmd # R Markdown source
│
├── README.md


---

## **Requirements**

### **Option 1: Using R and RStudio**
You will need:
- R (≥ 4.2.0)
- RStudio
- Install required packages:
```r
install.packages(c(
  "tidyverse",
  "caret",
  "randomForest",
  "rpart",
  "pROC",
  "ggplot2",
  "knitr",
  "readr",
  "dplyr"
))

### **Option 2: Using Python** (optional, if Python scripts included)

You will need:
- Python (≥ 3.9)
- Recommended: Create a virtual environment before installing dependencies.

**Install dependencies**:
```bash
pip install -r requirements.txt


## **Setup Instructions**

Follow the steps below to replicate the analysis and generate the final report.

---

### **1. Clone the repository**
```bash
git clone https://github.com/Tran_Huu_Hao_Nguyen/Assignment-1-Part-D.git
cd Assignment-1-Part-D
2. Prepare the environment
Option A: Using R and RStudio (Recommended)
Requirements:

R (≥ 4.2.0)

RStudio

Install required R packages:

r
Copy
Edit
install.packages(c(
  "tidyverse",
  "caret",
  "randomForest",
  "rpart",
  "pROC",
  "ggplot2",
  "knitr",
  "readr",
  "dplyr"
))
Option B: Using Python (optional, if Python scripts are included)
Requirements:

Python (≥ 3.9)

Create and activate a virtual environment:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # MacOS/Linux
venv\Scripts\activate      # Windows
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
3. Place dataset
Ensure that the dataset file enhanced_student_habits_performance_dataset.csv is placed inside the data/ folder.

4. Run the pipeline
For R:
Execute the scripts in the src/ folder in the following order:

01_data_preprocessing.R – Missing value check, normalization, outlier treatment

02_feature_engineering.R – Feature creation and transformation

03_model_selection.R – Define regression and classification models

04_model_training.R – Train and fine-tune models

05_model_evaluation.R – Evaluate model performance

For Python (if available):
Run the corresponding .py scripts in numerical order inside the src/ folder.

5. Generate the final report
R:
r
Copy
Edit
rmarkdown::render("reports/Assignment 1_Part D_Comprehensive Final Report.Rmd")
Python:
Run Jupyter Notebooks or Python scripts to generate figures/tables, then compile them into your report format.

The compiled PDF or HTML will be saved in the reports/ folder.

Citation:

Nguyen, H.H. (2025). Student Habits and Academic Performance Prediction. University of Adelaide, Big Data Analysis Project.
