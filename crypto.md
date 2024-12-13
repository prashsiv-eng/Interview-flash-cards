# Cryptographic Algorithms and Protocols: An Overview

Cryptography forms the backbone of secure communication and data protection in the digital world. Below is an overview of key cryptographic paradigms, their advantages, disadvantages, and applications.

---

## Symmetric Cryptography

**Description**:  
Symmetric cryptography uses a single key for both encryption and decryption. Both the sender and recipient share this secret key securely.

**Example**:  
Bob encrypts a message using a shared key. Alice decrypts it using the same key.

**Advantages**:
- **Speed**: Faster and computationally efficient.
- **Efficiency**: Suitable for encrypting large amounts of data.

**Disadvantages**:
1. **Key Exchange Problem**: Securely sharing the key over insecure channels is challenging.
2. **Trust Dependency**: Both parties must trust each other to keep the key secure.
3. **No Authentication**: Does not verify the sender's identity, lacking non-repudiation and integrity.

**Algorithms**:
- **DES**: Operates with a 64-bit block size.
- **3DES**: Enhances DES security by applying encryption three times.
- **AES**: Supports key sizes of 128, 192, and 256 bits.

**Modes of Operation**:
1. **ECB (Electronic Codebook)**: Simple but prone to pattern leaks.
2. **CBC (Cipher Block Chaining)**: Links blocks for better security.
3. **CTR (Counter Mode)**: Supports parallel processing.
4. **GCM (Galois Counter Mode)**: Combines encryption with integrity.

---

## Asymmetric Cryptography

**Description**:  
Asymmetric cryptography uses a pair of keys: a public key for encryption and a private key for decryption.

**Example**:  
Bob encrypts a message using Alice's public key. Only Alice can decrypt it using her private key.

**Advantages**:
1. **No Key Exchange Risks**: Public keys can be shared openly.
2. **Authentication**: Ensures the sender's authenticity and provides non-repudiation.

**Disadvantages**:
1. **Slower**: Computationally intensive compared to symmetric cryptography.
2. **PKI Requirement**: Needs a Public Key Infrastructure (PKI) for managing keys and certificates.

**Applications**:
- **TLS (Transport Layer Security)**: Ensures secure web communication.
  - **Key Exchange**: ECDHE (Elliptic Curve Diffie-Hellman Ephemeral).
  - **Authentication**: ECDSA or RSA (e.g., RSA-2048 or higher).
  - **Encryption**: AES-256-GCM.
  - **Hashing**: SHA-256 or SHA-384.

**Example Cipher Suite**:  
`TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384`

---

## Message Integrity and Authentication

### Message Authentication Code (MAC)
- **Purpose**: Verifies message integrity using a symmetric key.
- **Algorithms**: MD5, SHA-1, SHA-256.

### Hashed Message Authentication Code (HMAC)
- **Purpose**: Enhances MAC by combining the message with a secret key before hashing.
- **Formula**: `hash(o_key_pad || hash(i_key_pad || message))`

**Advantages**:
- More secure than standard MAC.
- Resistant to tampering due to the use of a key.

**Disadvantages**:
- Cannot authenticate the sender or provide non-repudiation.

---

## Hashing Algorithms

Hashing generates a fixed-size digest from input data for verifying integrity.  
**Common Algorithms**:
- **MD5**: 128-bit digest (deprecated due to vulnerabilities).
- **SHA-1**: 160-bit digest (deprecated for modern use).
- **SHA-2**: Includes SHA-256 (256-bit) and SHA-512 (512-bit) digests.

---

## Digital Signatures

**Description**:  
Digital signatures ensure integrity, authentication, and non-repudiation.  
- The sender generates a message digest using a hash function.
- The digest is encrypted with the sender's private key.

**Verification**:  
The recipient uses the sender's public key to decrypt the digest and compares it with a new hash of the message.

---

## Public Key Infrastructure (PKI)

PKI manages digital certificates and public-private key pairs. Certification Authorities (CAs) validate public keys and issue certificates to establish trust.


