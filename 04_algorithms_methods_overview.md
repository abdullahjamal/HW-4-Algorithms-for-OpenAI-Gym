# Un-Informed and Informed Search Algorithms:
*DFS*: It is an algorithm for traverse and search a graph or tree. The strategy of DFS is to expand the deepest node first. It is usually implemented using stack which uses LIFO strategy. It is linear in space with respect to the paths explored.

*BFS*: The goal of BFS is the same as DFS but it expands the shallowest node first. It is usually implemented using Queue which uses FIFO strategy. It is exponential in time and space.

*Uniform Search*: BFS finds the shortest path in terms of actions but it fails to incorporate the cost. The uniform search expands the cheapest node first. It is implemented with different data structure i.e. priority queue where priority is the cumulative cost.

*Heuristic Search*: So far, we have discussed uninformed search where an agent doesn’t know about the goal unless they happen to stumble on goal. Heuristic search is a part of informed search which uses heuristic function. The idea behind heuristic function is to inform the search about the direction to a goal. It tells an information about which neighbor will lead to a goal.

*Greedy Search*: The strategy is to expand a node that seems closest to a goal.

*A star Search*: It is a combination of both lowest cost first and best-first search. It considers both path cost and heuristic information. Examples are path-planning, routing problems, video games, robot motion planning etc.

# Adversarial Search:
*Minimax Search*: It is kind of backtracking algorithm that uses a minimax function. Minimax function computes a minimax value for each node which is best achievable for a current player assuming the opponent is playing optimally too.

*Alpha-Beta Pruning*: It reduces the computation time of minimax search by a huge amount allow us to search faster and deeper which is a problem in simple minimax search. It introduces two new parameters alpha and beta. Alpha is value that MAX can get at any choice point along the path while beta is the best value for the MIN. 

*Expectimax Search*: It has a little variation from minimax search. In addition to min and max operation, it has a chance operation whose outcome is uncertain and it takes the expected values of an event.

# MDPs & Reinforcement Learning:
Before briefly describing RL algorithms, I will touch upon the markov decision process. It is defined as a set of states, set of actions, transition function that gives a probability that an action leads from one state to another state, a reward function, and a start state or may be terminal state.

*Value function*: It is equal to the expected total reward for an agent starting from some state. It tells you how good a state is for an agent to be in. There is an optimal value function corresponds to the higher value among other functions for all state. Optimal policy corresponds to optimal value function.

*Q-function*: It is a function of state-action pair which returns a value.

*Value Iteration*: It computes the optimal value function by iteratively improving the estimate of value function. It repeatedly update the Q-function and value function until it converges. It repeats the bellman updates.

*Policy Iteration*: Value function tries to find the optimal value function but the agent only cares about the optimal policy and sometimes you can get the convergence of optimal policy before value function. Policy iteration redefine the policy at each time step and estimate the value function from this policy until convergence. It is guaranteed to find the optimal policy and takes less time as compare to value iteration.

*Q-Learning*: We can use previous briefly described algorithms in those environments where agents can interact with environment, and from history of its interactions, they can try to approximate transition probabilities and rewards. After that, they can use those algorithms to find optimal policy. We can call them model-based learning. In model free-learning, the agent doesn’t assume to know anything about transition functions and rewards rather agent will derive an optimal policy via interaction with the environment. Q-learning is a case of model-free learning. It is a sample based q-value iteration which approximate the q function of state action pair from the samples that observe during the interaction with the environment.

