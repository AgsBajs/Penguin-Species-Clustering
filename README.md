# Penguin Clustering Project

## Overview
This project applies K-Means clustering to the Palmer Penguins dataset to find natural groupings of penguins based on their physical measurements. The goal is not to predict species labels, but to explore how penguins can be grouped by body traits such as beak length, depth, flipper size, and body mass.

The project walks through data mapping, cleaning, preprocessing, visualization, and model creation. It concludes with insights about cluster patterns and biological interpretation.

---

## Dataset
The dataset used in this project was obtained from Kaggle:  
**Youssef Aboelwafa — Clustering Penguins Species**  
[https://www.kaggle.com/datasets/youssefaboelwafa/clustering-penguins-species](https://www.kaggle.com/datasets/youssefaboelwafa/clustering-penguins-species)

This dataset contains measurements of penguins including:
- culmen_length_mm – Length of the beak (culmen)  
- culmen_depth_mm – Depth (thickness) of the beak  
- flipper_length_mm – Length of the flipper  
- body_mass_g – Body mass in grams  
- sex – Male or Female

---

## Steps in the Project

1. **Mapping the Original Data**
   - Loaded and explored the dataset using pandas.  
   - Checked for missing or inconsistent values using `.info()` and `.describe()`.

2. **Data Exploration and Visualization**
   - Plotted histograms and scatter plots to view the spread and relationships between measurements.  
   - Observed that body mass and flipper length are positively correlated, while culmen depth varies more independently.

3. **Preprocessing**
   - Dropped missing values.  
   - Standardized numerical features using StandardScaler so each measurement contributes equally to the clustering process.

4. **K-Means Clustering**
   - Applied K-Means with k = 3.  
   - Added cluster labels to the dataset and calculated cluster centers.  
   - Visualized the clusters using scatter plots to confirm clear group separation.

5. **Additional Visualizations**
   - Created a correlation heatmap to identify relationships between features.  
   - Used PCA (Principal Component Analysis) to visualize the clusters in 2D.  
   - Added boxplots by cluster to highlight how physical traits differ among clusters.

6. **Results and Insights**
   - Three distinct clusters were formed, likely representing different species or body size groups.  
   - The model successfully grouped penguins with similar body characteristics.  
   - Identified that data cleaning and scaling are crucial for meaningful clustering results.

---

## Technologies Used
- Python  
- Pandas  
- Matplotlib  
- Scikit-learn

---

## Reference
Youssef Aboelwafa. *Clustering Penguins Species.* Kaggle, 2023.  
[https://www.kaggle.com/datasets/youssefaboelwafa/clustering-penguins-species](https://www.kaggle.com/datasets/youssefaboelwafa/clustering-penguins-species)
