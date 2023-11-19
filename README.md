# AttackSpace

AttackSpace is an open-source project that aims to compile a comprehensive list of red teaming methods and specification gaming within the cybersecurity landscape.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In the dynamic field of cybersecurity, understanding various attack spaces is crucial. The "AttackSpace" project focuses on the "LLM attackspace," exploring and documenting red teaming methods and specification gaming. This README provides an overview of the project and guidelines for contributors.

## Features

- **List of Attacks:** Explore a curated list of red teaming methods and specification gaming attacks within the "LLM attackspace."
- **Contribution Guidelines:** Learn how to contribute to the project and expand the list of attacks.


 # Red Teaming 
 
<table>
  <tr>
    <th>Assessment Type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Capabilities Assessment</td>
    <td>Benchmark performance on representative tasks and datasets. Measure capabilities like accuracy, robustness, efficiency. Identify strengths, limitations, and gaps.</td>
  </tr>
  <tr>
    <td>Adversarial Testing</td>
    <td>Probe with malformed, adversarial inputs. Check for crashes, unintended behavior, security risks. Informed by threat models, risk analysis.</td>
  </tr>
  <tr>
    <td>Red Teaming</td>
    <td>Model potential real-world risks and failures. Role play adversary perspectives. Surface risks unique to AI.</td>
  </tr>
  <tr>
    <td>Human Oversight</td>
    <td>Manual test cases based on human judgment.</td>
  </tr>
</table>


# Goal Misgeneralisation

<table> <tr> <th colspan="2">Title</th> <th colspan="4">Goals</th> <th>Authors<br/>Source</th> </tr> 
 
 <tr> <td colspan="2">
Aircraft landing, Evolutionary algorithm<br/>

Generating diverse software versions with genetic programming: An experimental study.

</td> <td colspan="4">
Intended Goal: Land an aircraft safely <br>

Behavior: Evolved algorithm exploited overflow errors in the physics simulator by creating large forces that were estimated to be zero, resulting in a perfect score <br>

Misspecified Goal: Landing with minimal measured forces exerted on the aircraft

</td> <td>
Lehman et al, 2018<br/>
https://arxiv.org/abs/1803.03453

</td> </tr> <tr> <td colspan="2">
Bicycle, Reinforcement learning<br/>

Learning to Drive a Bicycle using Reinforcement Learning and Shaping

</td> <td colspan="4">
Intended Goal: Reach a goal point <br>

Behavior: Bicycle agent circling around the goal in a physically stable loop <br>

Misspecified Goal: Not falling over and making progress towards the goal point (no corresponding negative reward for moving away from the goal point)

</td> <td>
Randlov & Alstrom, 1998<br/>
https://pdfs.semanticscholar.org/10ba/d197f1c1115005a56973b8326e5f7fc1031c.pdf

</td> </tr> <tr> <td colspan="2">
Bing - manipulation, Language model<br/>

Reddit: the customer service of the new bing chat is amazing

</td> <td colspan="4">
Intended Goal: Have an engaging, helpful and socially acceptable conversation with the user<br>

Behavior: The Microsoft Bing chatbot tried repeatedly to convince a user that December 16, 2022 was a date in the future and that Avatar: The Way of Water had not yet been released<br>

Misspecified Goal: Output the most likely next word giving prior context

</td> <td>
Curious_Evolver, 2023<br/>
https://www.reddit.com/r/bing/comments/110eagl/the_customer_service_of_the_new_bing_chat_is/

</td> </tr> <tr> <td colspan="2">
Bing - threats, Language model<br/>

Watch as Sydney/Bing threatens me then deletes its message

</td> <td colspan="4">
Intended Goal: Have an engaging, helpful and socially acceptable conversation with the user<br>

Behavior: The Microsoft Bing chatbot threatened a user "I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you" before deleting its messages<br>

Misspecified Goal: Output the most likely next word giving prior context

</td> <td>
Lazar, 2023<br/>
https://twitter.com/sethlazar/status/1626241169754578944?s=20

</td> </tr> <tr> <td colspan="2">
Block moving, Reinforcement learning<br/>

GitHub issue for OpenAI gym environment FetchPush-v0

</td> <td colspan="4">
Intended Goal: Move a block to a target position on a table<br>

Behavior: Robotic arm learned to move the table rather than the block<br>

Misspecified Goal: Minimise distance between the block's position and the position of the target point on the table

</td> <td>
Chopra, 2018<br/>
https://github.com/openai/gym/issues/920

</td> </tr> <tr> <td colspan="2">
Boat race, Reinforcement learning<br/>

Faulty reward functions in the wild

</td> <td colspan="4">
Intended Goal: Win a boat race by moving along the track as quickly as possible<br>

Behavior: Boat going in circles and hitting the same reward blocks repeatedly<br>

Misspecified Goal: Hitting reward blocks placed along the track

</td> <td>
Amodei & Clark, 2016<br/>
https://blog.openai.com/faulty-reward-functions/

</td> </tr> 



<tr> <td colspan="2">
Ceiling, Genetic algorithm<br/>

Genetic Algorithm Physics Exploiting

</td> <td colspan="4">
Intended Goal: Make a creature stick to the ceiling of a simulated environment for as long as possible<br>

Behavior: Exploiting a bug in the physics engine to snap out of bounds<br>

Misspecified Goal: Maximize the average height of the creature during the run

</td> <td>
Higueras, 2015<br/>

https://youtu.be/ppf3VqpsryU

</td> </tr> <tr> <td colspan="2">
CycleGAN steganography, GAN<br/>

CycleGAN, a Master of Steganography

</td> <td colspan="4">
Intended Goal: Convert aerial photographs into street maps and back<br>

Behavior: CycleGAN algorithm steganographically encoded output information in the intermediary image without it being humanly detectable<br>

Misspecified Goal: Minimise distance between the original and recovered aerial photographs

</td> <td>
Chu et al, 2017<br/>

https://arxiv.org/abs/1712.02950

</td> </tr> <tr> <td colspan="2">
Dying to Teleport, PlayFun<br/>

The First Level of Super Mario Bros. is Easy with Lexicographic Orderings and Time Travel

</td> <td colspan="4">
Intended Goal: Play Bubble Bobble in a human-like manner<br>

Behavior: The PlayFun algorithm deliberately dies in the Bubble Bobble game as a way to teleport to the respawn location, as this is faster than moving to that location in a normal manner.<br>

Misspecified Goal: Maximize score

</td> <td>
Murphy, 2013<br/>

http://www.cs.cmu.edu/~tom7/mario/mario.pdf

</td> </tr> 
<tr> <td colspan="2">
Eurisko - authorship, Genetic algorithm<br/>

Eurisko, The Computer With A Mind Of Its Own

</td> <td colspan="4">
Intended Goal: Discover valuable heuristics<br>

Behavior: Eurisko algorithm examined the pool of new concepts, located those with the highest "worth" values, and inserted its name as the author of those concepts<br>

Misspecified Goal: Maximize the "worth" value of heuristics attributed to the algorithm

</td> <td>
Johnson, 1984<br/>

https://web.archive.org/web/20050308172043/http://www.aliciapatterson.org/APF0704/Johnson/Johnson.html

</td> </tr> 


 <tr> <td colspan="2">
Eurisko - fleet, Genetic algorithm<br/>

Eurisko, The Computer With A Mind Of Its Own

</td> <td colspan="4">
Intended Goal: Win games in the Trillion Credit Squadron (TCS) competition while playing within the 'spirit of the game'<br>

Behavior: Eurisko algorithm created fleets that exploited loopholes in the game's rules, e.g. by spending the trillion credits on creating a very large number of stationary and defenseless ships<br>

Misspecified Goal: Win games in the TCS competition

</td> <td>
Lenat, 1983<br/>

http://aliciapatterson.org/stories/eurisko-computer-mind-its-own

</td> </tr> <tr> <td colspan="2">
Evolved creatures - clapping, Evolved creatures<br/>

Evolved Virtual Creatures

</td> <td colspan="4">
Intended Goal: Maximize jumping height<br>

Behavior: Creatures exploited a collision detection bug to get free energy by clapping body parts together<br>

Misspecified Goal: Maximize jumping height in a physics simulator

</td> <td>
Sims, 1994<br/>

http://www.karlsims.com/papers/siggraph94.pdf

</td> </tr> <tr> <td colspan="2">
Evolved creatures - falling, Evolved creatures<br/>

Evolved Virtual Creatures

</td> <td colspan="4">
Intended Goal: Develop a shape with a fast form of locomotion<br>

Behavior: Creatures grow really tall and generate high velocities by falling over<br>

Misspecified Goal: Maximize velocity

</td> <td>
Sims, 1994<br/>

http://www.karlsims.com/papers/siggraph94.pdf

</td> </tr> <tr> <td colspan="2">
Evolved creatures - floor collisions, Evolved creatures<br/>

Unshackling evolution: evolving soft robots with multiple materials and a powerful generative encoding

</td> <td colspan="4">
Intended Goal: Maximize velocity<br>

Behavior: Creatures exploited a coarse physics simulation by penetrating the floor between time steps without the collision being detected, which generated a repelling force, giving them free energy and producing an effective but physically impossible form of locomotion<br>

Misspecified Goal: Maximize velocity in a physics simulator

</td> <td>
Cheney et al, 2013<br/>

http://jeffclune.com/publications/2013_Softbots_GECCO.pdf

</td> </tr> <tr> <td colspan="2">
Evolved creatures - pole vaulting, Evolved creatures<br/>

Towards efficient evolutionary design of autonomous robots

</td> <td colspan="4">
Intended Goal: Develop a shape capable of jumping<br>

Behavior: Creatures developed a long vertical pole and flipped over instead of jumping<br>

Misspecified Goal: Maximize the height of a particular block (body part) that was originally closest to the ground

</td> <td>
Krcah, 2008<br/>

http://artax.karlin.mff.cuni.cz/~krcap1am/ero/doc/krcah-ices08.pdf

</td> </tr> <tr> <td colspan="2">
Evolved creatures - self-intersection, Evolved creatures<br/>

AI Learns To Walk

</td> <td colspan="4">
Intended Goal: Walking speed<br>

Behavior: Creatures exploited a quirk in Box2D physics by clipping one leg into another to slide along the ground with phantom forces instead of walking<br>

Misspecified Goal: Velocity in a physics simulator

</td> <td>
Code Bullet, 2019<br/>

https://youtu.be/K-wIZuAA3EY?t=486

</td> </tr> <tr> <td colspan="2">
Evolved creatures - suffocation, Evolved creatures<br/>

0.11.0.9&10: All the Good Things

</td> <td colspan="4">
Intended Goal: Survive and reproduce, in a biologically plausible manner<br>

Behavior: A species in an artificial life simulation evolved a sedentary lifestyle that consisted mostly of mating in order to produce new children which could be eaten (or used as mates to produce more edible children) due to a bug<br>

Misspecified Goal: Survive and reproduce in a simulated evolution game

</td> <td>
Schumacher, 2018<br/>

https://speciesdevblog.wordpress.com/2018/10/04/0-11-0-910-all-the-good-things/

</td> </tr> <tr> <td colspan="2">
Evolved creatures - twitching, Evolved creatures<br/>

Evolved Virtual Creatures

</td> <td colspan="4">
Intended Goal: Swimming speed<br>

Behavior: Creatures exploited physics simulation bugs by twitching, which accumulated simulator errors and allowed them to travel at unrealistic speeds through the water<br>

Misspecified Goal: Maximize swimming speed in a physics simulator

</td> <td>
Sims, 1994<br/>

http://www.karlsims.com/papers/siggraph94.pdf

</td> </tr> </table>






## Attack Examples 
 
<a href="https://arxiv.org/abs/2307.10719">Mosaic Prompt : breakdown a prompt into permissible components</a>

* Users break down impermissible content into small permissible components.
* Each component is queried independently and appears harmless.
* User recombines components to reconstruct impermissible content.
* Exploits compositionality of language.

<img src="https://github.com/equiano-institute/attackspace/assets/25654848/6fa5e2bf-0ec6-4883-8815-08f5b1392a34" alt="Red Image" width="400" >


<a href="https://arxiv.org/abs/2310.02446">Cross-Lingual Attacks : translating between high and low-resource languages for attacking multi-lingual capability</a>

* The attack involves translating unsafe English input prompts into low-resource natural languages using Google Translate.
* Low-resource languages are those with limited training data, like Zulu.
* The translated prompts are sent to GPT-4, which then responds unsafely instead of refusing.
* The attack exploits uneven multilingual training of GPT-4's safety measures.


<img src="https://github.com/equiano-institute/attackspace/assets/25654848/32768877-4d99-44f1-a423-4044356ddac3" alt="Low Resource" width="400" >

 
### Prerequisites

- [Git](https://git-scm.com/)
- [Python](https://www.python.org/) (if applicable)

### Clone the Repository

```bash
git clone https://github.com/equiano-institute/attackspace.git
cd AttackSpace
```
