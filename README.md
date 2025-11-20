# BPPSO_EX1

This repository performs basic analysis of the event log issued at the BPI challenge 2017.

## General Purpose

The main goal of this project is to apply core process mining and data science techniques to a real-world event log—the BPIC-17 loan application dataset from a Dutch financial institution. The analysis covers the following objectives:

1.  **Process Discovery:** Analyzing the event log to derive a comprehensive Business Process Model and Notation (BPMN) diagram.
2.  **Statistical Analysis:** Generating fundamental statistics to characterize the event log's key features, such as trace length, process duration, and most common loan goals.
3.  **Advanced Data Analysis:** Investigating the relationship between trace length and process time using regression and applying k-means clustering to segment process instances based on time/length and event presence.

## Repository Structure

The project is structured around the main analysis sections of the accompanying report.

| File/Folder | Section in Report | Description |
| :--- | :--- | :--- |
| `2.2.Basic_Analysis.ipynb` | Section 2.2 | Basic statistical analysis, including event log characteristics and frequency distributions. |
| `2.3.Process_Model.ipynb` | Section 2.3 | Deriving and analysing the process model from the event log. |
| `2.4.1.Linear_Regression.ipynb`| Section 2.4.1 | Analysis of the relationship between trace length and time needed using linear regression and outlier detection. |
| `2.4.2.Clustering.ipynb` | Section 2.4.2 | Advanced analysis using k-means clustering (based on time/length and bag-of-activities) and Principal Component Analysis (PCA). |
| `BPIC-17_ProcessModel.bpmn` | Section 2.3.4 | The final, manually refined BPMN model derived from the process mining results. |
| `figures/` | Figures in Report | Directory to store all generated plots and process models from the notebooks. |
| `requirements.txt` | Section 2.1 | List of required Python libraries for the analysis. |

## How to Run the Analysis

Follow these steps to set up the environment and run the analysis notebooks.

### 1. Setup Virtual Environment

It is highly recommended to use a virtual environment to manage dependencies.

```bash
# Create a new virtual environment
python3 -m venv venv

# Activate the virtual environment
source venv/bin/activate  # On Linux/macOS
# .\venv\Scripts\activate  # On Windows PowerShell
```
### 2. Include XES File
The XES-File of the BPI-2017 Challenge is not uploaded in the Git repository, but has to be manually uploaded to the local workspace. Further potential file paths, especially for reading the log, but also to save certain figures, needs to be updated manually. 
