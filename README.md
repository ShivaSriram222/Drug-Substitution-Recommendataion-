### Drug Substitution Recommendation System
## Overview

This project builds a machine learning-based recommendation system that suggests safer drug alternatives based on ingredients, adverse events, and warning labels. It leverages text mining, dimensionality reduction, clustering, and supervised learning to analyze over 100,000+ drug records from the openFDA API.

## Key Features

Scrapes and preprocesses real-world drug data from openFDA.

Extracts text features from drug warnings using TF-IDF.

Applies PCA to reduce dimensionality by 70% while retaining 85% variance.

Clusters drugs using hierarchical clustering with 83% accuracy.

Uses Random Forest to predict safer substitutions with 92% accuracy.

Provides a framework for safer prescription and regulatory insights.

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

Machine Learning Methods: TF-IDF, PCA, Hierarchical Clustering, Random Forest

Data Source: openFDA API (https://open.fda.gov/apis/
)

## Project Structure

data/  
    Before_cleaning_drug_event_data.csv  
    Before_cleaning_drug_ndc_data.csv  
    After_Cleaning.csv  

notebooks/  
    DrugRecommendationSystem_Module1.ipynb  
    DrugRecommendationSystem_Module2.ipynb  
    DrugSubstitutionSystem_Module3.ipynb   
    Drug_Substitution_Final.ipynb     <-- (clean combined notebook)

requirements.txt
README.md


## Results

Clustering Accuracy: ~83%

Prediction Accuracy (Random Forest): ~92%

Dimensionality Reduction: 70% reduction with 85% variance retention

(Add plots or visualizations screenshots here, such as PCA clusters and Random Forest feature importance.)

## Future Work

Use transformer embeddings for richer drug text representations.

Deploy as a Streamlit or Gradio web app for real-time substitution recommendations.

Extend to multilingual drug warnings and global FDA-equivalent datasets.

