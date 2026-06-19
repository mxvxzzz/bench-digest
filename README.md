# STM32MPU Provider

In OpenSSL terms, a provider is a unit of code that offers implementations for cryptographic operations such as digests, ciphers, signatures, and more.

STM32 Provider offloads cryptographic operations for security peripherals embedded in ST MPUs, through the Linux AF_ALG and Cryptodev.

Here is a overviweuw of the CryptoAPI architecture, from User space to hardware :

# CryptoAPI Architecture with STM32MPU Provider  

![Architecture Crypto](images/stprovider.svg)

# Current algorithm implemented

## Digest :

- SHA-1
- SHA-224
- SHA-256
- SHA-384
- SHA-512
- SHA3-256
- SHA3-384
- SHA3-512

## HMAC

- HMAC-SHA-1
- HMAC-SHA-224
- HMAC-SHA-256
- HMAC-SHA-384
- HMAC-SHA-512
- HMAC-SHA3-256
- HMAC-SHA3-384
- HMAC-SHA3-512

---

# Benchmark Results on STM32MP25 :

You can view the latest performance reports for SHA-1, SHA-256, and SHA-512 here:

👉 https://mxvxzzz.github.io/bench-digest/
