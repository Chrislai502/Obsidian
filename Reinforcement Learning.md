[[PPO]]
[[SAC]]
## Keywords
- **Policy Invariance** :  Refers to a property where a certain transformations or changes in the environment or the agent's state (eg. action representations) do not affect the optimal policy. 

## Surveys
- A Survey on Offline Reinforcement Learning: Taxonomy, Review, and Open Problems
	- IQL 
		- https://arxiv.org/pdf/2110.06169
	- SAC
		- Soft actor-critic: Offpolicy maximum entropy deep reinforcement learning with a stochastic actor
	- TT 
		- https://arxiv.org/pdf/2106.02039
- Transfer Learning in Deep Reinforcement Learning: A Survey
	Categorizes based on Which components in an RL system is being pre-trained / transferred to train another policy / component. Categories are as follows:
	1. Reward Shaping:
		- Involves re-using reward functions from teacher methods.
		- Examples:
			Static Potential Function:
			- [[Potential Based Reward Shaping]]
			- [[Potential Based State Action Advice]]
			Dynamic Potential Function:
			- [[Dynamic Potential Based]]
			- [[Dynamic Value Function Advice]]
	2. Learning From Demonstrations:
		1. Pre-training Policy: 
			- [[Mastering the game of Go with deep neural networks and tree search]]
		2. Pre-training Value Functions: 
			- [[Pretraining deep actor-critic reinforcement learning algorithms with expert demonstrations]]
		Policy Iteration Frameworks:
		- [[Direct policy iteration with demonstrations]]
		Policy Gradient Methods:
		- [[Learning sparse rewarded tasks from sub-optimal demonstrations]]
		- [[Leveraging demonstrations for deep reinforcement learning on robotics problems with sparse rewards]]
		- [[Overcoming exploration in reinforcement learning with demonstrations]]
		- [[Policy optimization with demonstrations]]
		
