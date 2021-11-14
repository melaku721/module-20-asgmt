# Module-20-asgmt
## Joint Saving Accounts - Solidity

In this Joint_saving.sol file we will see how to automate a joint saving accounts.
First we create or define all the variables as shown in the image below

![](SolCodeScsh/JScodeVar.png)

Define a function named Withdraw with a require statements that checks or confirm if the recipient is valid or not, and if there is a sufficient ballance to execute the transaction. Also defined contract balance, last withdraw amount and last to withdraw variables in this function.

![](SolCodeScsh/JScodeWfun.png)

The Dposit funtion that holds contract balance variable is defined as follows.

![](SolCodeScsh/JScodeDfun.png)

Defined another Set Accounts function to take the two adresses to create the joint accounts.

![](SolCodeScsh/JScodeSetAccfun.png)

Finally defined the fallback function to be executed when the functions above does not match any of the available functions in a smart contract or if there was no data supplied at all.

![](SolCodeScsh/JScodeFallbackfun.png)


* As  result after we complete the code we will compile and deploy the contract. All transactions excuted as shown below in this Excution Result section.

The green dot with the checkmarc indicates that compiled without error. And we have to check if we are in the right environment, correct network, account address, and if we are working on the right contract.

![](Execution_Results/JScompiled.png)

Once we confirm all the information is right after compilation we proceed to deploy the contract.

![](Execution_Results/JSdeployed.png)

Then we set the joint accounts by providing the account addresses for Account one and Account two.

![](Execution_Results/JSsetaccounts.png)

To test the functionality of the contract we will check the contract balance amount after we send ether of different amount in separate transactions. This time we use deposit function to send

Transaction 1: Sending 1 ether

![](Execution_Results/JSdTX1.png)

Transaction 2: Sending 10 ether

![](Execution_Results/JSdTX2.png)

Transaction 3: Sending 5 ether

![](Execution_Results/JSdTX3.png)

After we deposited funds successfully, we test the functionality of the contract's withdrawal by verifying the amount in the contract balance, the last to withdraw and the last withdraw amount.

Transaction 1: Withdraw 5 ether

![](Execution_Results/JSwTX1.png)

Transaction 2: Withdraw 10 ether

![](Execution_Results/JSwTX2.png)












