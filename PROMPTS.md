# Prompt Engineering in AI

Prompt engineering is the art of asking the right question to get the best output from a Large Language Model (LLM). It enables direct interaction with the LLM using only plain language prompts. The goal of prompt engineering is to find the optimal prompt so that the language model best solves the task at hand.


Links for reference and study :

- [ earn Prompting Beginner](https://learnprompting.org/docs/basics/intro)
- [ Learn Prompting Advanced]()
-

## Tokens

In the context of Large Language Models (LLMs) like GPT-3 or GPT-4, a token can be as short as one character or as long as one word. For example, "a" is one token, "apple" is one token, and "a apple" is two tokens.

Tokens are the units that the model reads when processing text. The model doesn't read character by character or word by word, but token by token. The number of tokens in a text string affects how much of it can be processed by the model at once, as each model has a maximum limit of tokens it can handle in a single request.

It's important to note that tokenization depends on the language and the specific tokenization algorithm used. For example, in English, "don't" would be tokenized into two tokens: "don" and "'t". But in some other languages or with different tokenization rules, it might be considered as a single token.

[Measure the number of tokens for a string/text](https://platform.openai.com/tokenizer)


## Best pratices for prompt Engineering

1. Give clearer instructions
2. Split complex tasks into simpler subtasks
3. Structure the instruction to keep the model on task
4. Prompt the model to explain before answering
5. Ask for justifications of many possible answers, and then synthesize
6. Generate many outputs, and then use the model to pick the best one
7. Custom-tune custom models to maximize performance


## Types of Prompts

### Direct Prompting (Zero-shot)

Direct prompting, also known as Zero-shot, is the simplest type of prompt. It provides no examples to the model, just the instruction. For example, you can ask the model to generate a list of ideas for blog posts for tourists visiting New York City for the first time.

### Chain-of-Thought Prompting (CoT)

Chain-of-Thought (CoT) prompting is a type of language prompting technique used in natural language processing (NLP) that involves the generation and refinement of chains of reasoning to facilitate better language understanding and generation. In CoT prompting, a language model is presented with a prompt to perform a given task. The model is then given a set of rationales (or reasons) for why a given word or phrase might be the correct answer.

You can use this sentence in your **prompt** to improve your results
![Alt text](./img/COT%20trigger.png)

## Zero-Shot Learning

Zero-shot learning (ZSL) is a problem setup in deep learning where, at test time, a learner observes samples from classes which were not observed during training, and needs to predict the class that they belong to. For example, given a set of images of animals to be classified, along with auxiliary textual descriptions of what animals look like, an artificial intelligence model which has been trained to recognize horses, but has never been given a zebra, can still recognize a zebra when it also knows that zebras look like striped horses.

## Example

Let’s consider an example of a prompt for a chatbot:

> Prompt: You are a mighty and powerful prompt-generating robot. You need to understand my goals and objectives and then design a prompt. The prompt should include all the relevant information context and data that was provided to you. You must continue asking questions until you are confident that you can produce the best prompt for the best outcome. Your final prompt must be optimized for chat interactions. Start by asking me to describe my goal, then continue with follow-up questions to design the best prompt.

In this example, the prompt is designed to guide the chatbot to interact with the user, understand their goals and objectives, and then generate a suitable response. This is an example of direct prompting or zero-shot learning, where the chatbot is given a task without any examples.

## Conclusion

Prompt engineering is a crucial aspect of working with AI models, particularly in the field of natural language processing. It involves designing and refining prompts to guide the model’s responses. Understanding and effectively using techniques like CoT and zero-shot learning can significantly enhance the performance of AI models.