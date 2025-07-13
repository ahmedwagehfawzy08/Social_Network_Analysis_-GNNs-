```markdown
# 📊 Social Network Analysis with Python (NetworkX)

A Python project to model and analyze social relationships using graphs. It covers network creation, visualization, and centrality analysis using [NetworkX](https://networkx.org/), with both manual and real-data examples — including a dataset inspired by *Grey’s Anatomy* character interactions.

---

## 🚀 Project Goals

- Create and visualize social graphs using NetworkX.
- Perform centrality analysis (Degree, Betweenness, Eigenvector).
- Explore shortest paths, connected components, and clustering.
- Use real-world data (from CSV) to simulate character relationships.

---

## 🧰 Libraries Used

- `networkx` – for graph modeling and analysis  
- `matplotlib` – for plotting the network  
- `pandas` – for reading external datasets  
- `warnings` – to suppress unnecessary output

---

## 📁 Data

### Example 1: Manual Graph
Nodes and edges are manually added to simulate relationships between public figures:
- **Nodes**: Obama, Trump, Michelle, Hillary, etc.
- **Edges**: Represent interactions, debates, or associations.

### Example 2: Grey's Anatomy Dataset
`ga_edgelist.csv` is a CSV file with columns:
```csv
from,to
lexi,sloan
owen,yang
...
```
Each row represents a connection between characters.

---

## ⚙️ How to Run

1. **Clone the repo or download the script**:
```bash
git clone https://github.com/yourusername/social-network-analysis.git
```

2. **Install dependencies**:
```bash
pip install networkx matplotlib pandas
```

3. **Run the Python script**:
```bash
python social_network_analysis.py
```

Make sure the `ga_edgelist.csv` file is in the same folder if you want to run the Grey's Anatomy part.

---

## 🔍 Features & Analysis

- **Graph Creation**: Manual & from dataset  
- **Visualization**: Simple and full network plots with labels  
- **Centrality Metrics**:
  - Degree Centrality
  - Eigenvector Centrality
  - Betweenness Centrality
- **Clustering**:
  - Individual node clustering
  - Average clustering across the network
- **Connected Components**
- **Shortest Paths Between Nodes**
- **Subnetwork Extraction (BFS Tree)**

---

## 📊 Example Output

**Obama's neighbors**: Michelle, Trump, Clinton, Mitt  
**Shortest path from Mitt to Ivanka**: `['Mitt', 'Obama', 'Trump', 'Ivanka']`  
**Most central in Grey’s Anatomy graph**: Karev (by degree centrality)

---

## 📈 Visualizations

- Draw networks using `nx.draw_networkx()`  
- Customize size, labels, and layout  
- Highlight subgroups with `bfs_tree` and connected components

---

## 💡 Future Ideas

- Interactive web interface with Streamlit or Flask  
- Export visualizations to image/PDF  
- Apply community detection algorithms (Louvain, etc.)  
- Use dynamic/temporal networks
