# ZKP

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Zero-Knowledge Proofs allow a prover to demonstrate knowledge of something to a verifier without revealing the actual information. In this context, the prover can generate an off-chain proof that convinces the verifier of the solution's validity without disclosing any sensitive data.

```

    Prover         Smart Contract (Verifier)
  ___________        ________________
 |           |      |                |
 |           |      |                |
 |           |      |                |
 |    Prove  |      |    Verify      |
 |    Proof  |<---->|    Solution    |
 |           |      |                |
 |___________|      |________________|

```


This repository contains an implementation of a Solidity smart contract that acts as a verifier for zero-knowledge proofs (zk-SNARK) without revealing any information about the solution. The prover can generate an off-chain proof and submit it to the verifier smart contract to prove the solution without disclosing any sensitive data.

## Overview

Zero-Knowledge (ZK) cryptography allows the creation of a Solidity smart contract that can act as a verifier without knowing the solution to the problem. The prover, in this case, generates an off-chain proof, which can be posted to the verifier smart contract to demonstrate that a puzzle has been solved without revealing the actual solution.

The implementation in this repository leverages the Circom domain-specific language for defining arithmetic circuits. These circuits are used to generate zero-knowledge proofs. The provided `verify` function in the Solidity smart contract performs the verification process using the zk-SNARK scheme.


## Usage

To use this implementation, follow these steps:

1. Clone the repository: `git clone https://github.com/shivam017arora/zkp-quadratic-hardhat.git`
2. Install the required dependencies: `npm install` or `yarn install` (recommended)
3. Run the tests: `yarn hardhat test`

## License

This project is licensed under the [MIT License](LICENSE).

Please note that this implementation is for educational purposes and may not be suitable for production environments. Use it at your own risk.
