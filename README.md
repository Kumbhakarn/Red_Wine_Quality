# Red_Wine_Quality
  * Wine Quality classification is a difficult piece of work since taste is the least factor of the human senses. A good wine quality prediction can be very useful in the certification process. This project aims to determine which features are the best quality of red wine and generate insights into each of these attributes.

# Data Set Information
  * Wine Quality Data Set. This dataset is available on Kaggle repository
      https://www.kaggle.com/datasets/ruthgn/wine-quality-data-set-red-white-wine/download?datasetVersionNumber=2

  * This data set contains records related to red and white variants of the Portuguese Vinho Verde wine. It contains information from 1599 red wine samples and 4898 white wine samples. Input variables in the data set consist of the type of wine (either red or white wine) and metrics from objective tests (e.g. acidity levels, PH values, ABV, etc.), while the target/output variable is a numerical score based on sensory data—median of at least 3 evaluations made by wine experts. Each expert graded the wine quality between 0 (very bad) and 10 (very excellent). Due to privacy and logistic issues, there is no data about grape types, wine brand, and wine selling price.
  * This data set is a combined version of the two separate files (distinct red and white wine data sets) originally shared in the UCI Machine Learning Repository.

   <a id='top'></a>
<div class="list-group" id="list-tab" role="tablist">
<p style="background-color:#4a8fdd;font-family:newtimeroman;color:#FFF9ED;font-size:200%;text-align:center;border-radius:9px 9px;">TABLE OF CONTENTS</p>   
    
* [1. INTRODUCTION](#1)
    
* [2. IMPORTING NECESSARY LIBRARIES](#2)
    
* [3. LOADING DATASET](#3)
    
* [4. INITIAL INFORMATION ABOUT DATASET](#4)
    
    * [4.1. Get Initial Information](#4.1)    
    * [4.2. Descriptive Statistics of Numeric Variables](#4.2)    
    * [4.3. Pandas Profiling](#4.3)    
    * [4.4. Check null Values](#4.4)
    * [4.5. Rename Column Names](#4.5) 
    
    
* [5. DATA VISUALIZATION](#5)
    
    * [5.1. Histplot](#5.1)    
    * [5.2. Pairplot](#5.2)    
    * [5.3. Scatterplot](#5.3)    
    * [5.4. Smooth Kernel Density with Marginal Histograms](#5.4)
    * [5.5. Regplot](#5.5)
    * [5.6. Hexagonal Binned Plot](#5.6)
    * [5.7. Visualization with Plotly Express](#5.7)
    * [5.8. Heatmap and Correlation](#5.8)
    
    
    
* [6. DATASET PREPROCESSİNG](#6)
    
    * [6.1. Look at Dataset](#6.1)    
    * [6.2. Divide Quality Range into 2 Parts](#6.2)    
    * [6.3. Look at Dataset (with changed 'quality' variable)](#6.3)    
    * [6.4. Select Dependent and Independent Variables](#6.4)
    * [6.5. Split Dataset into Train and Test Sets](#6.5)
    * [6.6. Standardization](#6.6)    

    
    
* [7. BUİLDİNG CLASSİFİCATİON MODELS](#7)
    
    * [7.1. K-Nearest Neighbors (KNN) Model](#7.1)    
    * [7.2. Hyperparameter Tuning for KNN Model](#7.2)    
    * [7.3. Get Best Parameters of KNN Model](#7.3)    
    * [7.4. Build KNN Model with Best Parameters](#7.4)
    * [7.5. Accuracy Score of KNN Model on Test set](#7.5)
    * [7.6. Classification Report of KNN Model](#7.6)    
    * [7.7. Gradient Boosting Machines (GBM) Model](#7.7)     
    * [7.8. Hyperparameter Tuning for GBM Model](#7.8)    
    * [7.9. Get Best Parameters of GBM Model](#7.9)    
    * [7.10. Build GBM Model with Best Parameters](#7.10)   
    * [7.11. Accuracy Score of GBM Model on Test set](#7.11)    
    * [7.12. Classification Report of GBM Model](#7.12)    
    * [7.13. Light GBM Model](#7.13)    
    * [7.14. Hyperparameter Tuning for Light GBM Model](#7.14)    
    * [7.15. Get Best Parameters of Light GBM Model](#7.15)   
    * [7.16. Build Light GBM Model with Best Parameters](#7.16)    
    * [7.17. Accuracy Score of Light GBM Model on Test set](#7.17)    
    * [7.18. Classification Report of Light GBM Model](#7.18)    
    * [7.19. ROC AUC - Light GBM Model](#7.19)
    
    
### Requirements

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [VS Code](https://code.visualstudio.com/)
