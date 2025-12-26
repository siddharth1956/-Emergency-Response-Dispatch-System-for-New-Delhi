# 🚨 Emergency Response Dispatch System for New Delhi  
### Part 1 – Emergency Network Modelling & Core DSA Algorithms

## 📌 Project Overview
This project models the city of **New Delhi** as a **weighted graph** to simulate an
emergency response network. The goal of **Part-1** is to apply **core Data Structures
and Algorithms (DSA)** concepts such as **Graphs, BFS, DFS, Hashing, and Dijkstra’s
Algorithm** to analyze city connectivity and compute shortest emergency routes.

The implementation is done using **Python** in a **Google Colab / Jupyter Notebook**
environment.

---

## 🎯 Objective (Part-1)
- Load and preprocess real-world city data using Pandas
- Model locations and roads as a weighted undirected graph
- Analyze connectivity using BFS and DFS
- Compute shortest paths using Dijkstra’s algorithm
- Enable fast searching using hashing
- Visualize the city network and shortest routes

---

## 📂 Dataset Description
The project uses the following CSV files:

| File Name | Description |
|---------|-------------|
| `locations.csv` | City locations (nodes) with latitude, longitude, and category |
| `roads.csv` | Roads (edges) with distance and traffic delay |
| `emergencies_facilities.csv` | Emergency facilities metadata (used in Part-2) |
| `incidents_sample.csv` | Sample emergency incidents (used in Part-2) |

---

## 🛠️ Technologies Used
- **Python 3**
- **Pandas** – Data loading and preprocessing
- **NetworkX** – Graph construction and algorithms
- **Matplotlib** – Graph visualization
- **Google Colab / Jupyter Notebook**

---

## ⚙️ How to Run the Project

### Option 1: Google Colab (Recommended)
1. Open https://colab.research.google.com
2. Upload the notebook `Emergency_Dispatch_Part1.ipynb`
3. Upload all CSV files when prompted:
   - `locations.csv`
   - `roads.csv`
   - `emergencies_facilities.csv`
   - `incidents_sample.csv`
4. Run all cells from top to bottom

---

### Option 2: Local Jupyter Notebook
1. Install required libraries:
   ```bash
   pip install pandas networkx matplotlib
## Part 2 – Emergency Dispatch Optimization & Analysis
Part 2 extends the system with emergency facility mapping, incident routing,
priority-based dispatch using queues and heaps, Minimum Spanning Tree (MST)
analysis, sorting-based analytics, and enhanced visualizations.
