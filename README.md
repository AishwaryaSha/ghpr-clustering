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


## Dataset

This project uses the dataset from the paper:

> Jiaxi Xu, Fei Wang, Jun Ai.  
> *Defect Prediction With Semantics and Context Features of Codes Based on Graph Representation Learning*.  
> IEEE Transactions on Reliability, 2021.  

📖 If you use this dataset, please cite their paper:

@ARTICLE{xu2021defect,
author={Jiaxi Xu and Fei Wang and Jun Ai},
journal={IEEE Transactions on Reliability},
title={Defect Prediction With Semantics and Context Features of Codes Based on Graph Representation Learning},
year={2021}
}


You can download the dataset directly from their repository:  
[GHPR_dataset on GitHub](https://github.com/feiwww/GHPR_dataset)

After downloading, place `ghprdata.csv` in the root of this project folder before running the notebook.
