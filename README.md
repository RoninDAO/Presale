# This is meant to explain the functionalities of the smart contract

## Basic ERC20 interface Functions
line 1 to 79. this defines the standard interface that all ERC20 compliant tokens must implement
line 80 to 102 has optional metadata that can be implemented.

## Math functions
line 142 to 354, defines safe versions of solidity's math operators.

## ECR20 implementation
line 381 to 702 this is an implementation of the ERC20 interface mentionned above, nothing special here very standard

## Adress library function
line 708 to 918 this defines a few useful functions when dealing with adresses consult as needed

## Safe ECR20 functions
line 920 to 1011 defines safer versions of certain functions in the ECR20 implementation, basically wrapping the function calls to throw exceptions that can be caught in a `try {} catch` type statement.

## Crowdsale contract
line 1053 and beyond, This is the contract itself, some of the state variables that can be found here are the price of token, the min amount that can be spent, and the tiers as an enum.
some functions of note are :
TogglePresale:line 1123
TogglePublicsale 1127
SetWhitelistTiers: line 1132
ChangePrice : line 1152
deposit: line 1158
claim : line 1243

Further information of setWhitelistTiers
params : address[] : list of adresses
         Tiertype tier: 0 for public, 1 for ronin club members
