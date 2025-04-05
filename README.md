# TSP Solver Comparison: Christofides vs Ant Colony Optimization 🧭🐜

This project implements and compares two algorithms for solving the Traveling Salesman Problem (TSP):
- **Christofides Algorithm** – A graph-theoretic approximation with guaranteed performance.
- **Ant Colony Optimization (ACO)** – A probabilistic heuristic inspired by nature.

The algorithms were tested on both synthetic data and a real-world dataset of U.S. cities.

---

## 📌 Features

- Compare TSP solutions across:
  - Path quality (total distance)
  - Execution time
  - Visualization clarity
- Graph construction using MSTs and complete graphs
- Real-world distance calculations using the Haversine formula
- Interactive maps with Plotly for city-based paths

---

## 🛠 Technologies Used

- **Python 3**
- **Numpy / Pandas** – Data handling and matrices
- **NetworkX** – Graph construction and operations
- **Matplotlib** – Static plotting
- **Plotly Express + Graph Objects** – Interactive map visualization
- **Scipy** – Distance matrix calculations
- **Custom Haversine Logic** – For geo-coordinates

---

## 🔬 Algorithms

### ✅ Christofides Algorithm
- Constructs a **Minimum Spanning Tree (MST)**
- Matches nodes with odd degree for Eulerian tour
- Generates a near-optimal path with ≤1.5x optimal distance

### 🐜 Ant Colony Optimization (ACO)
- Uses **pheromone trails** and **heuristic desirability**
- Balances **exploration (randomness)** and **exploitation (best paths)**
- Allows dynamic tuning with parameters like `alpha`, `beta`, `decay`, and `ants`

---

## 🧪 Dataset

- **File**: `cities_usa.csv`
- **Columns**: `City`, `Latitude`, `Longitude`
- Used to calculate pairwise distances and plot actual map-based routes.

---

## 📊 Outputs

- Optimal Path (sequence of cities)
- Total Path Distance
- Execution Time
- Visualizations:
  - 📉 Static Graphs (Matplotlib)
  - 🗺️ Interactive Maps (Plotly)
