# Spam Classifier Lab

## Introduction
Welcome to the Spam Classifier Lab! In this lab, you'll experience the entire data science pipeline, from data ingestion to deploying a lightweight Streamlit app. We'll be using a dataset of text messages and your goal will be to create an effective spam classifier. The lab will take you through data cleaning, exploratory data analysis, modeling, and visualization, culminating in an interactive Streamlit application where you can test your model's predictions on custom SMS messages.

## Lab Overview

1. **Data Ingestion**: Load a Pandas dataframe of text messages.
2. **Data Cleaning**: Investigate and address data quality issues.
3. **Exploratory Data Analysis**: Create visualizations to understand the distribution and characteristics of the data.
4. **Modeling**: Build a "steel thread" model using CountVectorizer and Multinomial Naive Bayes, followed by a more detailed modeling process employing a TF-IDF vectorizer, Random Forest, and Logistic Regression.
5. **Visualization**: Use Plotly and YellowBrick for advanced visualizations of the data and model performance.
6. **Streamlit App**: Build and deploy a lightweight app to interact with your spam classifier.

## Installation Instructions

### Setting Up Your Environment with Anaconda

1. **Download and Install Anaconda**
    - If you haven't installed Anaconda yet, download it from the [official website](https://www.anaconda.com/products/distribution).
    - Follow the installation instructions for your specific operating system.

2. **Create a New Conda Environment**
    - Open the Anaconda Command Prompt or terminal.
    - Run the following command to create a new environment named "spam_env":
      
```
conda create --name spam_env python=3.10
```
    
    - Activate the environment:

```
conda activate spam_env
```

4. **Install the Required Packages**
    - Attempt to install all necessary packages using `conda`:
  

```bash
conda install jupyterlab=4.0.4 pandas=2.0.3 numpy=1.25.2 pymongo=4.4.1 matplotlib=3.7.2 scikit-learn=1.3.0 ipython-autotime plotly=5.5.0 streamlit=1.25.0 yellowbrick=1.5
```

    - If any packages are not available or updated in the conda repositories, make a note of them. After the above command finishes, install those particular packages using `pip`. For example:

```bash
pip install package_name==version_number
```

5. **Launching JupyterLab**
    - With the environment activated (`conda activate spam_env`), you can start JupyterLab by running:

```bash
jupyter lab
```

6. **Note**: Always ensure you have the `spam_env` environment activated when working on this project. This ensures you're using the correct versions of libraries and dependencies.

## Getting Started

Once your environment is set up and you've activated it, navigate to the lab's notebook file and open it in JupyterLab to begin.

Happy coding!

## How to Submit Your Lab:
- Save Your Notebook: Make sure you've saved the latest version of your notebook. This can be done by clicking on the save icon or by pressing Ctrl + S (or Cmd + S on Mac).
- Check Your Outputs: Before submission, quickly review your notebook to ensure all outputs are clearly visible. This will help in the grading process as your outputs will demonstrate the results of your code.
- Save your notebook as `firstname lastname Spam Classification Lab.ipynb`. E.g., if I were submitting this assignment, my file would be `Sam Goodgame Spam Classification Lab.ipynb`. Navigate to the assignment page on Canvas for the Foundations of Data Science module and upload your .ipynb file.