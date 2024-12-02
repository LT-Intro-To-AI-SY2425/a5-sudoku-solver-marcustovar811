# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

Comarping, DFS goes as deep as it can down one path before turning back. This can be fast if it finds a good path early, and it doesn’t need much memory because it only keeps track of the items on its current path. But, it's inefficient on large paths because it is too complex. DFS is best when memory is sparse and you can stop early if you find what you need. BFS looks at all the paths level by level. It can find answers faster in certain  cases, but it uses a ton of memory. It’s better to choose BFS when you have a lot of paths that go deep.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

It affected my algorithim because both choices impacted my data structures in lots of ways that can be great depending on the amount of data available. we could have possibly used Recursive Call Stack to operate in the same objecting that DFS accomplishes. 

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?'

This current implementation can be adapted to create efficient data structures that can handle larger puzzles. For example, the Sudoku solver could be scaled up to work with bigger levels. The concepts from the Sudoku algorithim can also be applied to real-world problems, like pattern recognition. In some areas like health and science, this approach could help uncover useful patterns in large amounts of data.