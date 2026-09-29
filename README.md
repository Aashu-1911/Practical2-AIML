# AIML Practical 2: Search Algorithms

This practical demonstrates common uninformed, informed, local, and constraint-satisfaction search techniques.

## Implemented algorithms

- Breadth First Search (BFS)
- Depth First Search (DFS)
- Uniform Cost Search (UCS)
- Greedy Best-First Search
- A* Search
- Hill Climbing for 8-Queens
- Simulated Annealing for 8-Queens
- Backtracking CSP for 4-Queens

## Project files

- `AIML_Practical_2_Search_Algorithms.ipynb`: notebook containing the practical explanation, implementations, timing table, and charts.
- `search_algorithms.py`: standalone executable version of the algorithms.
- `requirements.txt`: Python packages required by the standalone script and notebook.
- `sample_input.txt`: input/configuration values represented by the built-in example graph and seeded local-search runs.
- `sample_output.txt`: representative output from the standalone script. Execution times vary by machine.
- `screenshots/`: place screenshots of the notebook output and charts here.

## Dataset

No external dataset is required. The graph, weighted graph, heuristic values, and 8-Queens/4-Queens problem definitions are included in the notebook and Python source file.

## Requirements

Python 3.9 or newer is recommended. Install dependencies with:

```bash
python -m pip install -r requirements.txt
```

## Run the source code

```bash
python search_algorithms.py
```

The script prints the paths, costs, nodes expanded, and local-search/CSP results. It also displays two comparison charts. In a headless environment, replace `plt.show()` with `plt.savefig(...)` if image files are needed.

## Run the notebook

Open `AIML_Practical_2_Search_Algorithms.ipynb` in VS Code or Jupyter, select a Python kernel, and run the cells from top to bottom. Run the final timing and chart cells after all algorithm definitions have been executed.

## Notes on results

BFS and DFS operate on the unweighted graph. UCS and A* operate on the weighted graph. The local-search methods use a fixed seed (`42`) so their example results are repeatable, although execution time depends on the computer running them.
