<link rel="stylesheet" href="/assets/css/custom.css">

# Symmetric vs Asymmetric Encryption
Encryption is a core part of cryptography, and understanding the difference between symmetric and asymmetric methods is crucial.  

**Symmetric encryption** uses the same key to encrypt and decrypt data. This makes it fast and efficient, but securely sharing the key between parties can be difficult. Examples include AES and DES.  

**Asymmetric encryption** uses a pair of keys: a public key to encrypt and a private key to decrypt. This solves the key-sharing problem, but it is slower than symmetric encryption. Examples include RSA and ECC.  

In practice, most secure systems combine both: asymmetric encryption securely shares a symmetric key, which then encrypts the bulk of the data. This is how many messaging apps and HTTPS connections work.  

[Learn More](https://www.cloudflare.com/learning/ssl/what-is-encryption/)
