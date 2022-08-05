# FinTech_Unit_20_Joint_Savings_Account
A Solidity Smart Contract that automates hosting of joint savings accounts.


### Background

A fintech startup company has recently hired you. This company is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain that connects financial institutions. Currently, the team is building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts.

To automate the creation of joint savings accounts, you’ll create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. Your smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.


### Technologies

Remix Ethereum IDE

#### Step 1: Create a Joint Savings Account Contract in Solidity.

Please see Joint_savings.sol

#### Step 2: Compile and Deploy Your Contract in the JavaScript VM

![Successful deployment](Execution_Results/Step_3_1.png)

#### Step 3: Interact with Your Deployed Smart Contract

1. Use the `setAccounts` function to define the authorized Ethereum address that will be able to withdraw funds from your contract.

     > **Note** You can either use the following Ethereum addresses or create new, dummy addresses on the [Vanity-ETH](https://vanity-eth.tk/) website, which includes an Ethereum vanity address generator.
    >
    > ```text
    > Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb
    > Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0
    > ```
    
![setAccounts](Execution_Results/Step_3_1.png)

2. Test the deposit functionality of your smart contract by sending the following amounts of ether. After each transaction, use the `contractBalance` function to verify that the funds were added to your contract:

    * Transaction 1: Send 1 ether as wei.
    
![send 1ETH](Execution_Results/Step_3_2_1ETH.png)

    * Transaction 2: Send 10 ether as wei.
    
![send 10ETH](Execution_Results/Step_3_2_10ETH.png)

    * Transaction 3: Send 5 ether.
    
![send 5ETH](Execution_Results/Step_3_2_5ETH.png)

3. Once you’ve successfully deposited funds into your contract, test the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, use the `contractBalance` function to verify that the funds were withdrawn from your contract. Also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

5 ETH to Account 1 with verifications
![5 ether to account 1 with verifications](Execution_Results/Step_3_3_5ETHto1.png)

10 ETH to Account 2 with verifications
![10 ether to account 2 with verifications](Execution_Results/Step_3_3_10ETHto2.png)
