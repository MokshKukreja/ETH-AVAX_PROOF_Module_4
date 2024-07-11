# ETH-AVAX_PROOF_Module_4
Module 4 Project: Degen Token (ERC-20): Pioneering the Future of Gaming

## DEGEN Token Contract

This Solidity smart contract implements an ERC-20 token named DEGEN (DGN). It supports token minting, burning, transferring, and redeeming for game items.

## Overview

- **Token Name:** DEGEN
- **Token Symbol:** DGN
- **Decimals:** 18

## Features

1. **Minting Tokens:**
   - Only the contract owner can mint new tokens.
   - Minted tokens are added to the recipient's balance.

2. **Burning Tokens:**
   - Tokens can be burned from a specified address.
   - Ensures the amount burned does not exceed the address's balance.

3. **Transferring Tokens:**
   - Tokens can be transferred between addresses.
   - Checks that the sender has a sufficient balance and that the recipient address is valid.

4. **Redeeming Tokens for Game Items:**
   - Tokens can be redeemed based on specific game item requirements.
   - Validates the token amount against the requirements for each game item before burning them.

## Usage

To deploy the contract:
- Use a Solidity compiler compatible with version ^0.8.18.

### Functions

- **mintTokens(address recipient, uint256 amount):** Allows the contract owner to mint tokens and assign them to a recipient.
- **burnTokens(address from, uint256 amount):** Burns tokens from a specified address.
- **transferTokens(address to, uint256 amount):** Transfers tokens from the sender's address to a specified address.
- **redeemTokens(address recipient, uint256 amount, uint256 gameItem):** Redeems tokens based on game item requirements, burning them from the recipient's address.

## Deployment

Deploy the contract on a compatible Ethereum network using tools such as Remix, Truffle, or Hardhat.

## Security Considerations

- Ensure only trusted parties have access to the contract owner's private key to prevent unauthorized minting.
- Implement proper access control mechanisms and thoroughly test all contract interactions before deployment.
