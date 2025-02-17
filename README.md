This repository contains a Solidity smart contract with a bug in the balanceOf function. The bug causes unexpected behavior when the balance of an account is zero.  The solution demonstrates how to correctly handle this edge case.

## Bug

The balanceOf function does not explicitly check for a zero balance, leading to potential issues when interacting with accounts that have no tokens.  This could manifest in the UI or cause unexpected results in other parts of the application.

## Solution

The solution introduces a check for a zero balance, handling the case gracefully and preventing errors.

## How to Reproduce

1. Compile the `balanceOfBug.sol` contract.
2. Deploy the contract to a test network.
3. Call the `balanceOf` function with an address that has a zero balance.
4. Observe the unexpected behavior.

5. Compile the `balanceOfSolution.sol` contract.
6. Deploy the contract to a test network.
7. Call the `balanceOf` function with an address that has a zero balance.
8. Observe the correct behavior.