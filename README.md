# DFS · Topological Sort · Cycle Detection Visualizer
### A High-Fidelity, Zero-Dependency Algorithmic Explorer

A 100% self-contained, interactive tool built to visualize the mechanics of **Depth-First Search (DFS)**, **Topological Sorting**, and **Cycle Detection** in directed graphs.

---

## 🚀 The "Vanilla" Challenge
This project was built under strict architectural constraints to ensure a deep understanding of the DOM, SVG manipulation, and core algorithms:
* **0 External Libraries:** No React, No D3.js, No jQuery, No Bootstrap.
* **100% Offline Capable:** Works with no internet connection; all logic, styles, and structures are contained within a single HTML file.
* **Native Technologies:** Built using only **HTML5**, **CSS3 (Custom Properties & Animations)**, **Vanilla JavaScript (ES6+)**, and **SVG**.

---

## Algorithmic Features
This tool doesn't just show nodes changing colors; it visualizes the mathematical metadata generated during a DFS traversal:

* **Step-by-Step Execution:** Line-by-line pseudocode tracking that syncs with the visual graph state.
* **Edge Classification:** Real-time detection and labeling of **Tree**, **Back**, **Forward**, and **Cross** edges.
* **Parenthesis Theorem:** A dedicated SVG timeline visualizing the nesting property of discovery ($d[u]$) and finish ($f[u]$) times.
* **Topological Sort:** Interactive generation of linear ordering based on finish-time descending order.
* **Cycle Detection:** Automatic flagging of back-edges that violate the Directed Acyclic Graph (DAG) property.
* **DP on DAGs:** A module exploring the "Longest Path" problem using DFS-based Dynamic Programming.

---

## Technical Implementation
### SVG Engine
The graph is rendered using a custom-built SVG coordinate system. Nodes and edges are manipulated directly via the DOM API, using `requestAnimationFrame` for smooth, high-performance transitions.

### State Machine
The visualizer uses a step-buffer system. When a graph is loaded, the algorithm "pre-computes" the execution steps, allowing the user to step forward and backward through time without re-running the logic.

### UI/UX
* **Theme:** A custom "Neon-Dark" interface using CSS radial gradients and variable-based theming.
* **Responsive:** Grid-based layout that adapts to different screen sizes.
* **Typography:** Optimized system-font stack for 100% offline consistency.

---

## How to Use
1.  **Download** the `index.html` file.
2.  **Open** the file in any modern web browser (Chrome, Firefox, Safari, Edge).
3.  **Interact:** * Select a **Preset Graph** or enter a custom **Adjacency List**.
    * Click **Build Steps** to initialize the algorithm.
    * Use **Step** to learn line-by-line or **Play** to watch the full animation.
    * Hover over the **Pseudocode** lines for detailed tooltips explaining the "Why" behind the "How."

---

## 📜 Academic Context
This tool was developed for **BCS 309: Algorithms** to demonstrate that the tool is merely the medium—the goal is a deep, intuitive understanding of graph theory and algorithmic efficiency.

