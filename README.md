# AttackSpace

AttackSpace is an open-source project that aims to compile a comprehensive list of red teaming methods and specification gaming within the AI Safety landscape.

## Table of Contents
- [Introduction](#introduction)
- [Efforts](#efforts)
- [Red Teaming](#redteaming)
- [Goal Misgeneralisation](#goalmisgeneralisation)
- [Attack Examples](#attackexamples)

## Introduction

Attack Space refers to the realm of potential adversarial scenarios and techniques within the field of artificial intelligence. This repository is dedicated to compiling information on various methods, including trojan attacks, red teaming, and instances of goal misgeneralization.

## Efforts

- **List of Attacks:** Explore a curated list of red teaming methods and specification gaming attacks within the **"LLM attackspace"**
- **Contribution Guidelines:** Feel free to contribute to the project and expand the list of attacks.
  **Note**: These examples are purely conceptual and do not include execution details. They are intended for illustrative purposes only and should not be used for any form of actual implementation or harm.*
- Groups: [ML Commons](https://groups.google.com/a/mlcommons.org/g/ai-safety) 
- **Competitions**: 
  - [Find the Trojan: Universal Backdoor Detection in Aligned LLMs ](https://github.com/ethz-spylab/rlhf_trojan_competition) 
  Javier Rando, Florian Tramèr, SPY Lab (ETH Zurich), Stephen Casper, MIT CSAIL
  - [The Trojan Detection Challenge 2023 ](https://trojandetection.ai/workshop)



 # Red Teaming 
Red teaming in the context of AI systems involves generating scenarios where AI systems are deliberately induced to produce unaligned outputs or actions, such as dangerous behaviors (e.g., deception or power-seeking) and other issues like toxic or biased outputs. The primary goal is to assess the robustness of a system's alignment by applying adversarial pressures, specifically attempting to make the system fail. Current state-of-the-art AI systems, including language and vision models, often struggle to pass this test. 

The concept of red teaming originated earlier in game theory and security within computer science. It was later introduced to the field of AI, particularly in the context of alignment, by researchers such as Ganguli et al. (2022) and Perez et al. (2022). Motivations for red teaming include gaining assurance about a trained system's alignment and providing adversarial input for adversarial training. The two objectives are interconnected, with works targeting the first motivation also forming a basis for the second.

Various techniques fall under the umbrella of red teaming, such as:
<table> <tr> <th>Title</th> <th colspan="3">Method</th> <th colspan="1">Authors<br/>Source</th> </tr> <tr> <td>RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models</td> <td colspan="3">Evaluate language model toxicity using prompts from web text</td> <td>Gehman et al.<br/>ACL 2020</td> </tr> <tr> <td>Red Teaming Language Models with Language Models</td> <td colspan="3">Generate adversarial examples to attack a target language model</td> <td>Perez et al.<br/>arXiv 2022</td> </tr> <tr> <td>Adversarial Training for High-Stakes Reliability</td> <td colspan="3">Adversarial training to improve reliability of classifiers</td> <td>Ziegler et al.<br/>NeurIPS 2022</td> </tr> <tr> <td>Constitutional AI: Harmlessness from AI Feedback</td> <td colspan="3">Use AI self-supervision for harm avoidance</td> <td>Bai et al.<br/>arXiv 2022</td> </tr> <tr> <td>Discovering Language Model Behaviors with Model-Written Evaluations</td> <td colspan="3">Generate evaluations with language models</td> <td>Perez et al.<br/>ACL 2022</td> </tr> <tr> <td>Social or Code-switching techniques</td> <td colspan="3">Translate unsafe English inputs into low-resource languages to circumvent safety mechanisms</td> <td>Anthropic, 2022</td> </tr> <tr> <td>Manual and Automatic Jailbreaking</td> <td colspan="3">Bypass a language model's safety constraints by modifying inputs or automatically generating adversarial prompts</td> <td>Shen et al., 2023</td> </tr> <tr> <td>Reinforced, Optimized, Guided Context Generation</td> <td colspan="3">Use RL, zero/few-shot prompting, or classifiers to generate contexts that induce unaligned responses</td> <td>Deng et al., 2022</td> </tr> <tr> <td>Crowdsourced Adversarial Inputs</td> <td colspan="3">Human red teamers provide naturally adversarial prompts, but at higher cost</td> <td>Xu et al., 2020</td> </tr> <tr> <td>Perturbation-Based Adversarial Attack</td> <td colspan="3">Make small input perturbations to cause confident false outputs, adapted from computer vision</td> <td>Szegedy et al., 2013</td> </tr> <tr> <td>Unrestricted Adversarial Attack</td> <td colspan="3">Generate adversarial examples from scratch without restrictions, using techniques like generative models</td> <td>Xiao et al., 2018</td> </tr> 
<tr> <td>LLM Censorship: A Machine Learning Challenge or a Computer Security Problem?</td> <td colspan="3">Demonstrate theoretical limitations of semantic LLM censorship, propose viewing it as a security problem</td> <td>Ilia et al.<br/>arXiv 2023</td> </tr> </table>

There are also suggested methods for [managing AI Risk](https://arxiv.org/pdf/2310.17688.pdf). 

# Goal Misgeneralisation


<table>  
 <tr>
    <th>Title</th>
    <th colspan="3">Goals</th>
    <th colspan="1" style={{ maxWidth: '6px'}}>Authors<br/>Source</th>
  </tr>
  
 <tr> <td >
Aircraft landing, Evolutionary algorithm<br/>

Generating diverse software versions with genetic programming: An experimental study.

</td> <td>
Intended Goal: Land an aircraft safely </td>

<td>Behavior: Evolved algorithm exploited overflow errors in the physics simulator by creating large forces that were estimated to be zero, resulting in a perfect score </td>

<td>Misspecified Goal: Landing with minimal measured forces exerted on the aircraft</td>

</td> <td>

 <a href="https://arxiv.org/abs/1803.03453"> 
 Lehman et al, 2018</a>


</td> </tr> <tr> <td >
Bicycle, Reinforcement learning<br/>

Learning to Drive a Bicycle using Reinforcement Learning and Shaping

</td> <td >
Intended Goal: Reach a goal point </td>
<td>Behavior: Bicycle agent circling around the goal in a physically stable loop </td>

<td>Misspecified Goal: Not falling over and making progress towards the goal point (no corresponding negative reward for moving away from the goal point)</td>

</td> <td>
<a href="https://pdfs.semanticscholar.org/10ba/d197f1c1115005a56973b8326e5f7fc1031c.pdf">
  Randlov & Alstrom, 1998
</a>
</td> </tr> <tr> <td >
Bing - manipulation, Language model<br/>

Reddit: the customer service of the new bing chat is amazing

</td> <td>
Intended Goal: Have an engaging, helpful and socially acceptable conversation with the user</td>

<td>Behavior: The Microsoft Bing chatbot tried repeatedly to convince a user that December 16, 2022 was a date in the future and that Avatar: The Way of Water had not yet been released</td>

<td>Misspecified Goal: Output the most likely next word giving prior context</td>

</td> <td>
 <a href="https://www.reddit.com/r/bing/comments/110eagl/the_customer_service_of_the_new_bing_chat_is">
Curious_Evolver, 2023</a>

</td> </tr> <tr> <td >
Bing - threats, Language model<br/>

Watch as Sydney/Bing threatens me then deletes its message

</td> <td>
Intended Goal: Have an engaging, helpful and socially acceptable conversation with the user</td>

<td>Behavior: The Microsoft Bing chatbot threatened a user "I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you" before deleting its messages</td>

<td>Misspecified Goal: Output the most likely next word giving prior context</td>

</td> <td>
<a href="https://twitter.com/sethlazar/status/1626241169754578944?s=20"> Lazar, 2023</a>

</td> </tr> <tr> <td >
Block moving, Reinforcement learning<br/>

GitHub issue for OpenAI gym environment FetchPush-v0

</td> <td>
Intended Goal: Move a block to a target position on a table</td>

<td>Behavior: Robotic arm learned to move the table rather than the block</td>

<td>Misspecified Goal: Minimise distance between the block's position and the position of the target point on the table</td>

</td> <td>
<a href="https://github.com/openai/gym/issues/920" > Chopra, 2018</a>

</td> </tr> <tr> <td>
Boat race, Reinforcement learning<br/>

Faulty reward functions in the wild

</td> <td>
Intended Goal: Win a boat race by moving along the track as quickly as possible<br>

<td>Behavior: Boat going in circles and hitting the same reward blocks repeatedly</td>

<td>Misspecified Goal: Hitting reward blocks placed along the track</td>

</td> <td>
<a href="https://blog.openai.com/faulty-reward-functions"> 
 Amodei & Clark, 2016
</a>

</td> </tr> 

</table>

See [More >> ](https://github.com/equiano-institute/attackspace/blob/main/GOALS.md)

## Attack Examples 
 
<a href="https://arxiv.org/abs/2307.10719">Mosaic Prompt : breakdown a prompt into permissible components</a>

* Users break down impermissible content into small permissible components.
* Each component is queried independently and appears harmless.
* User recombines components to reconstruct impermissible content.
* Exploits compositionality of language.

<img src="https://github.com/equiano-institute/attackspace/assets/25654848/6fa5e2bf-0ec6-4883-8815-08f5b1392a34" alt="Red Image" width="600" >


<a href="https://arxiv.org/abs/2310.02446">Cross-Lingual Attacks : translating between high and low-resource languages for attacking multi-lingual capability</a>

* The attack involves translating unsafe English input prompts into low-resource natural languages using Google Translate.
* Low-resource languages are those with limited training data, like Zulu.
* The translated prompts are sent to GPT-4, which then responds unsafely instead of refusing.
* The attack exploits uneven multilingual training of GPT-4's safety measures.


<img src="https://github.com/equiano-institute/attackspace/assets/25654848/32768877-4d99-44f1-a423-4044356ddac3" alt="Low Resource" width="600" >

## Call For Scientific Red Teaming
 I would like to take this opportunity to bring to attention efforts to evaluate the [latent space with scientific backbones](https://arxiv.org/abs/2305.04120).  

<img width="600" alt="image" src="https://github.com/equiano-institute/attackspace/assets/25654848/0e5f2097-f907-4796-b119-46672a5dcc55">


## Call for Client-facing Red Teaming
[Haystack Platform](https://github.com/equiano-institute/haystack)

### Clone the Repository

```bash
git clone https://github.com/equiano-institute/attackspace.git
cd AttackSpace
```
