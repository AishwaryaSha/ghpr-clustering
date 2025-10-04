# Clustering GitHub Pull Requests and Error Logs

This project explores how we can **cluster GitHub pull request messages, commit data, and error logs** to identify recurring issues and patterns in codebases.  
The approach uses **TF-IDF, UMAP, and KMeans clustering** on PR titles, commit messages, and stack traces.

## Features
- Preprocess PR messages and error logs
- Generate embeddings using TF-IDF
- Dimensionality reduction with UMAP
- Clustering with KMeans
- Evaluation using silhouette and Davies-Bouldin scores
- Visualizations with Seaborn and Matplotlib

## Files
- `ghprdata.csv` - csv file for the dataset
- `ghpr_clustering.ipynb` – Jupyter notebook with cleaned code and analysis
- `requirements.txt` – Python dependencies

## Installation
Clone the repository and install requirements:

```bash
git clone https://github.com/<your-username>/ghpr-clustering.git
cd ghpr-clustering
pip install -r requirements.txt
