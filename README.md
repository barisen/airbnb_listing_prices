# airbnb_listing_prices

THe training data consists of airbnb listing data from London. Dataset has both textual and non-text features.
In this notebook we conduct EDA, Feature Engineering, Training Benchmark Models, treating text_features and Training and Investigating Nerual Network models for text_features.
As well as finally training a final ensemble model and predicting the prices. 
This module has been created as a part of Final Task for ADAMS - Advanced Data Analytics for Management Support (SoSe 2023) offered by Humboldt University.

The Notebooks is separated in to separate section:
## Table of Contents

    1. Introduction
    2. Importing Libraries
    3. Data Import
    4. Getting to know Data
        4.1 Early Checks and Balances¶
        4.2 Ydata Profiling
        4.3 Data Sampling:
        4.4 Visualize Map Data
    5. Data Transformations
        5.1 Non-Text Data
            5.1.1 Date features
            5.1.2 Numeric features
            5.1.3 Categorical Features
            5.1.4 Binary Features
            5.1.5 Other Features: `Amenities`
            5.1.6 Location features `neighbourhood, zipcode, lat/long`
        5.2 Outlier Handling
        5.3 Scaling the numeric columns
        5.4 Cleaning the text features
    6. Target Distribution
    7. Final Data Preparation for Model Training
        7.1 Creating Embeddings for Text Features
        7.2 Seprate Embeddings for each Text Feature in to a Dict
        7.3 Stacking all Text Features in to 1 and Creating Embeddings¶
    8. Model Training
        8.1 Benchmark Models
            8.1.1 Linear Regression
            8.1.2 Linear Regression - Ridge Fit
            8.1.3 Random Forest
            8.1.4 XGBoost
        8.2 NLP + Neural Networks
            8.2.1 FNN
            8.2.1.1 Hyperparameter Tuning
            8.2.3 Final FNN
        8.3 RNN Architecture
            8.3.1 Simple GRU
            8.3.2 GRU with Glove
            8.3.3 Bi-directional GRU
        8.4 Commentary on the model comparison¶
        8.5 Adding Hyperparameter Tuning to Picked Model¶
        8.6 Stacked Model Approach
        8.7 Model with Separate Embedding Layers for Individual Text Features
        8.8 Working with Amenities column as a Embedding
        8.9 Final Comparison Of Models  
    9. Conclusion
    10. Predicting for the final test_data
        10.1 Preparing the Train_Data for Final Model
        10.2 Train & Predict with the Final Model
