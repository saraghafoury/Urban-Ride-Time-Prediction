# Urban Ride Time Prediction

**Course:** Data Mining

## Team Members

- **Mobina kaksar**
- **Sara Ghafoury**

---

## Project Overview

This project focuses on predicting the duration of urban ride trips using data mining and machine learning techniques. The goal is to analyze ride information, perform data preprocessing, engineer useful features, and build predictive models for estimating trip duration.

The target variable is **`elapsed_seconds`**, which represents the total trip duration in seconds.

---

## Dataset

The dataset contains completed ride records with the following features:

| Feature | Description |
|---------|-------------|
| `record_key` | Unique trip identifier |
| `carrier_code` | Service provider |
| `start_time` | Trip start timestamp |
| `end_time` | Trip end timestamp |
| `rider_total` | Number of passengers |
| `start_xcoord`, `start_ycoord` | Pickup coordinates |
| `end_xcoord`, `end_ycoord` | Dropoff coordinates |
| `save_forward_marker` | Data storage indicator |
| `elapsed_seconds` | **Target variable** |

> **Note:** The original dataset is not included in this repository because of its size.

---

## Project Workflow

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Model Training
- Model Evaluation

---

## Data Cleaning

The following preprocessing steps were performed:

- Handling missing values
- Removing duplicate records
- Validating coordinate values
- Handling invalid passenger counts
- Detecting and removing outliers using the IQR method
- Calculating trip distance
- Detecting unrealistic travel speeds

---

## Feature Engineering

New features were generated, including:

- Start hour
- Day of week
- Month
- Weekend indicator
- Rush hour indicator
- Haversine distance
- Manhattan distance
- Encoded categorical variables

---

## Repository Structure

```text
Urban-Ride-Time-Prediction/
│
├── data/
│   ├── student_vesion.csv
│   └── ...
│
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── Feature_Engineering.ipynb
│   ├── EDA.ipynb
│   └── Model_Training.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/saraghafoury/Urban-Ride-Time-Prediction.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Author

This project was developed as part of the **Data Mining** course.