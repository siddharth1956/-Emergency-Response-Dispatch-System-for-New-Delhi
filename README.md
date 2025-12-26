# 🚨 Emergency Response Dispatch System for New Delhi

**Optimizing Urban Emergency Services Using Data Structures and Algorithms**

---

## 📌 Project Overview

Rapid emergency response is a critical requirement in densely populated metropolitan cities like **New Delhi**, where traffic congestion, complex road networks, and limited emergency resources can significantly delay response times.  

This project presents a **Data Structures and Algorithms (DSA)–driven Emergency Response Dispatch System** that models the city as a graph and applies classical optimization algorithms to **minimize response time, prioritize critical incidents, and analyze infrastructure resilience**.

The system goes beyond simple distance-based routing by incorporating **traffic delays, incident severity, and resource constraints**, enabling smarter and more realistic dispatch decisions.

---

## 🎯 Key Objectives

- Model New Delhi’s road network using **graph data structures**
- Compute **fastest emergency routes**, not just shortest distances
- Prioritize incidents based on **severity**
- Optimize **resource allocation** when multiple emergencies occur
- Analyze city infrastructure using **graph analytics**
- Demonstrate real-world applications of **DSA concepts**

---
---

## 🛠️ Technologies & Tools Used

- **Programming Language:** Python
- **Libraries:** NetworkX, heapq, matplotlib
- **Concepts:**  
  - Graphs (Adjacency List)
  - Priority Queues (Heaps)
  - Greedy Algorithms
  - Dynamic Programming
  - Graph Traversals

---

## 🧠 Core Algorithms & Data Structures

| Component | Technique Used | Purpose |
|--------|---------------|--------|
| Graph Representation | Adjacency List | Efficient storage of sparse road networks |
| Shortest Path | Dijkstra’s Algorithm | Fastest route calculation |
| Connectivity Check | BFS / DFS | Identify isolated or disconnected areas |
| Incident Priority | Max-Heap | Handle high-severity cases first |
| Dispatch Optimization | Greedy + DP concepts | Resource allocation |
| Infrastructure Analysis | MST (Prim’s Algorithm) | Identify critical road segments |

---

## 🚀 Project Breakdown

### 🔹 Part 1: Network Modeling & Routing Engine

This part focuses on building a **digital twin of New Delhi’s road network**.

#### Features:
- City modeled as a **weighted undirected graph**
- Nodes represent:
  - Intersections
  - Hospitals
  - Fire stations
  - Landmarks
- Edges represent road segments

#### Dynamic Edge Weight Formula:
Weight = Distance (km) + λ × Traffic Delay (minutes)
Where `λ` is a normalization factor converting time delay into cost units.

#### Algorithms Used:
- **Dijkstra’s Algorithm** → Fastest path selection
- **BFS / DFS** → Connectivity & reachability analysis

📌 *Result:*  
The system intelligently avoids heavily congested roads even if they are geographically shorter.

---

### 🔹 Part 2: Dispatch Optimization & Infrastructure Analytics

This part focuses on **decision-making and optimization**.

#### 🔥 Emergency Triage System
- Incidents assigned **severity scores**
- A **Max-Heap (Priority Queue)** ensures:
  - Life-threatening cases are dispatched first
  - Lower-priority incidents wait if resources are limited

#### 🚑 Resource Allocation
- Models ambulance allocation as an **optimization problem**
- Inspired by **Dynamic Programming** (Knapsack / Activity Selection)
- Prevents greedy local decisions when global optimization is needed

#### 🛣️ Infrastructure Analysis (MST)
- Uses **Prim’s Algorithm**
- Identifies:
  - Critical corridors
  - Roads whose failure can disconnect the city
- Useful for **urban planning and disaster preparedness**

---

## 📊 Sample Simulation Result

**Incident:** Fire at Connaught Place  
**Available Stations:**  
- Station A (closer, heavy traffic)  
- Station B (farther, light traffic)

**Decision:**  
✔ System dispatches **Station B**, arriving **earlier despite longer distance**

📌 *Insight:* Traffic-aware routing altered dispatch decisions in ~40% of test cases compared to distance-only routing.

---

## ⚠️ Limitations

- Uses **static CSV data** (no live traffic API)
- Single-agent routing (one ambulance at a time)
- Turn penalties at intersections not modeled

---

## 🔮 Future Enhancements

- Real-time traffic integration (Google Maps API)
- Machine Learning–based traffic prediction
- Multi-agent routing optimization
- Mobile app interface for emergency responders

---

## 📄 Project Report

A detailed academic explanation of the system design, algorithms, and results is available here:

👉 **[Download Project Report (PDF)](Project_Report.pdf)**

---

## 🧑‍🎓 Author

**Siddharth Shetty**  
Bachelor of Engineering – Computer Engineering  
Mumbai University  
📅 December 2025

---

## 📚 References

- Cormen et al., *Introduction to Algorithms*, MIT Press
- NetworkX Official Documentation
- Dijkstra, E. W. (1959), *A Note on Two Problems in Connexion with Graphs*

---

## ⭐ Final Note

This project demonstrates how **theoretical DSA concepts** like graphs, heaps, and greedy algorithms can be transformed into **real-world, life-saving systems** for smart cities.

If you find this project useful, feel free to ⭐ the repository.
