Overview

For each of the following problems implemented the below:
* Design and implement two approximation algorithms
* Implement a random test input generator
* Run the algorithms on generated test inputs. Decide, which algorithm is better

Input
* Telecommunication optical network represented by a multigraph G; each edge of a graph represents a signal transmission channel with a bandwidth B;  k transmission demands, each demand i has a source si ,a destination ti and the size

Find
* Routing of all demand, i.e. a path Pi between si and ti  for every demand i. The sum of signal sizes going through each edge should not exceed its bandwidth. The total number of used transmission channels should be mini­­mal

Problem Statement
* Routing of all transmission demands, in such a way that number of used transmission channels are minimum

Deciding Factors
* Edges not shared by demands will always need a whole channel, even if channel is not filled to capacity
* We need to apply bin packing only to shared edges
* Number of channels required can differ largely based on the selected paths
* Therefore, path selection is the most critical part for solving this problem

Approaches
* Greedy Algorithm
* Local Search

Conclusion
* It is not guaranteed that any of the approaches used will give optimal solution
* Local search will converge and give us optimal solution if it completes
* However, to complete local search and get global maxima it takes a lot of time
* We took an iteration bound to terminate the search after a certain time
* When local search is terminated by iteration bound, there remains a possibility of getting local maximum 
* Nevertheless, for more complicated and larger graphs Local search will be better than Greedy Algorithm
