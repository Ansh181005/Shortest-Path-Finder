# Shortest Path Finder

A visual, interactive tool for finding the shortest path between nodes in a graph using Dijkstra's algorithm. Built with pure HTML, CSS, and JavaScript.

## Features

- **Dual Graph Creation Modes**
  - **User-Created**: Manually build custom graphs by adding edges between nodes
  - **Random**: Automatically generate connected random graphs

- **Interactive Visualization**
  - Canvas-based graph rendering
  - Circular node layout for optimal visibility
  - Visual path highlighting in real-time
  - Color-coded nodes (blue for start, red for end, green for path)

- **Dijkstra's Algorithm**
  - Finds shortest path between any two nodes
  - Displays total distance
  - Shows complete path route

- **Edge Management**
  - Add custom weighted edges
  - Remove edges dynamically
  - Real-time edge list display

## How to Use

1. **Setup**
   - Enter the number of nodes (2-20)
   - Choose graph type (User-Created or Random)
   - Click "Create Graph"

2. **For User-Created Graphs**
   - Use the edge controls to add connections
   - Select "From Node" and "To Node"
   - Enter edge weight (distance)
   - Click "Add Edge"

3. **Find Shortest Path**
   - Select start node from dropdown
   - Select end node from dropdown
   - Click "Find Shortest Path"
   - View the highlighted path and total distance

4. **Reset**
   - Click "Reset" to clear the graph and start over

## Technical Details

### Algorithm
- **Dijkstra's Algorithm**: Guarantees the shortest path in weighted graphs with non-negative edge weights
- **Time Complexity**: O(V²) where V is the number of vertices
- **Space Complexity**: O(V)

### Graph Representation
- Adjacency matrix for storing edge weights
- Undirected graph (bidirectional edges)
- Nodes arranged in circular layout for visualization

### Key Components

**Graph Class** (index.html:285-425)
- `generateRandomGraph()`: Creates random connected graphs
- `addEdge()`: Adds weighted edges between nodes
- `dijkstra()`: Implements shortest path algorithm
- `ensureConnected()`: Guarantees graph connectivity

**Visualization**
- HTML5 Canvas API
- Dynamic node positioning
- Real-time path highlighting
- Weight labels on edges

## Installation & Running

No installation or build process required!

1. Clone or download the repository
2. Open `index.html` in any modern web browser
3. Start creating graphs and finding paths

```bash
# Simply open the file
open index.html
# or
start index.html
# or double-click the file
