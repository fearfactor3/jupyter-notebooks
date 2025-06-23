# Jira Issues Data Analysis

A Jupyter notebook project for analyzing and sorting Jira issues data. This project provides tools to load, analyze, and export Jira issues data sorted by different categories.

## 📊 Project Overview

This repository contains a Jupyter notebook that demonstrates how to:

- Load Jira issues data from CSV files
- Sort issues by different categories (Type, Priority, Status)
- Export sorted results to Excel spreadsheets for further analysis

## 🚀 Features

- **Data Loading**: Read Jira issues from CSV format
- **Multi-Category Sorting**: Sort issues by:
  - Issue Type (Bug, Story, Task, etc.)
  - Priority (High, Medium, Low)
  - Status (In Progress, To Do, In Review, etc.)
- **Excel Export**: Export sorted data to Excel workbook with separate sheets for each category
- **Sample Data**: Includes sample Jira issues data for testing and demonstration

## 🛠️ Setup and Installation

### Prerequisites

- Python 3.7+
- pip package manager

### Installation Steps

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd jupyter-notebooks
   ```

2. **Install required packages**

   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

4. **Open the notebook**

   - Navigate to `sort_jira_issues_notebook.ipynb`
   - Run all cells to see the analysis in action

## 📋 Dependencies

- **pandas** (2.2.3): Data manipulation and analysis
- **xlsxwriter** (3.2.0): Excel file creation and formatting

## 🔧 Usage

### Using the Sample Data

The notebook comes with sample Jira issues data (`sample_jira_issues.csv`) that includes:

- Issue Key
- Summary
- Issue Type
- Priority
- Status
- Assignee
- Reporter
- Created/Updated dates
- Due Date

### Using Your Own Data

To use your own Jira data:

1. Export your Jira issues to CSV format
2. Replace `sample_jira_issues.csv` with your data file
3. Update the `file_path` variable in the notebook if needed
4. Ensure your CSV has the required columns: `Issue Type`, `Priority`, `Status`

### Output

The notebook generates:

- Sorted DataFrames displayed in the notebook
- Excel file (`sorted_jira_issues_by_status.xlsx`) with three sheets:
  - **Sorted by Priority**: Issues ordered by priority level
  - **Sorted by Status**: Issues grouped by current status
  - **Sorted by Type**: Issues categorized by issue type
