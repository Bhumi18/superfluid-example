# Superfluid Funding Example

This project demonstrates a simple funding contract using Superfluid Protocol on the Polygon network. It allows users to start and stop funding streams to different projects using Super Tokens (fDAIx).

## Overview

The `Funding` contract provides the following main functionalities:

1. Minting and wrapping fDAI to fDAIx
2. Starting a funding stream to a receiver
3. Stopping a funding stream
4. Staking MATIC to receive fDAIx
5. Checking fDAIx balance

## Prerequisites

- Solidity ^0.8.13
- Superfluid Protocol
- Polygon network (testnet)

## Contract Details

- The contract is deployed on the Polygon testnet
- It uses fDAIx as the Super Token for streaming
- Utilizes Superfluid's Constant Flow Agreement (CFA) for creating token streams

## Key Functions

- `gainDaiX()`: Mints fDAI and wraps it into fDAIx
- `startFunding(address receiver, int96 flowRate)`: Starts a funding stream to a receiver
- `stopFunding(address receiver)`: Stops a funding stream to a receiver
- `getDAIx(uint256 amount)`: Allows users to stake MATIC and receive fDAIx
- `getBalance()`: Checks the fDAIx balance of the caller

## Setup and Deployment

1. Clone the repository
2. Install dependencies
3. Deploy the contract on Polygon testnet, providing the Superfluid host and fDAIx token addresses

## License

This project is licensed under the MIT License.
