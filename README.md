# Openzeppelin Token (ZenoToken)

## Overview

This repository contains a simple Ethereum ERC-20 token contract named Openzeppelin (ZenoToken). The contract is implemented in Solidity and utilizes the OpenZeppelin library for ERC-20 standards, burning functionality, and ownership management.

## Contract Details

The Openzeppelin contract inherits from three different OpenZeppelin contracts:

1. **ERC20**: Implements the ERC-20 token standard with basic token functionality.

2. **ERC20Burnable**: Extends ERC20 and allows the owner to burn (destroy) a specific amount of tokens.

3. **Ownable**: Provides basic authorization control, simplifying the implementation of user permissions.

## Token Details

- **Name**: ZenoToken
- **Symbol**: ZT
- **Initial Supply**: 600 tokens (minted to the deployer's address)

## Functions

### `constructor()`

- Initializes the token with the name "ZenoToken" and symbol "ZT".
- Mints 600 tokens to the address deploying the contract.

### `mint(address to, uint256 amount) public onlyOwner`

- Allows the owner to mint new tokens and assign them to a specified address.

### `burn(uint256 amount) public override onlyOwner`

- Allows the owner to burn (destroy) a specific amount of tokens.

### `transfer(address recipient, uint256 amount) public override returns (bool)`

- Overrides the transfer function from ERC20 to add transfer functionality.

### `transferFrom(address sender, address recipient, uint256 amount) public override returns (bool)`

- Overrides the transferFrom function from ERC20 to add transfer functionality with allowance.

## Usage

Deploy the contract to an Ethereum-compatible blockchain using a tool like [Remix](https://remix.ethereum.org/)


## Author

Donato Zeno, 202011124@fit.edu.ph

## License
This project is licensed under the [Metacrafters] 
