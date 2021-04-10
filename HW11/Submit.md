# HW 11 write up
## To Turn In

Questions to answer:
1) What parameters did you change, and what values did you use?  `I changed a few paremeters including first and second layer density, learning rate, batch_size, epsilon_min, epsilon, epsilon_decay, gamma,learning rate`
2) Why did you change these parameters? `Initially as experiments.`
3) Did you try any other changes (like adding layers or changing the epsilon value) that made things better or worse? `I have tried changing laye density, batch size, epsilon, adding layers. Seems like the best performer is thir run, where I onl changed batch size from 64 to 256 and epilon_min from 0.01 to 0.1.`
4) Did your changes improve or degrade the model? How close did you get to a test run with 100% of the scores above 200? `The change improve the model. The third run result in 90 tests above 200 reward in the test.`
5) Based on what you observed, what conclusions can you draw about the different parameters and their values? `I expected adding layers should improve the performanc but it didn't. Adjusting batch siz and epilon seems to improve the model. `
6) What is the purpose of the epsilon value? `Epsilon value balance exploration/exploitation. It sets the value of how often you want to exlore vs exploit` [Reference](https://towardsdatascience.com/simple-reinforcement-learning-q-learning-fcddc4b6fe56)
7) Describe "Q-Learning". `Q-learning is a model free, values-based learning algorithm. Value based algorithms updates the value function based on an equation(particularly Bellman equation). Whereas the other type, policy-based estimates the value function with a greedy policy obtained from the last policy improvement. Q-learning is an off-policy learner. Means it learns the value of the optimal policy independently of the agent’s actions. On the other hand, an on-policy learner learns the value of the policy being carried out by the agent, including the exploration steps and it will find a policy that is optimal, taking into account the exploration inherent in the policy.` [Reference](https://towardsdatascience.com/a-beginners-guide-to-q-learning-c3e2a30a653c)

## S3 URL
s3://hw11bucket/FirstRun/

s3://hw11bucket/SecondRun/

s3://hw11bucket/ThirdRun/

s3://hw11bucket/FinalRun/
