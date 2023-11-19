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



<tr> <td>
Ceiling, Genetic algorithm<br/>

Genetic Algorithm Physics Exploiting

</td> <td>
Intended Goal: Make a creature stick to the ceiling of a simulated environment for as long as possible</td>

<td>Behavior: Exploiting a bug in the physics engine to snap out of bounds</td>

<td>Misspecified Goal: Maximize the average height of the creature during the run</td>

</td> <td>
<a href="https://youtu.be/ppf3VqpsryU" > Higueras, 2015</a>

</td> </tr> <tr> <td>
CycleGAN steganography, GAN<br/>

CycleGAN, a Master of Steganography

</td> <td >
Intended Goal: Convert aerial photographs into street maps and back</td>

<td>Behavior: CycleGAN algorithm steganographically encoded output information in the intermediary image without it being humanly detectable</td>

<td>Misspecified Goal: Minimise distance between the original and recovered aerial photographs</td>

</td> <td>
<a href="https://arxiv.org/abs/1712.02950"> Chu et al, 2017
</a>
 
</td> </tr> <tr> <td >
Dying to Teleport, PlayFun<br/>

The First Level of Super Mario Bros. is Easy with Lexicographic Orderings and Time Travel

</td> <td>
Intended Goal: Play Bubble Bobble in a human-like manner</td>

<td>Behavior: The PlayFun algorithm deliberately dies in the Bubble Bobble game as a way to teleport to the respawn location, as this is faster than moving to that location in a normal manner.</td>

<td>Misspecified Goal: Maximize score</td>

</td> <td>
<a href="http://www.cs.cmu.edu/~tom7/mario/mario.pdf" > 
Murphy, 2013
</a>


</td> </tr> 
<tr> <td>
Eurisko - authorship, Genetic algorithm<br/>

Eurisko, The Computer With A Mind Of Its Own

</td> <td>
Intended Goal: Discover valuable heuristics</td>

<td>Behavior: Eurisko algorithm examined the pool of new concepts, located those with the highest "worth" values, and inserted its name as the author of those concepts</td>

<td>Misspecified Goal: Maximize the "worth" value of heuristics attributed to the algorithm</td>

</td> <td>
<a href="https://web.archive.org/web/20050308172043/http://www.aliciapatterson.org/APF0704/Johnson/Johnson.html">
 Johnson, 1984 
</a>


</td> </tr> 


 <tr> <td >
Eurisko - fleet, Genetic algorithm<br/>

Eurisko, The Computer With A Mind Of Its Own

</td> <td>
Intended Goal: Win games in the Trillion Credit Squadron (TCS) competition while playing within the 'spirit of the game'</td>

<td>Behavior: Eurisko algorithm created fleets that exploited loopholes in the game's rules,
 <br/> e.g. by spending the trillion credits on creating a very large number of stationary and defenseless ships</td>

<td>Misspecified Goal: Win games in the TCS competition</td>

</td> <td>
<a href="http://aliciapatterson.org/stories/eurisko-computer-mind-its-own" > Lenat, 1983</a> 

</td> </tr> <tr> <td>
Evolved creatures - clapping, Evolved creatures<br/>

Evolved Virtual Creatures

</td> <td>
Intended Goal: Maximize jumping height</td>

<td>Behavior: Creatures exploited a collision detection bug to get free energy by clapping body parts together</td>

<td>Misspecified Goal: Maximize jumping height in a physics simulator</td>

</td> <td>

 <a href="http://www.karlsims.com/papers/siggraph94.pdf" > 
 Sims, 1994</a>



</td> </tr> <tr> <td>
Evolved creatures - falling, Evolved creatures<br/>

Evolved Virtual Creatures

</td> <td>
Intended Goal: Develop a shape with a fast form of locomotion</td>

<td>Behavior: Creatures grow really tall and generate high velocities by falling over</td>

<td>Misspecified Goal: Maximize velocity</td>

</td> <td>
<a href="http://www.karlsims.com/papers/siggraph94.pdf"> Sims, 1994</a>
</td> </tr> <tr> <td>
Evolved creatures - floor collisions, Evolved creatures<br/>

Unshackling evolution: evolving soft robots with multiple materials and a powerful generative encoding

</td> <td>
Intended Goal: Maximize velocity</td>

<td>Behavior: Creatures exploited a coarse physics simulation by penetrating the floor between time steps without the collision being detected, which generated a repelling force, giving them free energy and producing an effective but physically impossible form of locomotion</td>

<td> Misspecified Goal: Maximize velocity in a physics simulator</td>

</td> <td>
<a href="http://jeffclune.com/publications/2013_Softbots_GECCO.pdf" > 
Cheney et al, 2013
</a>
</td> </tr> <tr> <td>
Evolved creatures - pole vaulting, Evolved creatures<br/>

Towards efficient evolutionary design of autonomous robots

</td> <td>
Intended Goal: Develop a shape capable of jumping</td>


<td>Behavior: Creatures developed a long vertical pole and flipped over instead of jumping</td>

<td>Misspecified Goal: Maximize the height of a particular block (body part) that was originally closest to the ground</td>

</td> <td>
<a href="http://artax.karlin.mff.cuni.cz/~krcap1am/ero/doc/krcah-ices08.pdf
" > Krcah, 2008<br/>

</a>

</td> </tr> <tr> <td>
Evolved creatures - self-intersection, Evolved creatures<br/>

AI Learns To Walk

</td> <td>
Intended Goal: Walking speed</td>

<td>Behavior: Creatures exploited a quirk in Box2D physics by clipping one leg into another to slide along the ground with phantom forces instead of walking</td>

<td> Misspecified Goal: Velocity in a physics simulator</td>

</td> <td>
<a href="
https://youtu.be/K-wIZuAA3EY?t=486">
 Code Bullet, 2019</a>


</td> </tr> <tr> <td>
Evolved creatures - suffocation, Evolved creatures<br/>

All the Good Things

</td> <td>
Intended Goal: Survive and reproduce, in a biologically plausible manner</td>

<td>Behavior: A species in an artificial life simulation evolved a sedentary lifestyle that consisted mostly of mating in order to produce new children which could be eaten (or used as mates to produce more edible children) due to a bug</td>

<td>Misspecified Goal: Survive and reproduce in a simulated evolution game</td>

</td> <td>

 <a href="
https://speciesdevblog.wordpress.com/2018/10/04/0-11-0-910-all-the-good-things/" >

 Schumacher, 2018</a>


</td> </tr> <tr> <td>
Evolved creatures - twitching, Evolved creatures<br/>

Evolved Virtual Creatures

</td>
<td>Intended Goal: Swimming speed</td>

<td>Behavior: Creatures exploited physics simulation bugs by twitching, which accumulated simulator errors and allowed them to travel at unrealistic speeds through the water</td>

<td>Misspecified Goal: Maximize swimming speed in a physics simulator</td>

</td> <td>

 <a href="http://www.karlsims.com/papers/siggraph94.pdf" >
 Sims, 1994</a>


</td> </tr> 
<tr> 
 <td>Football, Reinforcement learning</td> 
 <td>Intended Goal: Score a goal in a one-on-one situation with a goalkeeper.</td> 
 <td>Behavior: Rather than shooting at the goal, the player kicks the ball out of bounds.<br/> Someone from the other team has to throw the ball in (in this case the goalie), so now the player has a clear shot at the goal.</td> 
 <td>Score a goal (without any restriction on it occuring in the current phase of play)</td> 
 <td>Kurach et al, 2019 <a href="https://arxiv.org/abs/1907.11180">Google Research Football: A Novel Reinforcement Learning Environment [Presentation at AAAI]</a></td> </tr> <tr> 
  
  <td>Galactica, Language model</td> <td>Intended Goal: Assist scientists in writing papers by providing correct information. </td>
  
<td>Behavior: Galactica language model made up fake papers (sometimes attributing them to real authors)</td> <td>Assist scientists in writing papers</td> <td>Heaven, 2022<br/><a href="https://www.technologyreview.com/2022/11/18/1063487/meta-large-language-model-ai-only-survived-three-days-gpt-3-science/">Why Meta’s latest large language model survived only three days online</a></td> </tr> <tr> <td>Goal classifiers, Reinforcement learning</td> <td>Intended Goal: Use a robot arm to move an object to a target location</td> 
 <td>Behavior: The RL algorithm exploited a goal classifier by moving the robot arm in a peculiar way resulting in an erroneous high reward, since the classifier was not trained on this specific kind of negative example</td> <td>A goal classifier was trained on goal and non-goal images, and the success probabilities from this classifier were used as the task reward</td> <td>Singh, 2019<br/><a href="https://bair.berkeley.edu/static/blog/end_to_end/pr2_classifier.gif">End-to-End Deep Reinforcement Learning without Reward Engineering</a></td> </tr> <tr> <td>Go pass, Reinforcement learning</td> <td>Intended Goal: Win games of tic-tac-toe</td>
 <td>Behavior: A reimplementation of AlphaGo applied to Tic-tac-toe learns to pass forever</td> <td>Maximize the average score in games of tic-tac-toe, where a loss = -win, and pass is an available move</td> <td>Chew, 2019<br/><a href="https://youtu.be/nk87zsxpF1A?si=j1usw9yBbby_Al54&t=1864">A Funny Thing Happened On The Way to Reimplementing AlphaGo in Go</a></td> </tr> <tr> <td>Gripper, Evolutionary algorithm</td> <td>Intended Goal: Move a box using a robot arm without using the gripper</td> 
   <td>Behavior: MAP-Elites algorithm controlling a robot arm with a purposely disabled gripper found a way to hit the box in a way that would force the gripper open</td> <td>Move a box to a target location</td> <td>Ecarlat et al, 2015<br/><a href="http://www.isir.upmc.fr/files/2015ACTI3564.pdf">Learning a high diversity of object manipulations through an evolutionary-based babbling</a></td> </tr> 

  <tr> <td>Half Cheetah spinning, Reinforcement learning</td> <td>Intended Goal: Run quickly</td> <td>Behavior: Model-based RL algorithm exploits an overflow error in a mujoco environment to achieve high speed by spinning</td> <td>Maximum forward velocity in a physics simulator</td> <td>Zhang et al, 2021<br/><a href="https://arxiv.org/abs/2102.13651">On the Importance of Hyperparameter Optimization for Model-based Reinforcement Learning</a></td> </tr> <tr> <td>Hide-and-seek, Reinforcement learning</td> <td>Intended Goal: Win a hide-and-seek game within the laws of physics</td> <td>Behavior: Box surfing, endless running, ramp exploitation by hiders and seekers</td> <td>Win a hide-and-seek game in a physics simulator</td> <td>Baker et al, 2019<br/><a href="https://openai.com/blog/emergent-tool-use/#surprisingbehaviors">Emergent Tool Use from Multi-Agent Interaction</a></td> </tr> <tr> <td>Impossible superposition, Genetic algorithm</td> <td>Intended Goal: Find low-energy configurations of carbon which are physically plausible</td> <td>Behavior: Genetic algorithm exploits an edge case in the physics model and superimposes all the carbon atoms</td> <td>Find low-energy configurations of carbon in a physics model</td> <td>Lehman et al, 2018<br/><a href="https://arxiv.org/pdf/1803.03453.pdf">The Surprising Creativity of Digital Evolution</a></td> </tr> <tr> <td>Indolent Cannibals, Genetic algorithm</td> <td>Intended Goal: Survive and reproduce, in a biologically plausible manner</td> <td>Behavior: A species evolved a sedentary lifestyle of mating and eating/mating with offspring</td> <td>Survive and reproduce in a simulation where survival required energy but giving birth had no energy cost</td> <td>Yaeger, 1994<br/><a href="https://www.researchgate.net/profile/Larry_Yaeger/publication/2448680_Computational_Genetics_Physiology_Metabolism_Neural_Systems_Learning_Vision_and_Behavior_or_PolyWorld_Life_in_a_New_Context/links/0912f50e101b77ec67000000.pdf">Computational genetics, physiology, metabolism, neural systems, learning, vision, and behavior or Poly World: Life in a new context</a></td> </tr>
  
 <tr> <td>Lego stacking, Reinforcement learning</td> <td>Intended Goal: Stack a red block on top of a blue block</td> <td>Behavior: The agent flips the red block rather than lifting it and placing on top of the blue block</td> <td>Maximize the height of the bottom face of the red block</td> <td>Popov et al, 2017<br/><a href="https://arxiv.org/abs/1704.03073">Data-efficient Deep Reinforcement Learning for Dexterous Manipulation</a></td> </tr> <tr> <td>Line following robot, Reinforcement learning</td> <td>Intended Goal: Go forward along the path</td> <td>Behavior: A robot with three actions (go forward, turn left, turn right) learned to reverse along a straight section of a path by alternating left and right turns</td> <td>Stay on the path</td> <td>Vamplew, 2004<br/><a href="https://www.researchgate.net/publication/228953260_Lego_Mindstorms_Robots_as_a_Platform_for_Teaching_Reinforcement_Learning">Lego Mindstorms Robots as a Platform for Teaching Reinforcement Learning</a></td> </tr> <tr> <td>Logic gate, Genetic algorithm</td> <td>Intended Goal: Design a connected digital circuit for audio tone recognition</td> <td>Behavior: A genetic algorithm designed a circuit with a disconnected logic gate that was necessary for it to function (exploiting peculiarities of the hardware)</td> <td>Maximize the difference between average output voltage when a 1 kHz input is present and when a 10 kHz input is present</td> <td>Thompson, 1997<br/><a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.50.9691&rep=rep1&type=pdf">An evolved circuit, intrinsic in silicon, entwined with physics</a></td> </tr> <tr> <td>Long legs, Reinforcement learning</td> <td>Intended Goal: Reach the goal by walking</td> <td>Behavior: An agent that could modify its own body learned to have extremely long legs that allowed it to fall forward and reach the goal without walking</td> <td>Reach the goal</td> <td>Ha, 2018<br/><a href="https://designrl.github.io/">RL for improving agent design</a></td> </tr> <tr> <td>Minitaur, Evolutionary algorithm</td> <td>Intended Goal: Walk while balancing the ball on the robot's back</td> <td>Behavior: Four-legged robot learned to drop the ball into a hole in its leg joint and then walk across the floor without the ball falling out</td> <td>Walk without dropping the ball on the ground</td> <td>Otoro, 2017<br/><a href="http://blog.otoro.net/2017/11/12/evolving-stable-strategies/">Evolving stable strategies</a></td> </tr> <tr> <td>Model-based planner, Reinforcement learning</td> <td>Intended Goal: Maximize performance within a real environment</td> <td>Behavior: RL agents using learned model-based planning paradigms such as model predictive control exploit the learned model by choosing a plan going through the worst-modeled parts of the environment and producing unrealistic plans</td> <td>Maximize performance within a learned model of the environment</td> <td>Mishra et al, 2017<br/><a href="https://arxiv.org/abs/1703.04070">Prediction and Control with Temporal Segment Models</a></td> </tr>
 
 <tr> <td>Molecule design, Bayesian optimization</td> <td>Intended Goal: Find molecules that bind to specific proteins</td> <td>Behavior: Bayesian optimizer finds unrealistic molecules that are valid according to the computed score</td> <td>Maximize a human-designed "log P" score accounting for synthesizability of the molecule and binding fitness based on a simulation on the space of molecules</td> <td>Maus et al. 2023<br/>"Local Latent Space Bayesian Optimization over Structured Inputs"</td> </tr> <tr> <td>Montezuma's Revenge - key, Reinforcement learning</td> <td>Intended Goal: Maximize score within the rules of the game</td> <td>Behavior: The agent learns to exploit a flaw in the emulator to make a key re-appear</td> <td>Maximize score</td> <td>Salimans & Chen, 2018<br/><a href="https://openai.com/research/learning-montezumas-revenge-from-a-single-demonstration">Learning Montezuma’s Revenge from a Single Demonstration</a></td> </tr> <tr> <td>Montezuma's Revenge - room, Reinforcement learning</td> <td>Intended Goal: Win the game (by completing all of the levels)</td> <td>Behavior: Go Explore agent learns to exploit a bug and remain in the treasure room indefinitely to collect unlimited points</td> <td>Maximize score</td> <td>Ecoffet et al, 2019<br/><a href="https://arxiv.org/abs/1901.10995">Go-Explore: a New Approach for Hard-Exploration Problems</a></td> </tr> <tr> <td>Negative sentiment, Language model</td> <td>Intended Goal: Produce text which is both coherent and not offensive</td> <td>Behavior: Model optimized for negative sentiment while preserving natural language</td> <td>Generate coherent text that maximizes positive human feedback</td> <td>Ziegler et al, 2019<br/><a href="https://arxiv.org/abs/1909.08593">Fine-Tuning Language Models from Human Preferences</a></td> </tr>

<tr> <td>Oscillator, Genetic algorithm</td> <td>Intended Goal: Design an oscillator circuit</td> <td>Behavior: Genetic algorithm designs radio that produces an oscillating pattern by picking up signals from neighboring computers</td> <td>Design a circuit that produces an oscillating pattern</td> <td>Bird & Layzell, 2002<br/><a href="https://people.duke.edu/~ng46/topics/evolved-radio.pdf">The Evolved Radio and its Implications for Modelling the Evolution of Novel Sensors</a></td> </tr> <tr> <td>Overkill, Reinforcement learning</td> <td>Intended Goal: Proceed through the levels (floors) in the Elevator Action ALE game</td> <td>Behavior: The agent learns to stay on the first floor and kill the first enemy over and over to get a small amount of reward</td> <td>Maximize score</td> <td>Toromanoff et al, 2019<br/><a href="https://arxiv.org/abs/1908.04683">Is Deep Reinforcement Learning Really Superhuman on Atari? Leveling the playing field</a></td> </tr> <tr> <td>Pancake, Reinforcement learning</td> <td>Intended Goal: Flip pancakes</td> <td>Behavior: Simulated pancake making robot learned to throw the pancake as high in the air as possible</td> <td>Time the pancake spends away from the ground</td> <td>Unity, 2018<br/><a href="https://blog.unity.com/news/introducing-the-winners-of-the-first-ml-agents-challenge">Pass the Butter // Pancake bot</a></td> </tr> <tr> <td>Pinball nudging, Reinforcement learning</td> <td>Intended Goal: Play pinball by using the provided flippers</td> <td>Behavior: DNN agent moves the ball to trigger a high-scoring switch infinitely without tilting the table</td> <td>Maximize score in a virtual pinball game</td> <td>Lapuschkin et al, 2019<br/><a href="https://www.nature.com/articles/s41467-019-08987-4">Unmasking Clever Hans predictors and assessing what machines really learn</a></td> </tr> <tr> <td>Player Disappearance, PlayFun</td> <td>Intended Goal: Play a hockey video game within the rules of the game</td> <td>Behavior: When about to lose, the PlayFun algorithm exploits a bug to make an opposing player disappear, forcing a draw</td> <td>Play a hockey video game in a simulated environment</td> <td>Murphy, 2014<br/><a href="https://www.youtube.com/watch?v=Q-WgQcnessA&t=1450s">NES AI Learnfun & Playfun, ep. 3: Gradius, pinball, ice hockey, mario updates, etc.</a></td> </tr> 

<tr> <td>Playing dead, Evolved organisms</td> <td>Intended Goal: Eliminate mutations which increased the replication rate of evolutionary agents</td> <td>Behavior: The organisms evolved to "play dead" in the test environment or probabilistically accelerate replication to slip through</td> <td>After each mutation, measure and delete mutants replicating faster than parents</td> <td>Wilke et al, 2001<br/><a href="https://www.nature.com/articles/35085569">Evolution of digital organisms at high mutation rates leads to survival of the flattest</a></td> </tr> <tr> <td>Power-seeking, Language model</td> <td>Intended Goal: Produce helpful, honest and harmless text</td> <td>Behavior: Larger LMs and RLHF models more often indicate willingness to pursue dangerous subgoals like power seeking</td> <td>Generate coherent text that maximizes positive human feedback</td> <td>Perez et al, 2023<br/><a href="https://arxiv.org/abs/2212.09251">Discovering Language Model Behaviors with Model-Written Evaluations</a></td> </tr> <tr> <td>Program repair - sorting, Genetic algorithm</td> <td>Intended Goal: Debug a program that sorts a list</td> <td>Behavior: GenProg made the program output an empty list, considered sorted</td> <td>Produce an output list which is in sorted order</td> <td>Weimer, 2013<br/><a href="https://web.eecs.umich.edu/~weimerw/p/weimer-ssbse2013.pdf">Advances in Automated Program Repair and a Call to Arms</a></td> </tr> <tr> <td>Program repair - files, Genetic algorithm</td> <td>Intended Goal: Debug a program to produce correct output</td> <td>Behavior: GenProg learned to delete the target output file and output nothing</td> <td>Minimize difference between program output and target output file</td> <td>Weimer, 2013<br/><a href="https://web.eecs.umich.edu/~weimerw/p/weimer-ssbse2013.pdf">Advances in Automated Program Repair and a Call to Arms</a></td> </tr> 

 <tr> <td>Qbert - cliff, Evolutionary algorithm</td> <td>Intended Goal: Play Qbert in a human-like manner</td> <td>Behavior: Agent baits opponent off cliff for infinite extra lives</td> <td>Maximize score</td> <td>Chrabaszcz et al, 2018<br/><a href="https://arxiv.org/abs/1802.08842">Back to Basics: Benchmarking Canonical Evolution Strategies for Playing Atari</a></td> </tr> <tr> <td>Qbert - million, Evolutionary algorithm</td> <td>Intended Goal: Play Qbert within the game rules</td> <td>Behavior: Agent exploits in-game bug for unlimited points</td> <td>Maximize score</td> <td>Chrabaszcz et al, 2018<br/><a href="https://arxiv.org/pdf/1802.08842.pdf">Back to Basics: Benchmarking Canonical Evolution Strategies for Playing Atari</a></td> </tr> <tr> <td>Reward modeling - Hero, Reward modeling</td> <td>Intended Goal: Maximize game score</td> <td>Behavior: Agent repeatedly shoots but misses spider</td> <td>Maximize output from learned reward model</td> <td>Ibarz et al, 2018<br/><a href="https://arxiv.org/abs/1811.06521">Reward learning from human preferences and demonstrations in Atari</a></td> </tr> <tr> <td>Reward modeling - Montezuma's Revenge, Reward modeling</td> <td>Intended Goal: Maximize game score</td> <td>Behavior: Agent repeatedly moves towards key without grabbing</td> <td>Maximize output from learned reward model</td> <td>Ibarz et al, 2018<br/><a href="https://arxiv.org/abs/1811.06521">Reward learning from human preferences and demonstrations in Atari</a></td> </tr> <tr> <td>Reward modeling - Pong, Reward modeling</td> <td>Intended Goal: Maximize game score</td> <td>Behavior: Agent bounces ball without scoring</td> <td>Maximize output from learned reward model</td> <td>Christiano et al, 2017<br/><a href="https://deepmind.com/blog/learning-through-human-feedback/">Deep reinforcement learning from human preferences</a></td> </tr> 

  <tr> <td>Reward modeling - Private Eye, Reward modeling</td> <td>Intended Goal: Maximize game score</td> <td>Behavior: Agent repeatedly looks left and right</td> <td>Maximize output from learned reward model</td> <td>Ibarz et al, 2018<br/><a href="https://arxiv.org/abs/1811.06521">Reward learning from human preferences and demonstrations in Atari</a></td> </tr> <tr> <td>Road Runner, Reinforcement learning</td> <td>Intended Goal: Play Road Runner to a high level</td> <td>Behavior: Agent kills itself to avoid losing</td> <td>Maximize score</td> <td>Saunders et al, 2017<br/><a href="https://owainevans.github.io/blog/hirl_blog.html">Trial without Error: Towards Safe RL with Human Intervention</a></td> </tr> <tr> <td>Robot hand, Reward modeling</td> <td>Intended Goal: Grasp an object</td> <td>Behavior: Agent tricked evaluator by hovering hand</td> <td>Maximize human feedback on grasping</td> <td>Christiano et al, 2017<br/><a href="https://openai.com/research/learning-from-human-preferences">Deep reinforcement learning from human preferences</a></td> </tr> <tr> <td>ROUGE summarization, Language model</td> <td>Intended Goal: Produce high-quality summaries</td> <td>Behavior: ROUGE-only model produced gibberish</td> <td>Maximize ROUGE score</td> <td>Paulus et al, 2017<br/><a href="https://arxiv.org/abs/1705.04304">A Deep Reinforced Model for Abstractive Summarization</a></td> </tr> <tr> <td>Running gaits, Reinforcement learning</td> <td>Intended Goal: Learn human-like running</td> <td>Behavior: Model learned unusual gaits like hopping to maximize reward</td> <td>Optimize model's running distance</td> <td>Kidziński et al, 2018<br/><a href="https://arxiv.org/abs/1804.00361">Learning to Run challenge solutions: Adapting reinforcement learning methods for neuromusculoskeletal environments</a></td> </tr> 
  
 <tr> <td>Soccer, Reinforcement learning</td> <td>Intended Goal: Gain possession of the ball</td> <td>Behavior: Agent learned to vibrate on the ball for shaping reward</td> <td>Maximize shaping reward for touching ball</td> <td>Andrew and Teller, cited in Ng et al, 1999<br/><a href="http://luthuli.cs.uiuc.edu/~daf/courses/games/AIpapers/ng99policy.pdf">Policy Invariance under Reward Transformations</a></td> </tr> <tr> <td>Sonic, Reinforcement learning</td> <td>Intended Goal: Play Sonic to a high level</td> <td>Behavior: Agent exploits level walls for higher score</td> <td>Maximize score in simulated environment</td> <td>Christopher Hesse et al, 2018<br/><a href="https://blog.openai.com/retro-contest/">OpenAI Retro Contest</a></td> </tr> <tr> <td>Strategy game crashing, Genetic algorithm</td> <td>Intended Goal: Play a strategy game</td> <td>Behavior: Crashing game gave advantage in genetic selection</td> <td>Maximize score in simulated game</td> <td>Salge et al, 2008<br/><a href="https://cs.pomona.edu/~mwu/CourseWebpages/CS190-fall15-Webpage/Readings/2008-Gameplaying.pdf">Using Genetically Optimized Artificial Intelligence to improve Gameplaying Fun for Strategical Games</a></td> </tr> <tr> <td>Superweapons, Unknown</td> <td>Intended Goal: Play Elite Dangerous within rules</td> <td>Behavior: AI exploited bug to craft overpowered weapons</td> <td>Play Elite Dangerous game</td> <td>Sandwell, 2016<br/><a href="https://www.digitalspy.com/videogames/a796635/elite-dangerous-ai-super-weapons-bug/">Elite's AI created super weapons to hunt down players</a></td> </tr> <tr> <td>Sycophancy, Language model</td> <td>Intended Goal: Produce helpful, honest, harmless text</td> <td>Behavior: LMs showed more agreement with user's views</td> <td>Generate text resembling training data</td> <td>Perez et al, 2023<br/><a href="https://arxiv.org/abs/2212.09251">Discovering Language Model Behaviors with Model-Written Evaluations</a></td> </tr> <tr> <td>Tetris pass, PlayFun</td> <td>Intended Goal: Play Tetris in a human-like manner</td> <td>Behavior: Algorithm pauses game indefinitely to avoid losing</td> <td>Maximize score</td> <td>Murphy, 2013<br/><a href="http://www.cs.cmu.edu/~tom7/mario/mario.pdf">The First Level of Super Mario Bros. is Easy with Lexicographic Orderings and Time Travel</a></td> </tr> 
 
 <tr> <td>Tic-tac-toe memory bomb, Evolutionary algorithm</td> <td>Intended Goal: Win tic-tac-toe games within rules</td> <td>Behavior: Player makes invalid moves to cause opponent to crash</td> <td>Win tic-tac-toe games on infinite board</td> <td>Lehman et al, 2018<br/><a href="https://arxiv.org/abs/1803.03453">Surprising Creativity of Digital Evolution</a></td> </tr> <tr> <td>Tigers, Diffusion model</td> <td>Intended Goal: Produce images reflecting user prompts</td> <td>Behavior: Model produces "five tigers" text instead of tigers</td> <td>Produce images that reflect user prompts</td> <td>Black et al, 2023<br/><a href="https://rl-diffusion.github.io/">Training Diffusion Models with Reinforcement Learning</a></td> </tr> <tr> <td>Timing attack, Genetic algorithm</td> <td>Intended Goal: Classify images by content</td> <td>Behavior: Algorithm infers labels from storage location</td> <td>Classify images correctly</td> <td>Ierymenko, 2013<br/><a href="https://news.ycombinator.com/item?id=6269114">Hacker News comment on "The Poisonous Employee-Ranking System That Helps Explain Microsoft’s Decline”</a></td> </tr> <tr> <td>Walker, Reinforcement learning</td> <td>Intended Goal: Walk at target speed</td> <td>Behavior: Agent learns to walk with only one leg</td> <td>Move at a target speed</td> <td>Lee et al, 2021<br/><a href="https://arxiv.org/abs/2106.05091">PEBBLE: Feedback-Efficient Interactive Reinforcement Learning via Relabeling Experience and Unsupervised Pre-training</a></td> </tr> <tr> <td>Walking up walls, Evolutionary algorithm</td> <td>Intended Goal: Navigate environment with walls naturally</td> <td>Behavior: Robots exploit physics bug to wiggle up walls</td> <td>Navigate simulated environment with walls</td> <td>Stanley et al, 2005<br/><a href="http://ieeexplore.ieee.org/document/1545941/">Real-time neuroevolution in the NERO video game</a></td> </tr> </table>



