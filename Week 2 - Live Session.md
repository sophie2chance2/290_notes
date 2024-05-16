# Context!

![](Pasted%20image%2020240515184258.png)
- How to measure how well the model works
	- Check similarity (rouge)
	- Human in the loop
	- If the model has never been trained on a chocolate chip recipe, will it be able to make that recipe
	- Have agent models evaluate the model
		- One likes Cakey cookies, another likes crispy, and they all score the model
		- Voting scheme to scale the votes of each of the agents
	- Models that are trained to generate an embedding for a whole sentence. The whole recipe. Just that ingredient. 
		- Getting a fuzzier match, doesn't need to be "cookie" can be "biscuit"
	- Not simple like a math problem, many right answers
- ![](Pasted%20image%2020240515185737.png)
	- Pretty quickly the transformer models were doing better than the humans because the model was jumbling words
- ![](Pasted%20image%2020240515185951.png)
	- ![](Pasted%20image%2020240515190053.png)
	- ![](Pasted%20image%2020240515190341.png)
- ![](Pasted%20image%2020240515191312.png)
	- Changing the order of the question and giving the text, would change the response. 
	- Say what you want and say what you don't want

### Embedding
- If you have a fixed set of words, your model is immediately out of date, new words being created
- Break words into parts (tokens)
- 30,000 - 50,000 tokens instead of over 100k words
- ![](Pasted%20image%2020240515193127.png)
	- Temperature at 1 is exactly what came in
		- Higher than 1 will be softer
			- Creative writing (temp: 1.5)
		- Lower than 1 will be sharper
			- Non-fiction writing (temp: .6)
			- A SUPER low temp (0.00001) may push it off in a weird direction, if there are 2 that are pretty close to being correct it will create a Huge difference between them even though there is a pretty small difference
- ![](Pasted%20image%2020240515194045.png)


# Python Notebook
https://github.com/MIDS-GenAI-290/2024-summer-private/blob/main/materials/lesson_notebooks/Week_2_Lesson_Notebook_Word_Embeddings_and_Simple_Next_Word_Predictions.ipynb

cos_sim
- Identify words that have similar uses
- Take the dot prod of 2 words and see how close the words are to each other

Hugging Face
- has a bunch of abstractions
- Large collection of trained models
- Has the weights needed to do the generation
- 