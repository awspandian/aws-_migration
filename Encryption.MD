Asymmetric Encryption
• Asymmetric encryption is also known as public key cryptography
• Messages encrypted with the public key can only be decrypted with the private key
• Messages encrypted with the private key can be decrypted with the public key
• Examples include SSL/TLS and SSH


Customer Master Keys (CMKs)
• Customer master keys are the primary resources in AWS KMS
• The CMK also contains the key material used to encrypt and decrypt data
• CMKs are created in AWS KMS
• Symmetric CMKs and the private keys of asymmetric CMKs never leave AWS KMS unencrypted
• By default, AWS KMS creates the key material for a CMK
• Can also import your own key material
• A CMK can encrypt data up to 4KB in size
• A CMK can generate, encrypt and decrypt Data Encryption Keys
• Data Encryption Keys can be used for encrypting large amounts of data

AWS Managed CMKs
• Created, managed, and used on your behalf by an AWS service that is integrated with AWS KMS
• You cannot manage these CMKs, rotate them, or change their key policies
• You also cannot use AWS managed CMKs in cryptographic operations directly; the service that creates them uses them on your behalf

Data Encryption Keys
• Data keys are encryption keys that you can use to encrypt data, including large amounts of data and other data encryption keys
• You can use AWS KMS customer master keys (CMKs) to generate, encrypt, and decrypt data keys
• AWS KMS does not store, manage, or track your data keys, or perform cryptographic operations with data keys
• You must use and manage data keys outside of AWS KMS

AWS CloudHSM
• AWS CloudHSM is a cloud-based hardware security module (HSM)
• Generate and use your own encryption keys on the AWS Cloud
• CloudHSM runs in your Amazon VPC
• Uses FIPS 140-2 level 3 validated HSMs
• Managed service and automatically scales
• Retain control of your encryption keys - you control access (and AWS has no visibility of your encryption keys)

AWS CloudHSM Use Cases
• Offload SSL/TLS processing from web servers
• Protect private keys for an issuing certificate authority (CA)
• Store the master key for Oracle DB Transparent Data Encryption
• Custom key store for AWS KMS – retain control of the HSM that protects the master keys
