# Computational-Intelligence
Personal repository for computational intelligence 2023-2024

**10/04/2023**
-
- Tried to the virtual environment locally in my pc.

**10/12/2023**
- 
- Trying different queues during the cancelled class of the following date.

**10/25/2023**
-
- Created and set up the personal repository for the computational intellignece 2023/2024
- Looked at some codes of my colleagues repositories and how they have done the set covering.
- Started doing some heuristic for the first lab.

**10/26/2023**
-
- Thought a seemingly optimisitc way with the help of my colleagues
- Finished the first lab.
- Pushed the lab to the repoitory

**10/27/2023**
-
- Place the repository link in the google document professor has provided.

**11/03/2023**
-
- Understanding how the halloween challenged works by with a collegue

**11/06/2023**
-
- Trying to figure out lab 2's agginment
- Playing the nim sum game and figuring out how does it work

**11/11/2023**
- 
- Try to understand deeper the theories which might be needed for lab 2 
- Working on a solution for lab 2 

**11/13/2023**
-
- Figuring out an optimal solution for lab 2
- Coding the population and fitness with a few of my collegues 

**11/14/2023**
-
- Finalization of lab 2 as we got to a perfect score

**11/17/2023**
--
- Committing lab 2 to the github repository
- Updating the log

**11/22/2023**
-- 
- Studying theory necessities for Lab 9 with some collegues 

**11/23/2023**
--
- Writing Some peer reviews of Lab 2 for two of my collegues 
- Asking some of my collegues to write a peer review of Lab 2 for me if they have the time

**11/24/2023**
--
- Implementing the basics of the Lab 9 with some collegues without major tests

**11/27/2023**
--
- Testing the Lab 9 implemnetation and tried to reduce the number of calls to the fitness by reducing the number of generations/offspring size only to ES with collegues

**11/28/2023**
--
- Searching and understanding out the classic genetic algorithm used for AI learning to play Google Chrome Dinosaur Game.
Each generation contains 500 individuals, the individuals which do the best live on to mutate for the next generations until you have an optimal solution which in this case is a dinosaur which can do a big jump, small jump and duck perfectly. In other words, we have a dinosaur which can't die.
The genotype in this scenario would represent the set of parameters or weights that define the neural network controlling the behavior of the dinosaur. If you use a neural network to control the dinosaur's actions (like jumping or ducking), the genotype would consist of the weights and biases of the neural network connections.
The phenotype, in this case, is the actual behavior of the dinosaur in the game as a result of applying the neural network specified by its genotype. It represents how well the dinosaur is able to play the game.
The phenotype is evaluated based on the performance of the dinosaur, such as how far it runs, how many obstacles it avoids, and how long it survives. The fitness function would quantify these aspects of performance.
    Initialization:
        In the first generation, you randomly generate 500 individuals, each with its own set of neural network weights (genotype).

    Evaluation:
        Each individual's phenotype is determined by letting the corresponding neural network control the dinosaur in the game. The performance of each dinosaur is measured using a fitness function, which could be based on factors like the distance covered, obstacles avoided, and survival time.

    Selection:
        The top-performing individuals (those with the best phenotypes) are selected to pass their genotypes to the next generation. This could be, for example, the top 10% of individuals.

    Crossover and Mutation:
        Crossover and mutation operations are applied to the genotypes of the selected individuals to create the next generation. Crossover involves combining the genetic information of two parents, and mutation introduces small random changes to the genotypes.

    Repeat:
        The process is repeated for multiple generations. Over time, the genotypes are fine-tuned through the selection, crossover, and mutation operations, leading to the evolution of a neural network that performs well in the game.

The goal is to evolve a genotype (set of neural network weights) that produces a phenotype (dinosaur behavior) that excels in playing the Google Chrome Dinosaur Game, gradually improving over generations until a highly effective strategy is discovered

**12/03/2023**
--
- Finalizing the Lab 9 implementation and pushing it on the github repository

**12/07/2023**
--
- Attending the lecture to understand the project of the course and later on discussing it with some collegues and what is necessary to be done regarding the project
- Studying the theory about Promoting Diversity for the rest of the days with collegues and catching up with essential topics

**12/10/2023**
--
- Writing some peer reviews of Lab 9 for three of my collegues 
- Asking some of my collegues to write a peer review of Lab 9 for me if they have the time

**12/14/2023**
--
- Study the theory regarding Adversarial Search and Reinforcement Learning slides with some collegues from morning until before the class starts

**12/15/2023**
--
- Reviewing the theory relating to Reinforcement Learning 
- Discussing the solution of the porfessor regarding the Lab 10

**12/18/2023**
--
- Meeting online with the usual collegues to study the slides if Reinforcement Learning and finishing it
- Discussing a little more about the Lab 10 and deciding on how to expand it
The ideas for now are: 
1) adding action-value function
2) adding Hybdrid Montecarlo simulation with full game simulation

**12/20/2023**
--
- Implementing the discussed ideas previously with collegues on an online meeting call for Lab 10 and acheiving good results on the same day

**12/22/2023**
-- 
- Continuing with the Theory, closing the Knowledge-based agent alongside with Multi-agent systems and Swarm Intelligence with the contribution of my collegues on an online call, discussing the matters accordingly together while reviewing the subjects

**12/24/2023**
--
- Adding the results of the tests running and some comments for Lab 10 as the finishing touches

**12/25/2023**
--
- Lab 10 Commit
- Updating the log

**12/27/2023**
-- 
- Me and my teammates organized a meeting to start the Quixo project.
- We talked about a way to add another player by extending it in the main
- We decided to go further with the MixMax strategy.
- Self.minmax returns the player and the best move for the player and in the end we want to return none because no one is playing.
- Random player's move is never invalid even though if it is random there's always a check (so we should print for each valid move where the player can do the move not that the fact for some reason (like the position is occupied) it can't do the move)
- Since minmax is deterministic, it can't change it's function so it's forever going to do the invalid move.
- the first player is minmax and the second player is random.
- We have to set a limit because the game is too long and the random player is stupidly winning. 
- We can think about Alpha-Beta pruning.
- An idea: in the non-terminal state if there are many 0, we are winning and if there are many 1 we are losing. You kinda push the play to pick any cube with an empty cell rather than a taken one because if you take the ones with symbols you have to change it to yours. It would be an even distribution if we try this method (choosing empty slots).

**12/28/2023**
--
- Me and my teammates set up another meeting to think of doing other strategies - Same MinMax as before but with Alpha-Beta pruning 
- alpha is the last value we take for the max player and beta is the last value we take for the min player.
- The second player still plays random
- Idea: when you reach a limit of subtree, instead of stopping, if the subtree is intersting, continue the exploring instead of stopping. The computational would for sure is higher but it would acheive good results. e.g. if there are 4 that are really close, continue more.
- Our MinMax approach with Alpha-Beta pruning apruning works perfectly with 96% chance of winning in 100 games
- Next working algorithm: Reinforcement Learining.
- We train action value function 
- We need to increase the reward in every zero the we find.
- Epsilon is the weight of the change, if there's too much winning or losing you don't want to go back and forth but you just want to change it a bit.
- We have a value 0 which is losing and 1 which is win, we will count the difference which is 1 so we will change to 0.01 and 1 and then do it again in the next iteration
- There are states we need in a certain situation that we won and the action in that situation.
- Each time we calculate the reward for a certain action, if it is better than the previous reward, we replace the reward until we find the max reward for an action
- We want to see what number of iteration is the best, for now we will need a lot. The problem here is the opponent but that fact that we are not exploring.


**01/05/2024**
--
- Writing some peer reviews of Lab 10 for three of my collegues.
- Asking some of my collegues to write a peer review of Lab 10 for me if they have the time.

**01/06/2024**
--
- Me and my teammates set the third meeting to continue with the Quixo Project. 
- We increased the learning rate, we will have to keep training with different number of iterations to see what would be it more optimized.
- We each tried with different numbers of epsilon to see whether we can reach better numbers of winning or not but the results are really low (maximum winning was 20%)
- Idea: Maybe moving from monte carlo to a more in depth analysis. Other than that, I think that we could also think about a way to improve the RL agent.
- One of my teammtes proposed EA as the alternative to RL. He also said that he will discuss the problem with a friend of his that is doing the project until further update for doing the rest of the project.


**01/07/2024**
--
- We discussed our problem with some collgegue about the MonteCarlo problem we have for thw Quixo project. She got 80% winnings against the random player. She also made an action value function, similar to us so we just have to see if we can improve our action value function.

**01/09/2024**
--
- Me and my teammates met before the class for the Quixo project to discuss a way of updating our reinforcement algorithm for the Quixo project.
- We decided to go on with Reinforcement Learning with Monte-Carlo and parallelization.

**01/10/2024**
--
- For MinMax solution of the Quixo project the game 50 out of 50 times
The problem is that with the new check_winner now is very slow and with the depth = 3 (no alpha beta) it took 107 minutes for 50 games but we I kinda found a solution with depth equal to 2 it takes way less time (5 min for 100 games) and we are still winning a lot (100 out of 100 times)

**01/20/2024**
-- 
- Restarting with the Theory with some of my collegues (Now we are going back to the beginning if the course and doing the earlier topics regarding Evolutionary Strategies (ES) and Evolutionary Programming (EP))
- By the request of my teammates, it was decided that I should train our agent for many iterations as possible and reload the dictionary later to update it by retraining and in the end, use the same file to test the agent against the random.

**01/21/2024**
-- 
- Continuing with the theory with some of my collegues (Regarding Evolutionary Programming (EP) and Classical EP)

**01/22/2024**
-- 
- After running some tests with my computer, me and my teammates realized that solving the Quixo project while using RL is unfeasible due to the branching factor of the tree
- Thus after a million iterations and a 5GB file the winnings were a bit above 30%
- Typically we could say that we are done with the project

**01/27/2024**
-- 
- Me and my usual collegues organzied a meeting to meet in person and finalize the remanant of the theory that has left and close the chapter of reviewing the course topics.

**01/28/2024**
--
- Me and my teammates (Whom I worked with for almost all labs + quixo project) planned a meeting to wrap up what we want to put for our reports in the sections in which we worked together. 
- We did the report for Lab 2 and Lab 9

**01/29/2024**
--
- Continuing and finalizing the wrap up of the report together with my collegues. 
- We did the report for Lab 10 and Quixo Project and finished the sections we did together.

**01/31/2024**
--
- Continuing the report (The remaining parts were Lab 1 and all of the reviews received/issued)
- Pushed all the files of Quixo project into my repository

**02/01/2024**
--
- Finalizing the report (The remaining parts were Lab 1 and all of the reviews received/issued)
- Sent an email to the porfessor for the report
- Finalizing the log
- Last Commit
