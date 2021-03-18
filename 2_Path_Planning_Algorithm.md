---
description: A general introduction to setting up your own path planning algorithm
---

# Path Planning Algorithm

## 1. Introduction

It is investigated what the most optimal path planning algorithm is for the clover drone. This is done since it was noted that this is not done in the base version of the drone. The path planning algorithm makes it possible that the drone would fly autonomous is a much better way than without the algorithm.

## 2. What algorithm is chosen?

Multiple path planning algorithms are found and it is investigated what is the best to implement. For example there is the Dijkstra algorithm and A\* and D\* and many more. The best algorithm is chosen based on a few criteria: the execution time, processing time. The path planning is chosen also based on the travel time and distance travelled. Based on these criteria the A\* algorithm is chosen. It does best in all these aspects, although the differences are really small. The best thing about the A\* algorithm is that it is really ”Smart”, it really is the shortest path \(known for now\). There is a difference in optimal paths for example: one can go 5 meters to the right \(x-direction\) and then 5 meters to the right \(y-direction\) however this is not optimal, it would be much better to go in a diagonal path. This difference would not be visible by only identifying the execution time and processing time since this would be the same. The difference is only noticeable in the amount of distance \(number of blocks\). Distance is also a vague term, what is meant? in this case it would be Manhattan distance, which is in case the ”amount of blocks” travelled.

The results of the different algorithms cannot be shown since this hugely depends on the environment of the path \(many obstacles or not\). It can however be noted that the A\* algorithm comes is on average 10 percent better than the other algorithms investigated.

## 3. How does A\* work?

**Result:** Optimal path between point A and point B

initialization;

make an openlist containing only the starting node

make an empty closed list

![](.gitbook/assets/image%20%2834%29.png)

## 4. Conclusion

After comparison the most optimal path planning algorithms is chosen. Based on a few criteria it came out that the A\* algorithm is the best. It overall wins because the algorithm really has the most optimal path instead of vertical and horizontal transitions.

Further research needs to be done to actually implement it and integrate it with the autonomous flight itself.

