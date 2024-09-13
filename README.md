# Bioinformatics Project: Machine Learning for Bioactivity Prediction

## Project Overview

This project is part of a multi-part series aimed at building a machine learning model from scratch to predict the biological activity of chemical compounds against a target protein. Specifically, the project focuses on predicting whether a compound has favorable biological activity against **Acetylcholinesterase**. The machine learning model will be deployed as a web app that can serve as a bioinformatics tool for users to predict bioactivity.

### Project Structure

This project is divided into multiple parts, with each video demonstrating different stages of the bioinformatics project lifecycle. The main focus is on **data collection, molecular descriptor calculation, exploratory data analysis (EDA), model building, and deployment of the machine learning model as a web app**.

### Part 1: Dataset Collection
- **Goal**: Collect a biological activity dataset.
- **Details**: Data was collected from the **ChEMBL database**, containing information on compounds tested for biological activity against a target protein or organism.
- **Outcome**: The dataset was pre-processed and ready for use in data science and machine learning tasks.

### Part 2: Molecular Descriptor Calculation and Exploratory Data Analysis (EDA)
- **Goal**: Calculate Lipinski descriptors and perform EDA.
- **Details**: **Lipinski descriptors** (proposed by Christopher Lipinski) were calculated to predict the likelihood of compounds being drug-like molecules. 
- **EDA**: Simple **box plots** and **scatter plots** were created to discern differences between active and inactive sets of compounds.
- **Outcome**: EDA provided insights into the structure and behavior of the dataset, which helped in preparing for model building.

### Part 3: Target Protein Selection and Dataset Preparation
- **Goal**: Modify the target protein and compute molecular descriptors.
- **Details**: The target protein was switched to **Acetylcholinesterase**, allowing for a larger dataset. **PADEL-Descriptor software** was used to compute molecular descriptors, and the dataset was prepared (split into X and Y dataframes) for model building.
- **Outcome**: The dataset was now ready for model training with computed descriptors.

### Part 4: Building Regression Models
- **Goal**: Use molecular descriptors to build regression models.
- **Details**: The computed molecular descriptors (X variables) were used to predict **pIC50 values** (Y variable) through regression modeling.
- **Outcome**: A basic regression model was created to predict the bioactivity of compounds based on the molecular descriptors.

### Part 5: Comparing Multiple Regression Models
- **Goal**: Build and compare multiple regression models for Acetylcholinesterase inhibitors.
- **Details**: Several **Quantitative Structure-Activity Relationship (QSAR)** models were built using the **lazypredict library** in Python, allowing for easy comparison of different regression models.
- **Outcome**: The best-performing model was selected for further refinement and deployment.

### Part 6: Deploying the Model as a Web App
- **Goal**: Deploy the machine learning model as a web app.
- **Details**: The web app was created to allow users to input a compound of interest and predict its likelihood of having favorable biological activity against Acetylcholinesterase. 
- **Outcome**: The bioinformatics tool is accessible as a web app, enabling easy use by researchers for drug discovery.

---

## Key Features

- **Data Collection**: Extracted bioactivity data from the ChEMBL database.
- **Descriptor Calculation**: Calculated **Lipinski descriptors** and other molecular descriptors using **PADEL-Descriptor software**.
- **Exploratory Data Analysis (EDA)**: Performed EDA using box plots and scatter plots to analyze active and inactive compounds.
- **Model Building**: Built several regression models to predict bioactivity and compared their performance using **lazypredict**.
- **Web App Deployment**: Deployed the final machine learning model as a user-friendly web app for predicting compound bioactivity.

## Tools and Libraries

- **Python**: Programming language for data manipulation and model building.
- **Pandas**: For handling datasets and creating dataframes.
- **Matplotlib/Seaborn**: For visualizations (box plots, scatter plots, etc.).
- **PADEL-Descriptor**: For computing molecular descriptors.
- **lazypredict**: To quickly build and compare machine learning models.
- **Flask/Streamlit**: For deploying the model as a web app.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/bioinformatics-project.git
