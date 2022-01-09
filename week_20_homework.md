# Week20 Homework

## Smart contracts built with Solidity
I created three contracts to automate company finances.


### AssociateProfitSplitter contract
This will accept Ether into the contract and divide the Ether evenly among the associate level employees. This will allow the Human Resources department to pay employees quickly and efficiently.

![first contract](/photos/first_code.png)

The contract is deployed.

![first deploy](photos/first_deploy.png)

The contract was deployed successfully.

![first deploy success](photos/first_deply_success.png)

Depossit function is called.  60000 Wei is distributed to three addresses.

![first deposit call](photos/first_deposit.png)

Deposit funcation call was successful.  Each address received 20000 Wei.

![first deposit success](photos/first_deposit_success.png)

The balance of the contract is checked.  The balance is 0.

![first check balance](photos/first_balance.png)


### TieredProfitSplitter 
This will distribute different percentages of incoming Ether to employees at different tiers/levels. For example, the CEO gets paid 60%, CTO 25%, and Bob gets 15%.

![second contract](photos/second_code.png)

The contract is deployed.

![second deploy](photos/second_deploy.png)

The contract was deployed successfully.

![second deploy success](photos/second_deploy_success.png)

Depoist function is called.  100000 Wei is ditributed to three addresses in differenct proportions (50%, 25% and 20%).

![second deposit call](photos/second_deposit.png)

Deposit function call was successful. Employees one, two and three reiceived their portions out of 100000 Wei.  The remainder was received by emplyee one.

![second deposit success](photos/second_deposit_success.png)

The balance of the contract is checked. The balance is 0.

![second check balance](photos/second_balance.png)


### DeferredEquityPlan 
This models traditional company stock plans. This contract will automatically manage 1000 shares with an annual distribution of 250 over 4 years for a single employee.

![third contract](photos/third_code.png)

The contract is deployed.  The deployed contract has a fastfoward function added which fastforwards time by 365 days. So we don't need to wait for 365 days to test the contract!

![third deploy](photos/third_deploy.png)

The contact was deployed successfully.

![third deploy success](photos/third_deploy_sucess.png)

Tha balance is checked before distribution.

![balance checked](photos/third_distribution_0.png)

Fastforwarded 365 days and the emplyee is entitled for the first distribution.

![first fastforward](photos/third_ff_1.png)

The first distribution was made.

![first distribution](photos/third_dist1_success.png)

The balance is checked.

![first distribution checked](photos/third_distribution_1.png)

Fastforwarded 365 days again and the emplyee is entitled for the second distribution.

![second fastforward](photos/third_ff_2.png)

The second distribution was made.

![second distribution](photos/third_dist2_success.png)

The balance is checked.

![second distribution checked](photos/third_distribution_2.png)

Fastforwarded 365 days again and the emplyee is entitled for the third distribution.

![third fastforward](photos/third_ff_3.png)

The third distribution was made.

![third distribution](photos/third_dist3_success.png)

The balance is checked.

![third distribution checked](photos/third_distribution_3.png)

Fastforwarded 365 days again and the emplyee is entitled for the fourth distribution.

![fourth fastforward](photos/third_ff_4.png)

The fourth distribution was made.

![fourth distribution](photos/third_dist4_success.png)

The balance is checked.

![fourth distribution checked](photos/third_distribution_4.png)

Fastfowarded 365 days again and see what happens...

![fifth fastforward](photos/third_ff_5.png)

Distribution is called.  But it generated error as the full distribution of 1000 was already made.

![error](photos/error.png)
