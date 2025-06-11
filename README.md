# Penguin Species Clustering

This project uses unsupervised machine learning to identify natural groupings of penguins in Antarctica based on their physical characteristics. The analysis was done using **K-Means clustering** and visualized through **PCA**.

---

## Dataset

- **Source**: Dr. Kristen Gorman and the Palmer Station, Antarctica LTER
- **File**: `penguins.csv`
- **Features Used**:
  - `culmen_length_mm`
  - `culmen_depth_mm`
  - `flipper_length_mm`
  - `body_mass_g`
  - `sex` (converted to numerical)

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
git clone https://github.com/yourusername/penguin-species-clustering.git
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
