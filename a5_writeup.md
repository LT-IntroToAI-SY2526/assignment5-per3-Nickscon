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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

I learned how to do 3 dimensional lists, and how to satisfy constraints within a list with finding and assignment of values. And how searching and finding values within 2d and 3d lists/arrays are very similar with the exception of inclusion of more repetitive functions, as search functions within 2d lists may only include one iteration of a column and row search but 3d lists would use multiple iterations as it loops through each boxes row and column to verify whether the move is valid or not by checking the value within the list. BFS and DFS are very similar except for the implementation in which they're different because of the objects that they'd scan

2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

We can apply our knowledge of this assignment through 3d and 2d lists and how to integrate them together along with class and methods inside of a class, as well as iterating through 3d objects and 2d objects which we did multiple times in this problem. Real world scenarios where DFS or BFS might be useful could be checking whether a student submitted an assignment or not except on a easier scale because it'd only be true or false instead of numerical values.

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

The stack class and queue classes work by looking through objects through different ways, as Stack uses a LIFO structure which is last in first out meaning the last object added in an array is the first object out which is important for DFS because it requires depth so it needs to go through the entire array before going out, meaning stack is the perfect class for DFS. While queue works as FIFO as the first object in an array is the first object out, which is perfect for BFS because it only goes on the surface level meaning it explores each row cell by cell. Meaning it explores all the neighboring cells before checking deeper. Stack vs Queue changes the way search algorithim follows solutions because of how the order of each search algorithim is, as Stack would be better for deeper searches as it goes into one branch deeply before checking other branches while Queue would just evenly check nods within branches before checking other nodes.