# 🚚 Graph-Based Logistics Optimizer (Truck Routes)

This project applies **Graph Theory** in Python to simulate and analyze the optimal delivery routes between **distribution centers and storage depots** using **Maximum Spanning Trees** and **shortest paths**. It is designed to process multiple "archipelagos" (island networks) from an input `.txt` file and visually display their optimized delivery paths.

---

## 📌 What This Project Does

- Reads and parses a graph structure from a `.txt` file input.
- Constructs a **graph for each archipelago** (group of islands and their connections).
- Calculates the **Maximum Spanning Tree (MST)** to ensure the strongest (most reliable) links between nodes.
- Computes **shortest paths** from warehouses (depots) to distribution centers.
- Visually plots each graph, its MST, and the final routes using **NetworkX** and **Matplotlib**.

---

## 🧾 Input Format (`.txt` file)

The project expects a text file with structured lines of integers. The sections include:

1. First line of each graph:
   ```
   N M S
   ```
   - `N` = number of nodes  
   - `M` = number of edges  
   - `S` = number of start-to-end routes (warehouse to depot)

2. Next `M` lines (edges with weight):
   ```
   node1 node2 weight
   ```

3. Next `S` lines (start and end nodes):
   ```
   start_node end_node
   ```

> You can repeat the above block to simulate multiple archipelagos in the same file.

---

## 📊 Features & Algorithms

- ✅ **Graph Construction** using `NetworkX`
- ✅ **Maximum Spanning Tree (MST)** for reliable routing
- ✅ **Shortest Path Calculation** with preserved strongest links
- ✅ **Custom visualization** with clear legends and edge weights
- ✅ **Multi-instance support** (handles multiple graphs in one file)

---

## 🛠️ Dependencies

Make sure you have Python installed, and then install the required packages:

```bash
pip install networkx matplotlib pandas
```

---

## ▶️ How to Run

1. Place your input file (e.g., `arquipelogo.txt`) in the same folder as the script.

2. Open and run the script:

```bash
python "Grafos Caminhão.py"
```

3. You will see console outputs and a sequence of graphs and optimal paths being plotted.

---

## 🖼️ Output Example

Each archipelago generates 3 visualizations:

- **Original Graph** with weighted edges
- **Maximum Spanning Tree**
- **Best Delivery Route** from warehouse to depot

Each delivery path highlights:
- The route in solid gray
- Non-used paths in dashed gray
- Start (warehouse) and end (depot) nodes in distinct colors

---

## 📁 File Organization

```
├── Grafos Caminhão.py       # Main script
├── arquipelogo.txt          # Input file (you must provide this)
```

---

> *“Efficient delivery starts with smart routes.”*

