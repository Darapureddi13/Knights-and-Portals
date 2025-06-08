# Knights-and-Portals
# Shortest Path Finder with Teleportation

## Overview
This Python program finds the shortest path from the top-left corner to the bottom-right corner of a grid, allowing exactly one teleportation between any two empty cells.

## Features
- Finds optimal path using normal movement or one teleportation
- Handles blocked and empty cells
- Returns path length or -1 if no path exists
- Includes comprehensive test cases

## Requirements
- Python 3.x
- No external dependencies

## Installation
1. Save the code to a file (e.g., `shortest_path.py`)
2. Run the script:
```bash
python shortest_path.py
```

## Usage
### Input Format
The grid should be a 2D list where:
- `0` represents an empty cell (movable/teleportable)
- `1` represents a blocked cell

### Output
- Integer representing shortest path length
- `-1` if no path exists

## Algorithm
1. Uses BFS to calculate distances from start and end positions
2. Evaluates all possible teleportation pairs
3. Compares paths with and without teleportation
4. Returns the shortest valid path

## Test Cases
The script includes 5 test cases:
1. Simple open grid (expected: 4)
2. Grid where teleport helps (expected: 4)
3. Grid requiring teleportation (expected: 6)
4. Completely blocked grid (expected: -1)
5. Large open grid (expected: 18)

## Example
```python
grid = [
    [0, 1, 0],
    [1, 0, 0],
    [0, 0, 0]
]
print(find_shortest_path(grid))  # Output: 4
```

## License
MIT License
