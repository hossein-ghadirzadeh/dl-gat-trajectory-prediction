# DL Assignment 2 – GAT for Pedestrian Trajectory Prediction

This repository contains the implementation and report for a deep learning assignment focused on trajectory prediction using Graph Attention Networks (GATs). The task is to forecast the future location of pedestrians based on their current position, movement, and spatial relations represented as a graph.

## Task Description

This project builds on concepts of Attention Mechanisms and Graph Neural Networks (GNNs). The goal is to predict the future (x, y) location of each pedestrian by modeling the scene as a graph, where each node represents a pedestrian and edges encode spatial relationships.

### Experiments

The following experiments were performed:

1. **Baseline GAT** — Standard GAT with 8 attention heads.
2. **Hyperparameter Tuning** — Compare performance using 1 and 4 heads, and apply deeper node embeddings.
3. **Custom Attention** — Replace the learnable attention mechanism with cosine similarity between node vectors.

## Repository Structure

- `notebook.ipynb` – Full pipeline, data processing, model building, training, and evaluation.
- `report.pdf` – Summary of experiments, visualizations, and discussion.
- `data/` – Raw pedestrian data (edges + nodes).
- `README.md` – This file.
- `.gitignore` - Ignores model checkpoints, etc.

> **Note:** The dataset consists of only one scene (two small files), so it is included in this repository for reproducibility.

## Required Libraries

Please ensure the following libraries are installed in your Python environment:

- `tensorflow`
- `matplotlib`
- `numpy`
- `pandas`
- `networkx`
- `spektral`

## How to Run

1. Install the dependencies:

```bash
pip install tensorflow numpy pandas matplotlib networkx spektral
```

2. Open notebook.ipynb using Jupyter Notebook, JupyterLab, or VS Code, and run all cells sequentially to reproduce the experiments.

## Evaluation

Performance was measured using Mean Squared Error (MSE) and Root Mean Squared Error (RMSE), corresponding to distance between predicted and actual (x, y) positions.

## Author

Arian Ghadirzadeh<br>
Deep Learning Course (TDIS22) – Assignment 2<br>
Jönköping University, School of Engineering (JTH)<br>
April 2025
