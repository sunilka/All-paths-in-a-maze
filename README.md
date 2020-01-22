# All-paths-in-a-maze
Print all the possible paths in a maze 

# Problem

Given a maze where some of the cells are blocked, where left top cell is the entry point and right bottom cell is the exit point, find all possible paths from entry to exit which goes through the non blocked cells.

# Solution

For finding all possible paths we do depth first traversal. We mark the start point as visited and then recursively try to find all possible paths form the accessible cells from the first cell. For example suppose we are at some arbitrary cell. We first mark the node, then call the function recursively to all its neighboring cells which are not blocked or marked earlier. If some paths are found from these recursive calls. It prepends current cell to those paths and return the result and unmark the current cell.
