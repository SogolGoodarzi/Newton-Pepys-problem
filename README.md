# Newton-Pepys-problem
<p align="justify"> In 1693, English chronicler Samuel Pips wrote to Isaac Newton asking him to evaluate a probability problem about a bet. Samuel's question was "which of the following is more likely?" </p>

A. Six fair dice are tossed independently and at least one "6" appears.
B. Twelve fair dice are tossed independently and at least two "6"s appear.
C. Eighteen fair dice are tossed independently and at least three "6"s appear.

### Newton's Intuitive Explanation: 
<p align="justify"> After solving the problem correctly for Pepys, in order to give Pepys an intuition why A is more likely to occur than B and C, Newton told him to divide the dice of B and C into groups of 6. Now A occurs when a dice should come up as a six among the six dice, while this should happen to B and C in each of their packs of six. But he also knew that this talk is not accurate because it is possible that two numbers of 6 will come in the same category, and that is why it does not solve the problem. </p>

<p align="justify"> According to the explanation above, it can be said that this explanation cannot be correct because Newton divided the number of throws into groups of 6 with the assumption that 6 comes at least once in each group of 6. Now, according to his own words, it is possible for 6 to come twice or three times in the same category in B and C, as a result, it contradicts the assumption he made to intuitively justify the problem. So this analysis cannot be accepted. </p>

<p align="justify"> An effective solution that can be provided to solve this problem is to find a relationship to calculate the desired probability. Through the concept of complementation, we can calculate the probability of the states where the dice do not land 6 at least n times. The probability of these events follows the binomial distribution, so we have. </p>

![image](https://github.com/SogolGoodarzi/Newton-Pepys-problem/assets/125180530/b64ab555-3f1d-4b86-bbe4-728b23255289)

![image](https://github.com/SogolGoodarzi/Newton-Pepys-problem/assets/125180530/09678aa5-da74-4ed5-9e6c-e3848598f9c0)

So, in this way, the desired probability can be calculated correctly.

<p align="justify"> Now we generalize Pepys's problem. Let $P_{n}$ be the probability of seeing n to six in throwing 6n dice. Similar to the previous question, show that the values ​​of $P_{n}$ converge to 0.5. First, we write the relationship that is necessary to obtain the desired probability, which is as follows: </p>

![image](https://github.com/SogolGoodarzi/Newton-Pepys-problem/assets/125180530/dd014a7f-8606-4f53-804a-d54e18d22f78)

<p align="justify"> According to the above relationship, by writing a suitable program using this relationship, it is possible to show the probability that the values ​​of $P_{n}$ will converge to the value of 0.5 by plotting a graph. We checked the proof of convergence of the desired probability to the number 0.5 in the form of two cases. One is in the form of the general formula presented (the code was checked based on the formula obtained above and the result was obtained) and the other method is in the form of random events that simulate the throwing of dice in this state and in each throw, the program chooses a random numerical between 1 and 6 and finally the probability is calculated and its graph is plotted. The diagram obtained based on the above relationship is as follows: </p>

![image](https://github.com/SogolGoodarzi/Newton-Pepys-problem/assets/125180530/2d4b3157-87bd-481c-9a73-14c276a3c0fa)

Also, the diagram obtained based on the simulation is as follows:

![image](https://github.com/SogolGoodarzi/Newton-Pepys-problem/assets/125180530/979b476f-6ee4-4ac2-a628-84e2fc5e88b8)

In both graphs, it is clear that the value of probability convergence is 0.5.
