# Penguin Species Clustering

## Project Description

This project was created to support ecological researchers in identifying penguin species in Antarctica using unsupervised machine learning. Due to missing species labels in the dataset, clustering techniques were used to uncover natural groupings based on penguin body measurements.

By applying **K-Means Clustering** and visualizing results using **Principal Component Analysis (PCA)**, the project successfully revealed three distinct clusters that likely correspond to the known native species: Adelie, Gentoo, and Chinstrap.

The project demonstrates skills in:
- Exploratory Data Analysis (EDA)
- Feature engineering and scaling
- Unsupervised machine learning (K-Means)
- Dimensionality reduction (PCA)
- Data storytelling through visualization

It also highlights the practical application of data science in solving real-world biological and environmental challenges.

---

## Dataset

- **Source**: Dr. Kristen Gorman and the Palmer Station, Antarctica LTER
- **Access**: The CSV file (`penguins.csv`) is included in the `/data` folder.
- **Features Used**:
  - `culmen_length_mm`
  - `culmen_depth_mm`
  - `flipper_length_mm`
  - `body_mass_g`
  - `sex` (converted to numerical)

This dataset does not include species labels, which is why unsupervised learning was used to uncover natural clusters.

---

## Methods

- **Data Cleaning**: Removed missing values, converted categorical to numerical.
- **Standardization**: Used `StandardScaler` to normalize feature ranges.
- **K-Means Clustering**:
  - Applied Elbow Method to identify optimal `k` (expected: 3 species).
  - Clustered penguins into groups without using actual species labels.
- **PCA**: Reduced features to 2D for visual cluster separation.

---

## Visualizations

### Elbow Method for Optimal Clusters
![Elbow Method](images/elbow_method.png)

### PCA Cluster Plot
![PCA Clusters](images/cluster_visual.png)

---

## Key Insights

- Clear separation into 3 clusters aligns with the known number of penguin species.
- `Flipper length` and `body mass` played a major role in clustering.
- PCA visualization confirms distinct natural groupings.


## How to Run Locally

```bash
git clone https://github.com/yievia/penguin-species-clustering.git
cd penguin-species-clustering
pip install -r requirements.txt
jupyter notebook notebooks/penguin_clustering.ipynb
```
---

## Tools Used
Python
pandas, numpy
seaborn, matplotlib
scikit-learn (KMeans, PCA)
Jupyter Notebook


## License
This project is for educational and portfolio purposes.
