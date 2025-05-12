# EX 6C TRAVELLING SALES MAN PROBLEM
## DATE:
## AIM:
To Solve Travelling Sales man Problem for the following graph.
![image](https://github.com/user-attachments/assets/653921a4-3d7b-4691-9b41-735e80f7af0b)

## Algorithm
1. Take the cost matrix that shows the cost between every pair of cities.
2. Generate all possible orders (permutations) in which the cities can be visited.
3. For each order, calculate the total travel cost, including returning to the starting city.
4. Keep track of the minimum total cost found so far.
5. After checking all possible orders, return the minimum cost as the final answer.
## Program:
```
/*
To implement the program for TSP.
Developed by: Subalakshmi V
Register Number:  212222040162
*/
```
```
def tsp_cost(tsp):
    return min(sum(tsp[i][j] for i, j in zip(path, path[1:] + path[:1])) for path in permutations(range(len(tsp))))

from itertools import permutations
tsp = [[-1, 30, 25, 10], [15, -1, 20, 40], [10, 20, -1, 25], [30, 10, 20, -1]]
print("Minimum Cost is :",tsp_cost(tsp))
```
## Output:
![image](https://github.com/user-attachments/assets/1e757740-b0d8-45de-b4aa-79a0fe04a797)

## Result:
Thus the program was executed successfully for finding the minimum cost to vist all cities.
