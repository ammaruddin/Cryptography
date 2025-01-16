# Cryptography Lab - Secure Encryption Techniques

⚠️ Disclaimer: This project is strictly for educational and ethical hacking purposes and done under controlled environment. Unauthorized use of these techniques is illegal.


## Overview
This lab, conducted by **Mohammed Ammaruddin**, explores various cryptographic techniques, including symmetric and asymmetric encryption, initialization vectors, and RSA key analysis. The lab demonstrates the importance of cryptographic principles in ensuring secure data transmission and highlights key concepts like initialization vectors, RSA key strength, and verification mechanisms.

---

## Objectives
1. Understand how initialization vectors (IVs) influence ciphertext variations in encryption.
2. Analyze the security of RSA public keys based on key length.
3. Explore verification processes and their significance in cryptographic applications.

---

## Key Findings

### Q5: Initialization Vectors and Ciphertext Variations
- OpenSSL generates a unique **initialization vector (IV)** for each encryption operation.
- Even with the same password, distinct IVs result in different ciphertexts.
- The `-p` option in OpenSSL's decryption command reveals the salt, key, and IV used during encryption.
- **Observation**: `ciphertext.txt` and `ciphertext2.txt` were encrypted with different IVs, producing distinct ciphertexts despite the same password.

---

### Q6: RSA Public Key Analysis
- **Key Length**: The RSA public key used in this lab has a length of **3072 bits**.
- **Strength**:
  - Longer keys, like the 3072-bit RSA key, offer a very high level of security.
  - They are resistant to brute-force attacks and key factorization attempts.
- **Applications**: This key size is recommended for most secure encryption applications requiring strong cryptographic guarantees.

---

### Q9: Verification Process
- **Result**: Verification failed.
- This highlights the importance of ensuring accurate cryptographic setup and key management in secure communication.

---

## Tools and Technologies
- **OpenSSL**: Used for encryption, decryption, and key analysis.
- **RSA Algorithm**: Evaluated for its cryptographic strength and application suitability.

---

## Insights
- **Initialization Vectors**: Critical in ensuring that ciphertexts remain unique and resistant to replay attacks, even with repeated use of the same password.
- **RSA Key Strength**: A 3072-bit key provides robust security, making it suitable for applications demanding high encryption standards.
- **Verification**: Proper configuration and validation are essential for cryptographic integrity.

---

## Recommendations
1. **Use Strong Keys**: RSA keys of at least 3072 bits are recommended for applications requiring long-term security.
2. **Employ Unique IVs**: Ensure that encryption tools generate unique IVs to strengthen ciphertext security.
3. **Verify Processes**: Always validate cryptographic processes to detect potential misconfigurations or vulnerabilities.

---

## Disclaimer
This lab was conducted in a controlled environment for **educational purposes only**. Unauthorized use of cryptographic techniques is strictly prohibited and may violate legal and ethical standards.
