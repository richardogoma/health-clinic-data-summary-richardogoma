# Mini Project: Health Clinic Data Summary & Outlier Analysis

## Project Goal
This project aims to develop a data analysis pipeline for LifeCare Clinics. It ingests raw patient vital signs data from CSV files, cleans it, calculates statistical summaries (mean, median, mode), and automatically flags patients with irregular vitals (outliers) for immediate medical review. Outliers are categorized as 'High Risk' or 'Critical' based on the Interquartile Range (IQR) method.

## How to Run This Project

To execute this data analysis pipeline, follow these simple steps:

1.  **Open the Google Colab Notebook**: Ensure you have this notebook open in Google Colab.
2.  **Upload the Dataset**: Make sure the `patient_vitals.csv` file is uploaded to your Colab environment in the `/data/` directory, or update the `filepath` argument in the `generate_summary_report` and plotting cells to the correct path of your dataset.
    *   **Note**: If the dataset is not found, the `load_data` function will print an error.
3.  **Run All Cells**: Navigate to the `Runtime` menu in Colab and select `Run all`.
    *   Alternatively, you can run each cell individually from top to bottom.

## Project Output

Upon successful execution, the notebook will:

*   Load and process the patient vital signs data.
*   Generate a **Health Clinic Data Summary Report** for 'Heart Rate' and 'Temperature', including:
    *   Arithmetic Mean
    *   Median
    *   Mode
    *   Identified outliers, clearly stating the `Patient ID`, `Value`, and `Severity` ('High Risk' or 'Critical') for each.
*   Display a **histogram of Heart Rates** to visualize their distribution.

## Dataset Citation

The `patient_vitals.csv` dataset used in this project is a modified version of data from the following sources:

1.  **Abubaker Sherif, Wooi Haw Tan, Chee pun Ooi, & Yi Fei Tan. (2021). Five vital signs of normal people [Data set]. Zenodo. https://doi.org/10.5281/zenodo.5549632**
2.  **Adesina, Olumide (2024), “Blood pressure count data”, Mendeley Data, V1, doi: 10.17632/3xp4r3xsr5.1**
