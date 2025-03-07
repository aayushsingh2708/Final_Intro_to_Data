# Laptop Price Prediction & Income Classification

## Introduction
This repository contains two Jupyter Notebooks that apply machine learning techniques to different datasets:

1. **Laptop Price Prediction (Regression)**: Predicts the price of a laptop based on various features such as brand, processor, and GPU.
2. **Income Classification (Classification)**: Predicts whether an individual earns more than $50K annually based on demographic and occupational data.

## Dataset Information
### Laptop Price Dataset
- Contains details about different laptop models, including brand, processor, storage, GPU, and resolution.
- Target variable: **Price ($)** (continuous variable for regression).

### Adult Income Dataset
- A well-known dataset for classification, where features like age, education, and work class are used to predict whether a person earns **more or less than $50K per year**.
- Target variable: **Income** (`<=50K` or `>50K`).

## Project Structure
```
├── Regression_Laptop_Price.ipynb  # Notebook for predicting laptop prices
├── Classification_Income.ipynb     # Notebook for classifying income levels
├── data/                           # Folder containing datasets
├── README.md                       # Project documentation
└── requirements.txt                 # Required Python libraries
```

## Installation & Usage
### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/laptop-income-ml.git
cd laptop-income-ml
```

### 2. Create a Virtual Environment (Optional but Recommended)
```sh
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```sh
pip install -r requirements.txt
```

### 4. Run the Jupyter Notebook
```sh
jupyter notebook
```
- Open **Regression_Laptop_Price.ipynb** to explore laptop price prediction.
- Open **Classification_Income.ipynb** to analyze and predict income classification.

## Machine Learning Models & Results
### 1. Laptop Price Prediction (Regression)
- **Model**: Linear Regression
- **Performance Metrics**:
  - **R² Score**: 0.9316
  - **Mean Absolute Error (MAE)**: $230.50
  - **Root Mean Squared Error (RMSE)**: $295.79

### 2. Income Classification (Classification)
- **Models**: Logistic Regression & K-Nearest Neighbors (KNN)
- **Performance**:
  - **Logistic Regression Accuracy**: ~82%
  - **KNN Accuracy**: ~83%
  - **KNN outperformed Logistic Regression** in recall, making it better at identifying high-income individuals.

## Key Insights
- **One-Hot Encoding & Feature Scaling** were critical in improving model performance.
- **Linear Regression worked well for laptop price prediction**, capturing 93% of variance in price.
- **KNN showed better recall than Logistic Regression** for income classification, making it preferable when capturing high-income individuals is a priority.

## Links
- Dataset sources:
  - [Laptop Dataset](https://example.com/laptop-dataset)
  - [Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult)
- Jupyter Notebooks:
  - [Regression Notebook](https://github.com/yourusername/laptop-income-ml/blob/main/Regression_Laptop_Price.ipynb)
  - [Classification Notebook](https://github.com/yourusername/laptop-income-ml/blob/main/Classification_Income.ipynb)

---
🚀 **Contributions & Issues**
Feel free to open issues or contribute improvements to this project!

📧 **Contact**
For questions or feedback, reach out via GitHub or email.
