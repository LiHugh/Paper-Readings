# [Generating Adjacency-Constrained Subgoals in Hierarchical Reinforcement Learning](https://papers.nips.cc/paper/2020/file/f5f3b8d720f34ebebceb7765e447268b-Paper.pdf)
Their code is available at https://github.com/trzhang0116/HRAC.
## Motivation
Distant subgoals can be substituted by closer subgoals, as long as they drive the low-level to move towards the same “direction”. By reducing the action space of the
high-level, the learning efficiency of both the high-level and the low-level can be improved: for the high-level, a considerably smaller action space relieves the burden of exploration and value function
approximation; for the low-level, adjacent subgoals provide a stronger learning signal as the agent can be intrinsically rewarded with a higher frequency for reaching these subgoals.

## Some Details
- Calculate the shortest transition distance: the author approximate this through n different deterministic policies. However, training a set of diverse policies separately is costly, and use one single policy n=1 to approximate the policy set can lead to non-optimality. Thus the author build a policy set by sampling policies that emerge in different training stage. To aggregate the adjacency information gathered by multiple policies, they explicitly memorize the adjacency information by constructing a binary k-step adjacency matrix of the explored states. The adjacency matrix has the same size as the number of explored states. (Limitation: too much memory space for this) 
