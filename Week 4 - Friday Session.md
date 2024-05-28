# This weeks News
![](Pasted%20image%2020240528141727.png)
- Once you get over 3B parameters then it is better with this method
- Predicting MULTIPLE future tokens - works with larger models (above 3B)
- ![](Pasted%20image%2020240528141919.png)

# Where are we? Training after Pre-Training & Supervised Fine-Tuning
![](Pasted%20image%2020240528142028.png)
![](Pasted%20image%2020240528142526.png)
- Often models are good at one task, ie. summarizing, translation, classification
![](Pasted%20image%2020240528142618.png)
- We want a model that can do everything
- Want them to be able to take any task and do a good job with it
- ALSO want them to be ethical, unbiased, helpful, safe

# The Alignment Problem
![](Pasted%20image%2020240528142914.png)
![](Pasted%20image%2020240528142959.png) 
- Not very good alignment right now
![](Pasted%20image%2020240528143117.png)
- Not that easy
- If misspelling very often, then model could learn that misspelling
- You must say... "I don't want this thing, I want this"
![](Pasted%20image%2020240528143316.png)
- Do you like it / do you not like it
![](Pasted%20image%2020240528143418.png)
- This is not the natural prediction for next word. 
- Will need to tweak the training 
- ![](Pasted%20image%2020240528143539.png)


# Alignment and Training
![](Pasted%20image%2020240528143555.png)

![](Pasted%20image%2020240528143853.png)

# Reinforcement Learning
![](Pasted%20image%2020240528143955.png)
- Reward system - take action based on reward structure
- Usually there is no reward until the very end

![](Pasted%20image%2020240528144238.png)
- At every decision, there is an infinite number of combinations
- Goal: Find a policy - 
	- A policy is the conditional probability to take an action A at time t when you are in state S at time T. YOu should take an action A at time S
	- ![](Pasted%20image%2020240528144509.png)
	- Optimize the reward over time
	- Can be deterministic or stochastic
	- Similar to what we are doing with predicting tokens given the context
	- ![](Pasted%20image%2020240528144845.png)
		- Estimate the value of a state if you take an action A given policy, pi. 
		- Chess - assign a value for this situation
- ![](Pasted%20image%2020240528145109.png)
- ![](Pasted%20image%2020240528151644.png)
# Instruction-based Training
# Reinforcement Learning from Human Feedback
![](Pasted%20image%2020240528152256.png)
![](Pasted%20image%2020240528152417.png)
- ^ Want to optimize this
- Can't just optimize for just one reward number. Need to keep the model pretty similar to the original model - you are fine tuning not redoing
- ![](Pasted%20image%2020240528153136.png)

# DPO
![](Pasted%20image%2020240528153614.png)
![](Pasted%20image%2020240528154128.png)

