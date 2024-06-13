# EVM-assessment
Introduction
MyToken is a simple ERC-20 compatible token smart contract implemented in Solidity. The contract allows for the creation, minting, and burning of tokens. This README provides an overview of the contract, including its features and how to interact with it.

Features
Public Variables:

tokenName: Stores the name of the token ("META").
tokenAbbrv: Stores the abbreviation of the token ("MTA").
totalSupply: Stores the total supply of the token.
Mapping:

balances: A mapping of addresses to their respective token balances.
Mint Function:

Increases the total supply of the token.
Increases the balance of the specified address by the given value.
Burn Function:

Decreases the total supply of the token.
Decreases the balance of the specified address by the given value.
Includes a check to ensure that the balance of the sender is greater than or equal to the amount to be burned.
Interacting with the Contract
Deploying the Contract
Compile the Contract: Use a Solidity compiler (e.g., Remix, Truffle) to compile the MyToken contract.
Deploy the Contract: Deploy the compiled contract to an Ethereum network (e.g., Mainnet, Ropsten, Ganache).
Using the Functions
Minting Tokens:

Call the mint function with the recipient address and the amount of tokens to mint.
Example: mint(0xRecipientAddress, 100)
Burning Tokens:

Call the burn function with the address and the amount of tokens to burn.
Ensure the address has a balance greater than or equal to the amount to burn.
Example: burn(0xAddress, 50)
Viewing Balances and Total Supply
Total Supply: Access the totalSupply variable to view the current total supply of tokens.
Balances: Access the balances mapping with an address to view the balance of that address.
Example: balances(0xAddress)
