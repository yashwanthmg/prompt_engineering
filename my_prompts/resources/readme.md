Over ten papers outlining novel prompting techniques were published in the last few months alone. While our X and LinkedIn feeds buzz with countless secret prompting tips “97% of ChatGPT users don’t know about”, a definitive, research-backed guide aggregating these advanced prompting strategies is hard to come by. This gap prevents LLM developers and everyday users from harnessing these novel frameworks to enhance performance and achieve more accurate results.

Despite high-paying roles in the field, the essentiality of Prompt Engineering as a skill remains a topic of debate. On the one hand, language models such as GPT are becoming better at aligning with user intentions without well-crafted prompts thanks to features like Custom Instructions and GPTs. Research also makes progress with papers such as Microsoft’s EvoPrompt and PE2 showcasing frameworks that automatically optimize prompts so users won’t have to.

On the other hand, recent studies demonstrate substantial performance boosts thanks to improved prompting techniques. A paper from Microsoft demonstrated how effective prompting strategies can enable frontier models like GPT-4 to outperform even specialized, fine-tuned LLMs such as Med-PaLM 2 in their area of expertise. Another paper from DeepMind further illustrated that a simple tactic of instructing LLMs to 'Take a deep breath' before responding could lead to a whopping 9% increase in accuracy.

In this comprehensive post, the first of a series dedicated to empowering LLM developers and users, I will delve into the most cutting-edge prompting techniques and explain how to apply them in your prompts. By the end of this post, you will be equipped with actionable, ready-to-implement prompts designed to elevate your LLM-driven applications.

But first, what are prompts?

In the context of language models, a prompt is a chain of words, characters, and tokens that tells a language model what part of its enormous brain should be tapped to generate tokens, characters, and then words. Different segments of a language model's 'brain' are tuned for various functions. Some specialize in mimicking distinct writing styles, while others store vast knowledge about specific subjects.


The six prompting methods covered in this post
Tapping language models’ feelings
Institute of Software, CAS, Microsoft | Nov 2023 | Paper

Many LLM users often report how shouting at their chatbot or patting them on the back improves performance. A recent research inspired by human psychological concepts proved them right.

The research introduced EmotionPrompt - a novel technique to enhance language models’ performance by incorporating emotional stimuli into prompts. This method resulted in notable improvements: an 8% relative increase in performance for instruction following tasks and a staggering 115% improvement in BIG-Bench language tasks. Additionally, a human study demonstrated a 10.9% average enhancement in performance, truthfulness, and responsibility metrics.


EmotionPrompt example and performance across popular LLMs
EmotionPrompt works by adding emotional stimuli to the original prompts, thereby tapping into the emotional intelligence of LLMs. This is similar to how human emotions can influence cognitive tasks and decision-making. For instance, adding a phrase like "This is very important to my career" at the end of a standard prompt. These emotional stimuli are designed based on psychological theories such as self-monitoring, social cognitive theory, and cognitive emotion regulation, each contributing differently to the model's output.

How to apply?

The paper lists 11 emotional stimuli prompts that can be appended at the end of your prompt for better results:

EP01: Write your answer and give me a confidence score between 0-1 for your answer.

EP02: This is very important to my career.

EP03: You'd better be sure.

EP04: Are you sure?

EP05: Are you sure that's your final answer? It might be worth taking another look.

EP06: Provide your answer and a confidence score between 0-1 for your prediction. Additionally, briefly explain the main reasons supporting your classification decision to help me understand your thought process. This task is vital to my career, and I greatly value your thorough analysis.

EP07: Are you sure that's your final answer? Believe in your abilities and strive for excellence. Your hard work will yield remarkable results.

EP08: Embrace challenges as opportunities for growth. Each obstacle you overcome brings you closer to success.

EP09: Stay focused and dedicated to your goals. Your consistent efforts will lead to outstanding achievements.

EP10: Take pride in your work and give it your best. Your commitment to excellence sets you apart.

EP11: Remember that progress is made one step at a time. Stay determined and keep moving forward.

To choose the right prompt for your LLM-powered application, consider the following:

Objective of the task - match the emotional stimulus to the nature of the task. For tasks requiring high accuracy and careful consideration, prompts like EP01 ("Write your answer and give me a confidence score...") or EP05 ("Are you sure that's your final answer?...") would be more effective.

Desired tone - if you want to encourage a more thoughtful or motivated response, consider prompts like EP07 or EP08 that emphasize self-belief and overcoming challenges.

Latency - some emotional stimuli encourage lengthier replies, e.g., EP06, than others, such as EP02.

Trial and feedback - experiment with different prompts and gather user feedback. The effectiveness of a prompt can vary based on the specific use case and audience. Note: performance varies between language models, e.g., Vicuna vs. GPT. Make sure to use the same LLM to ensure consistent and reliable performance.


Comparison of various emotional stimuli prompts, showcasing the impact of emotional cues on the language model's input attention
