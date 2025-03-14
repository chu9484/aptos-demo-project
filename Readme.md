# Student Identity Verification on Blockchain

![image](https://github.com/user-attachments/assets/dcb38d4e-31dc-4514-a4c3-3a3cea497fd3)


## Project Description:
The Student Identity Verification smart contract is designed to revolutionize the way educational institutions manage student identities and track attendance. By utilizing blockchain technology, the contract ensures that student identities are securely stored on-chain, providing transparency, immutability, and protection against fraud.

## Vision

The **Student Identity Verification** smart contract aims to streamline and secure student attendance and identity verification processes using blockchain technology. By storing each student’s identity on-chain, this solution ensures transparency, security, and immutability. The contract allows for easy storage of student information and verification in a decentralized environment, ensuring data integrity and preventing fraud in the educational sector.

## Features

1. **On-chain Identity Storage**:

   - The contract allows educational institutions to securely store student identities on the blockchain, associating them with unique identifiers.
   - This data is stored immutably, ensuring that once a student's identity is recorded, it cannot be tampered with.

2. **Student Verification**:
   - Institutions can verify the identity of a student by fetching stored data from the blockchain. This makes attendance tracking and identity validation easy and efficient.

## Smart Contract Overview

The contract consists of two primary functions:

1. **store_student**:
   - Inputs: Student ID (u64) and Name (vector of bytes).
   - Stores a student’s identity in a struct that includes the student's unique ID and name, associated with the signer's account.
2. **verify_student**:
   - Inputs: The signer's account.
   - Verifies the student’s identity by checking if the student data exists for the provided account.
  
## Smartcontract Deployment Details:
Deployed address: 0xb09a13f6cc285f82d2ab65f3b4e48bb80832ef1008e08f315a661f8a4a109d22
Screenshot:
![image](https://github.com/user-attachments/assets/2899bc7a-3d00-461a-8db4-9932a5d90722)


## Future Scope

1. **Enhanced Security with Cryptographic Proofs**:

   - The contract can integrate more advanced cryptographic proofs (e.g., zero-knowledge proofs) for even more secure identity verification without revealing sensitive data.

2. **Multi-Institution Support**:

   - Future versions of the contract could allow multiple educational institutions to operate within the same contract, enabling cross-institution identity verification for students.

3. **Integration with Attendance Systems**:

   - This contract could be extended to work alongside attendance tracking systems, automatically marking students present when their identity is verified.

4. **Decentralized ID Management**:

   - The smart contract could evolve into a comprehensive decentralized identity management system for educational institutions, where students hold their own digital credentials and share them securely.

5. **Scalability with NFTs or Tokenized Identities**:
   - The student identities could be tokenized as NFTs, offering a more scalable approach to managing student data, including the possibility of extending this system to other entities like employees or alumni.

## Installation and Usage

### Prerequisites

- Move language development environment.
- Access to the blockchain where the contract will be deployed.

### Steps

1. **Compile**: Compile the Move module using the Move compiler.
2. **Deploy**: Deploy the contract to your blockchain of choice.
3. **Interact**:
   - Use the `store_student` function to store student data on-chain.
   - Use the `verify_student` function to verify stored data.

### Example Usage

```
// Store a student's identity
store_student(&signer, 12345, b"John Doe");

// Verify a student's identity
verify_student(&signer);
```

By leveraging blockchain technology, this smart contract ensures secure, immutable, and verifiable student identities, improving the efficiency of attendance and identity verification processes for educational institutions.
