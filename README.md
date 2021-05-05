# AkropolisTestSession


As you might know, Akropolis is working with the Yearn protocol and develop strategies for Yearn Vaults.

1a. Measuring the ability to work with someone else's code
Let's take a look at the Yearn strategy pattern 

- https://github.com/yearn/yearn-vaults/blob/master/contracts/BaseStrategy.sol#L621

What is this function about? 
What is this function supposed to do? Try to explain what happens when you call this function
Describe the full workflow of calling this function, what is happening in the Vault, what is happening in the strategy itself, and debtOutstanding.


1b. Measuring the ability to understand a template
Let's imagine that there is some protocol (P). This protocol P gives a certain yield (Y) for liquidity provision, and also has its own liquidity mining (LM) functions, as well as additional reward tokens (R) that are accounted to balances each block.

How would you design a strategy based on the Yearn Vaults template in this case?


https://github.com/yearn/yearn-vaults/blob/master/contracts/BaseStrategy.sol#L621

   
The simplest strategy would be one which includes providing liquidity to P, receiving Y and R, and then reinvest income received in P at a regular basis in order to secure higher yield.



