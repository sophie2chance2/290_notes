![](photos/Pasted%20image%2020240508173427.png)
* x = features
* f(x) = function ~ Makes a prediction/classification based on the inputs
* Need a loss function
* Need an optimization function
![](photos/Pasted%20image%2020240508173919.png)
![](photos/Pasted%20image%2020240508174141.png)
- Pink: input
- Blue: H1
- Yellow: H2
- Green: Output
- Need to make sure that shape of matrices are correct
![](photos/Pasted%20image%2020240508174319.png)
- Output matrix of first step is 1x3 
![](photos/Pasted%20image%2020240508174512.png)
- Either trying to get a probability distribution
- Sigmoid will give a value between 0 and 1
- Softmax will give a value where all values will sub to 1
	- Max of 32k, so english language needs to be broken down into tokens
		- Means that you will likely go faster because you are using the tokenized values

### Batching
![](photos/Pasted%20image%2020240508175121.png)
- We will be using back propagation
	- We will calculate a loss based on how far off our answers were from the correct answer

![](photos/Pasted%20image%2020240508180128.png)
![](photos/Pasted%20image%2020240508180139.png)
![](photos/Pasted%20image%2020240508180333.png)
![](photos/Pasted%20image%2020240508180553.png)

# Cross Entropy
- Entropy
	- Uncertainty
		- An unfair coin (two heads) has an entropy of 0
			- Outcome is certain
		- A fair coin has an entropy of 1
			- 50/50 
		- 1000 sided die
			- The outcome is less certain 1 in 1000
- ![](photos/Pasted%20image%2020240508180816.png)
- ![](photos/Pasted%20image%2020240508180903.png)
	- D is the divergence value
	- Loss will not be 0 unless you did something wrong
		- There will always be some non-zero ambiguity with text
		- Today will be ______ ___ (could be day, weather, event, etc.)
- ![](photos/Pasted%20image%2020240508180922.png)
	- Useful for sparse categorical
- ![](photos/Pasted%20image%2020240508181030.png)
- ![](photos/Pasted%20image%2020240508181249.png)
- 