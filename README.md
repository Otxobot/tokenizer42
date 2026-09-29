# Tokenizer42 - Technology Choices

This document explains the technology choices made for this project and the reasoning behind each one. 

## Blockchain: BNB Smart Chain (BEP-20)

Chosen because this subject is produced in partnership with BNB Chain, and the provided testnet targets it directly.

BEP-20 is interface-compatible with ERC-20, which is the equivalent to the Ethereum technical standard to create and manage fungible tokens on the Ethereum blockchain. So the token logic itself doesn't change based on this choice. 

## Language: Solidity
 
Solidity is the standard language for EVM-compatible chains like BSC, and the only language OpenZeppelin's contract library is written in. 

Choosing it keeps the project aligned with the blockchain's own standards, as required by the subject. It also has the most amount of documentation available for learning. 

## Framework: Hardhat

Hardhat provides a built-in local test network, an integrated testing framework and support from OpenZeppelin's own plugins. 

This basically covers all the necessities I had for developing this token. Covering compilation, testing and deployment in a single toolchain.


## Scripting language: TypeScript

Type-checks scripts and tests against the contract's actual ABI, catching mistakes (wrong argument types, misspelled function names) before runtime rather than during a live deployment. It's also Hardhat's own default scaffold as of Hardhat 3.

