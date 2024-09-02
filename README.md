# Tumor_Diagnosis

## Resume
This project focuses on the analysis of a breast cancer diagnostic dataset, available from the UCI Machine Learning Repository. The dataset comprises various features computed from digitized images of fine needle aspirate (FNA) of breast masses, particularly properties of cell nuclei. The goal is to identify the features that significantly correlate with the diagnosis of breast cancer (malignant vs benign) and use these features to build predictive models.

The analysis includes data cleaning, feature selection, feature engineering, and visualization. Correlation analysis and hypothesis testing are performed to identify key predictors. Finally, interaction and polynomial features are created to enhance the predictive power of the model.

## Project Structure
### Dataset
- UCI Machine Learning Repository
- UW CS FTP Server

### Features
- ID number
- Diagnosis (M = Malignant, B = Benign)
- Radius (mean of distances from the center to points on the perimeter)
- Texture (standard deviation of gray-scale values)
- Perimeter
- Area
- Smoothness (local variation in radius lengths)
- Compactness (perimeter² / area - 1.0)
- Concavity (severity of concave portions of the contour)
- Concave points (number of concave portions of the contour)
- Symmetry
- Fractal dimension ("coastline approximation" - 1)
- Additional engineered features (e.g., interaction and polynomial features)

### Data Processing
- Data preview (`df.head()`)
- Data information (`df.info()`)
- Checking for missing values
- Dropping unnecessary columns (ID, Unnamed: 32)
- Conversion of diagnosis to binary (M = 1, B = 0)

### Data Analysis
- Correlation analysis with diagnosis
- Identification of top correlated features
- Visualization (pair plots, heatmaps)
- Skewness analysis and transformation

### Feature Engineering
- Interaction features (e.g., radius_texture_interaction)
- Polynomial features (e.g., radius_mean^2)
- Correlation of new features with diagnosis

### Hypothesis Testing
- Null Hypothesis: No difference in mean radius_mean between malignant and benign tumors
- Result: Reject the null hypothesis, confirming radius_mean as a significant predictor

### Visualizations
- Correlation Graphs
- Pair Plots
- Scatter Plots
- Heatmaps
