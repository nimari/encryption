### Encryption التشفير

- **Symmetric - التشفير المتماثل**
    - One Key - يستخدم مفتاح واحد للتشفير و نفس المفتاح لفك التشفير
    - Categories
        - Block Cipher: حيث يقسم المُدخل إلى أجزاء متساوية ثم تُشفر كل على حدة
        - Stream Cipher: حيث يتم التشفير على مستوى ال “بيت”
    - Algorithms - خوارزميات التشفير المتماثل
        - DES
        - AES
        - IDEA
        - BlowFish
        - RC
    - Data cab be encrypted when:
        - At rest
        - In Transit, In Motion or In Flight
    - Modes
        - ECB ( **E**lectronic **C**ode **B**ook )
        - CBC ( **C**ipher **B**lock **C**hain )
        - CFB ( **C**ipher **F**eed **B**ack )
        - OFB ( **O**utput **F**eed **B**ack )
- **Asymmetric - التشفير الغير متماثل يستخدم مفتاحين : أحدها للتشفير و الآخر لفك التشفير**
    - Algorithms - خوارزميات التشفير الغير متماثل
        - RSA
        - DSS
        - DSA
        - ECC
        - DHG ( **D**iffie **H**ellman **G**roup )
- **Hashing**: One Way Function
    - MD5
    - SHA1 - SHA2 - SHA3 - SHA256
- Encryption & Hashing Tools
    - [Openssl - Cryptography Toolkit](https://www.openssl.org/)
    - [JCrypTool — The cryptography e-learning platform](https://www.cryptool.org/en/jct/)

* * *

## Homomorphic Encryption - التشفير المتماثل الشكل

- What is Homomorphic Encryption ( HE ) ?
    
    - HE is a form of encryption that allows computation on encrypted data يمكنك إجراء عمليات رياضية على النص المُشفَّر
        
    - Example: Encrypt 2, 3, and 7, ask 3rd party to add the first two and multiply by the third: the result will be 35 but homomorphically encrypted
        
    - You can use non-encrypted values in the computations: FHE\_decrypt(FHE\_encrypt(2) * 5) equals 10
        
- FHE Pros:
    
    - Privacy Preserving.
    - The client never need to **trust** the model owner
- HE Cons:
    
    - Computationally expensive
    - Impact Mergers & Acquisitions
        - Due Diligence done without violating privacy
- FHE Use Cases
    
    - Outsourcing Computation
    - Applying AI, ML, Data Science to Encrypted Data without Decrypting it
    - In ML ( MLaaS ), The model owner never **sees** the clients’ private data
- FHE = **F**ully **H**omorphic **E**ncryption
    
    - Support Both **Addition** and **Multiplication**
    - IBM FHE Services

### Tools

- [Microsoft SEAL Library ( Open Source) : Started since 2015](https://github.com/microsoft/SEAL)

### Resources

- [OpenMined: What is Homomorphic Encryption?](https://www.youtube.com/watch?v=2TVqFGu1vhw)
- [Deep Dive into Homomorphic Encryption](https://www.youtube.com/watch?v=JM0bJoCRp0I)
- [Homomorphic Encryption Overview](https://www.youtube.com/watch?v=3zoT89DiLA0)
- [Bruce Schenier - Homomorphic Encryption Breakthrough](https://www.schneier.com/blog/archives/2009/07/homomorphic_enc.html)
- [IBM completes successful field trials on Fully Homomorphic Encryption](https://arstechnica.com/gadgets/2020/07/ibm-completes-successful-field-trials-on-fully-homomorphic-encryption/)
- [Homomorphic Encryption Standardization](https://homomorphicencryption.org/)
- [Google - Fully Homomorphic Encryption (FHE)](https://github.com/google/fully-homomorphic-encryption)
- [Github - Awesome Homomorphic Encryption](https://github.com/jonaschn/awesome-he)
