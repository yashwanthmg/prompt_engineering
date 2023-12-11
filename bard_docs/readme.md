Introduction to prompt design

bookmark_border
Prompt design is the process of creating prompts that elicit the desired response from language models. Writing well structured prompts is an essential part of ensuring accurate, high quality responses from a language model. This page introduces some basic concepts, strategies, and best practices to get you started in designing prompts.

What is a prompt
A prompt is a natural language request submitted to a language model to receive a response back. Prompts can contain questions, instructions, contextual information, examples, and partial input for the model to complete or continue. After the model receives a prompt, depending on the type of model being used, it can generate text, embeddings, code, images, videos, music, and more.

Prompt content types
Prompts can include one or more of the following types of content:

Input (required)
Context (optional)
Examples (optional)
Input
An input is the text in the prompt that you want the model to provide a response for, and it's a required content type. Inputs can be a question that the model answers (question input), a task the model performs (task input), an entity the model operates on (entity input), or partial input that the model completes or continues (completion input).

Question input
A question input is a question that you ask the model that the model provides an answer to.

Prompt:
What's a good name for a flower shop that specializes in selling bouquets of
dried flowers?
  

Response:
* **Dried Blooms**
* **Floral Arrangements**
* **The Flower Shop**
* **A Touch of Nature**
* **Bouquets Galore**
* **The Perfect Bloom**
* **Scented Splendor**
* **Dried Flower Arrangements**
* **Preserved Petals**
  
(text-bison@001)
Task input
A task input is a task that you want the model to perform. For example, you can tell the model to give you ideas or suggestions for something.

Prompt:
Give me a list of things that I should bring with me to a camping trip.
  

Response:
Tent, sleeping bag, sleeping pad, camping stove, cooking utensils, food, water, first aid kit, flashlight, lantern, matches or lighter, trash bags, map and compass, sunscreen, insect repellent, hat, sunglasses, and rain gear.
  
(text-bison@001)
Entity input
An entity input is what the model performs an action on, such as classify or summarize. This type of input can benefit from the inclusion of instructions.

Prompt:
Classify the following items as [large, small].
Elephant
Mouse
Snail
  

Response:
Elephant is large.
Mouse is small.
Snail is small.
  
(text-bison@001)
Completion input
A completion input is text that the model is expected to complete or continue.

Prompt:
Some strategies to overcome writer's block include
  

Response:
* **Freewriting.** This is a technique where you write whatever comes to mind, without stopping to think about grammar or spelling. This can help you to generate ideas and get your creative juices flowing.
* **Brainstorming.** This is a technique where you write down all of the ideas that come to mind, without judging them. Once you have a list of ideas, you can start to narrow them down and develop them further.
* **Mind mapping.** This is a technique where you draw a diagram of your ideas, connecting them with lines to show how they relate to each other. This can help you to visualize your ideas and see how they fit together.
* **Taking a break.** Sometimes, the best way to overcome writer's block is to take a break from writing and do something else for a while. This can help you to clear your head and come back to your writing with fresh eyes.
* **Getting help from others.** If you're struggling to overcome writer's block, don't be afraid to ask for help from others. You can talk to a friend, family member, or teacher, or you can seek professional help from a therapist or writing coach.
  
(text-bison@001)
Context
Context can be one of the following:

Instructions that specify how the model should behave.
Information that the model uses or references to generate a response.
Add contextual information in your prompt when you need to give information to the model, or restrict the boundaries of the responses to only what's within the prompt.

Prompt:
Marbles:
Color: red
Number: 12
Color: blue
Number: 28
Color: yellow
Number: 15
Color: green
Number: 17

How many green marbles are there?
  

Response:
There are 17 green marbles.
  
(text-bison@001)
Examples
Examples are input-output pairs that you include in the prompt to give the model an example of an ideal response. Including examples in the prompt is an effective strategy for customizing the response format.

Prompt:
Classify the following.
Options:
- red wine
- white wine

Text: Chardonnay
The answer is: white wine
Text: Cabernet
The answer is: red wine
Text: Moscato
The answer is: white wine

Text: Riesling
The answer is:
  

Response:
white wine
  

