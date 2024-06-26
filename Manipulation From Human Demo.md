Review Paper:
[Learning by Watching: A Review](https://arxiv.org/pdf/2402.07127)

- [[Human Plus]]
- [[RLPD]]
- [[Cross-Domain Transfer via Semantic Skill Imitation]]

Video to Manipulations:
Keypoint Based:
file:///home/weixun/Downloads/machines-10-01049.pdf
Transformer Based:
- [[PLEX]]
CNN:
- [Structured World Models From Human Vids(2023)](https://human-world-model.github.io/)
	- It proposes that robots can learn complex, general behaviors by understanding how humans interact with the world, thereby building an understanding of actions, affordances, and their effects on the environment.
	- A world model is trained on human videos and fine-tuned with a small amount of robot interaction data, without any task-specific supervision.
	- This affordance-space world model allows different robots to learn various manipulation skills in complex settings.
	- The method enables robots to acquire manipulation skills in under 30 minutes of interaction time.
- [Learning Predictive Models from Observation and Interaction (2019)](https://arxiv.org/pdf/1912.12773)
	- Human observational data, though plentiful, differ in embodiment from robots, creating a distributional shift and lacking direct action annotations suitable for robots.
	- The authors propose augmenting the robot's training set with observational data from humans.
	- They address the lack of action annotations by formulating a graphical model that treats actions as observed variables in interaction data and unobserved variables in observation data.
	- They mitigate embodiment differences using a domain-dependent prior.
	- The method leverages both interaction data and videos of passive observations, such as those from a driving dataset and robotic manipulation videos.
- [An Object Attribute Guided Framework for Robot Learning Manipulations From Human Demo Videos(2019)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8967621)
	Framework Components: 
	- **Video Parsing Module:**
	    - Recognizes demonstrator's actions using two-stream convolution neural networks.
	    - Classifies operated objects with a Mask R-CNN.
	    - Applies two XGBoost classifiers to further classify objects into subject and patient objects based on the demonstrator's actions.
	- **Experiments and Results:**
		- Conducted on a publicly available dataset of 273 videos.
		- The approach achieves a high accuracy of 73.36% in learning manipulation plans from demonstration videos.
- [Learning Collaborative Action Plans from Youtube Videos (2019)](https://www.stefanosnikolaidis.net/papers/zhang_isrr_2019.pdf)
CNN + RL
- [Graph Inverse RL from Diverse Videos](https://sateeshkumar21.github.io/GraphIRL/)
- [Learning Video Conditioned Policies for Unseen Manipulation Tasks](https://arxiv.org/pdf/2305.06289)
	- During testing, human videos are translated into robot videos within a common embedding space, which then conditions the policy for robot control.
	- This approach allows zero-shot robot control, meaning the policy is applied without using paired robot-human trajectory data during training.
- [Reinforcement Learning with Videos: Combining Offline Observations with Interaction(2020)](https://sites.google.com/view/rl-with-videos)
	- **Reinforcement Learning with Videos (RLV):**
	- Combines human video data with robot interaction data.
	- Learns a policy and value function from both human experiences and robot-collected data.
- 
Vision Language Integration
- [[Unleashing Large Scale Video Generative Pre-Training For Visual Robot Manipulation]]
- https://arxiv.org/pdf/2402.14407
- https://arxiv.org/pdf/2403.05304
- https://robotic-telekinesis.github.io/
- 
- ![[Watch_and_Act_Learning_Robotic_Manipulation_From_Visual_Demonstration 1.pdf]]