# SampleToken Smart Contract

## Overview
The `SampleToken` smart contract is an ERC20-based token that implements a simple minting and burning mechanism. The contract allows the **owner** to mint new tokens to any address and allows **any user** to burn tokens from their own balance.

## Features
- **Minting**: Only the owner of the contract can mint new tokens.
- **Burning**: Any user can burn tokens from their own balance.
- **Transfer**: Users can transfer tokens as per the standard ERC20 functionality.

## Contract Details

- **Token Name**: `SampleToken`
- **Token Symbol**: `SPT`
- **Owner**: The contract owner is set during deployment.

## Functions

### `mint(address to, uint256 amount)`
- **Description**: Allows the contract owner to mint new tokens and send them to a specified address.
- **Access Control**: Only the owner can call this function.
- **Parameters**:
  - `to` (address): The address to receive the minted tokens.
  - `amount` (uint256): The number of tokens to mint.

### `burn(uint256 amount)`
- **Description**: Allows any user to burn tokens from their own balance.
- **Access Control**: Available to all users.
- **Parameters**:
  - `amount` (uint256): The number of tokens to burn.
