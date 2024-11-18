#MyToken Smart Contract

## Overview
MyToken is a simple smart contract built using remix. It implements a basic token system with features for minting and burning tokens. This contract demonstrates how to manage token balances and a total supply of tokens.


##Features
#Token Details

Name: LAYI
Symbol: LAY
Total Supply: Initially set to 0.
##Token Minting:
A function to increase the total supply of tokens and add the corresponding value to a specified address.

##Token Burning:
A function to reduce the total supply of tokens and deduct the corresponding value from a specified address, with checks to ensure the sender's balance is sufficient.


# Requirements
## Public Variables
The contract includes the following public variables:

name: Stores the name of the token.
symbol: Stores the token abbreviation.
totalSupply: Tracks the total supply of the token.
Balances Mapping
The contract maintains a mapping balances to associate Ethereum addresses with their respective token balances.

##Functions
mint(address account, uint256 value)
Purpose: Adds tokens to the total supply and credits them to the specified address.

##Parameters:
account: The Ethereum address to receive the tokens.
value: The amount of tokens to mint.

##Behavior:
Increases totalSupply by value.
Increases the balance of account by value.


burn(address account, uint256 value)
Purpose: Reduces the total supply of tokens and deducts them from the specified address.

##Parameters:
account: The Ethereum address to burn tokens from.
value: The amount of tokens to burn.
Behavior:
Ensures the balance of account is greater than or equal to value.
Decreases totalSupply by value.
Decreases the balance of account by value.
