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
- 