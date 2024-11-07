Here is an enhanced version of the README for your **DijkstraOnMaps** project:

---

# DijkstraOnMaps

## Project Overview

**DijkstraOnMaps** is an implementation of **Dijkstra's Algorithm** to find the shortest path between nodes on a map. The map is imported from OpenStreetMap (OSM), a free and open service, and the data is used to generate a pathfinding solution on the map.

### Key Features

- **Shortest Path Calculation**: Using Dijkstra’s Algorithm to compute the shortest path.
- **Map Integration**: Uses real-world map data exported from OpenStreetMap (OSM).
- **Interactive Interface**: Allows users to select a source node and destination from a map via a web browser interface.

## Project Details

### Map Data
- The map is taken from **OpenStreetMap** and exported in `.osm` format, which is then processed and used in the program.
- **Nodes x Nodes adjacency matrix**: The connections between nodes are stored in an adjacency matrix, where each cell represents a direct connection between two nodes.

### Algorithm
- **Dijkstra’s Algorithm** is used to find the shortest path between nodes in the map.

## Files

There are two primary files in the project:

1. **`.py` File**: This Python file can be compiled and run directly using any Python IDE.
2. **`.ipynb` File**: This Jupyter notebook can be opened and run in **Jupyter** or **Google Colab** to compile all the cells and visualize the results interactively.

## Functioning

### Step-by-step Flow

1. **Map Analysis**:
   - Upon compilation, the map data is analyzed, and all nodes are extracted and stored in a list.
   - An **adjacency matrix** is generated, mapping the connections between nodes.

2. **Source Node Selection**:
   - Initially, all nodes are considered as potential start points, and paths to other nodes are generated.
   - The program prompts the user to select a **source node**. An interactive map is opened in the browser where the source node is selected by clicking on a **green dot**.

   ![Map with Source Node](https://user-images.githubusercontent.com/53964760/129915134-56acd5a4-0209-4d7e-8f34-52aeac29196f.png)  
   *The green dots represent the nodes.*

3. **Destination Nodes Display**:
   - After selecting the source, a list of **destination nodes** is displayed as red dots on the map.
   
   ![Map with Destination Nodes](https://user-images.githubusercontent.com/53964760/129915357-cfc77779-ddec-4cd1-adf6-b4e1796228ae.png)  
   *The blue dot is the source, and red dots represent possible destinations.*

4. **Shortest Path Calculation**:
   - The user selects one of the destination nodes.
   - The shortest path between the source and destination is then calculated and displayed on the map.

   ![Shortest Path Display](https://user-images.githubusercontent.com/53964760/129915584-7b4f62ea-7da1-4051-9ae8-a86d113d7c62.png)  
   *The shortest path is highlighted on the map.*

5. **Console Output**:
   - The entire process, including data analysis, node selection, and shortest path finding, runs in the console when the `.py` file is executed.

   ![Console Output](https://user-images.githubusercontent.com/53964760/129915621-e269a227-e960-4538-8aa3-80231b991b52.png)  
   *Console output displaying the analysis and pathfinding progress.*

## How to Use

### Prerequisites

Ensure that you have the following installed:

- Python 3.x
- Required libraries: `networkx`, `numpy`, `matplotlib`, `osm`, `folium`, `requests` (for map interaction)

### Steps to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/DijkstraOnMaps.git
   cd DijkstraOnMaps
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Python script:
   ```bash
   python dijkstra_on_maps.py
   ```

4. Alternatively, open the **`.ipynb`** file in **Jupyter** or **Google Colab** and run the cells.

5. Follow the prompts in the console to select a source and destination node, and visualize the results in your browser.

## Demo

You can see the whole process in action by running the `.py` file or Jupyter notebook. It will:
- Open an interactive map for node selection.
- Calculate the shortest path and display it visually.

## Acknowledgments

- OpenStreetMap (OSM) for providing free map data.
- Dijkstra's Algorithm for optimizing pathfinding on the map.
- Python libraries: `networkx`, `numpy`, `folium`, and others for visualization and computation.

---

This README provides a detailed, clear, and professional explanation of your project, helping others understand and use it effectively!
