# rust-blockchain-challenge

Challenge: Simple Payment System on a Custom Blockchain
Overview:
You are tasked with creating a simplified blockchain-based payment system in Rust. Your implementation should allow users to create wallets, execute transactions, and track the balances within the wallets on the blockchain.

Requirements:
Blockchain Structure:

Implement a basic blockchain structure.
Each block should contain a list of transactions, a timestamp, a hash of the previous block, and its own hash.
Implement the hash calculation using a cryptographic hash function, such as SHA-256.
Wallets:

Implement a wallet system that generates a public/private key pair.
Use the Rust secp256k1 library (or any other cryptographic library) to create keys that are suitable for digital signatures.
Transactions:

Implement a transaction model where one user can send a "coin" to another user's wallet.
Transactions should be signed using the sender's private key and verified by their public key.
Ensure transactions cannot be tampered with once added to a block.
Block Mining:

Implement a simple Proof-of-Work (PoW) algorithm for mining new blocks.
Use a difficulty target (like leading zeroes in the hash) to simulate the mining effort.
Blockchain Validation:

Validate the blockchain integrity by ensuring the blocks are properly linked together and the block hashes follow the difficulty rules.
Check for double spending and reject invalid transactions.
Networking (Optional):

Implement a very basic peer-to-peer network to propagate blocks and transactions.
Use TCP or UDP for communication between nodes (you can use libraries like tokio for asynchronous IO).
Testing:

Write tests for each component including block creation, transaction signing, blockchain validation, and wallet functionality.
Deliverables:
Rust source code with comments explaining your implementation.
Unit tests for all components.
A README file documenting how to run your blockchain and a guide on how to perform transactions.
Stretch Goals (Optional):
Implement a basic consensus mechanism to agree on the current state of the blockchain.
Add a basic transaction fee mechanism.
Create a command-line interface (CLI) to interact with your blockchain.
Optimize the Proof-of-Work algorithm to adjust difficulty based on the mining rate.
Evaluation Criteria:
Correctness: The blockchain must work as specified without errors.
Code Quality: Code should be well-organized and follow Rust's best practices.
Security: The implementation should not have any obvious security flaws.
Performance: The blockchain operations should perform reasonably well.
Testing: There should be thorough testing to ensure all parts are working as expected.
Resources:
The Rust Programming Language Book
Rust Crypto Libraries
Rust secp256k1 Library
Rust tokio for Asynchronous IO
Before starting this challenge, ensure you have a good understanding of blockchain concepts and are comfortable with Rust's syntax and features. Good luck!
