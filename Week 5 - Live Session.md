What is the basic mechanism used by a large language model to come up with an answer?

How is an LLM trained?
- Feeding tokenized text and it learning from that
- BERT: Mask training - block out a sentence 
- GPT: Reinforcement learning 
	- Generate content that we are more likely to like
	- Tells us what we want to hear
- What is the idea of self-attention?
	- Recognizing which words in the context are important to each word in the sentence
- What is a decoder v an encoder?
	- Encoder: 
		- Does not generate language well
		- Can look before AND after
		- Masks: Today is a ___ day out, so we are going to the beach.
	- Decoder:
		- Can only look at what came before
		- Good for generating text
- What is alignment?
	- Helpful, safe, and reliable
	- You want models that are condusive to human success
	- Drama: OpenAI got rid of their super-alignment team
- How to maintain alignment?
	- Monitoring and evaluation
	- PPO - Preferred, Policy, Optimization
		- Human labor

# Encoding and Processing of Media

- Transformers
	- Representations of what you put into them
		- good at distinguishing fall (the person), fall (the action), fall (the season), fall (the water fall)
- M2M-200
	- Subword model
	- You can tell the tokenizer how many tokens it can have
	- Hypothetically you could have an embedding with 26 embeddings, one for each letter
		- Would make it more difficult in other places because the 'a' in 'fall' is very different from the 'a' in 'aardvark'
	- Can do multiple languages
		- There will be relationships between languages
		- Mixture of experts that focus on language
- Attention heads
	- Kind of like filters

# Vision Transformers
![](Pasted%20image%2020240605194136.png)
![](Pasted%20image%2020240605194145.png)
- Take a picture and segment it (tokenize the photo)
	- randomly mask one token
	- Predict something about that masked token
- Reduce the number of colors
![](Pasted%20image%2020240605194600.png)
- Predict the class based on the labels you are given
- Modify the weights in the model as predictions are right/wrong

![](Pasted%20image%2020240605194723.png)

![](Pasted%20image%2020240605194906.png)

![](Pasted%20image%2020240605195020.png)
![](Pasted%20image%2020240605195109.png)
- High cos similarity if they belong together & low if they do not
![](Pasted%20image%2020240605195307.png)
- Encode the words, encode the image, do cos similarity

![](Pasted%20image%2020240605195726.png)
- Compare input to reconstructed input