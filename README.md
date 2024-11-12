# Mini-AES-CBC
AES128/192/256-CBC specialized for embedded systems (for both OS based devices and embedded systems)

Features : 
* Specialized for embedded systems.
* Only two routines, each one for encryption and decryption.
* No CPRNG/PRNG included thus it is user's responsibility to pass different IV for encrypting each time.


User routines :

Encryption : void AES_Encrypt(uint8_t AES_Type, uint8_t* PlainByteStream, uint32_t Size_PlainByteStream, const uint8_t* key, uint32_t* Size_EncryptedByteStream, uint8_t* IV);
Decryption : void AES_Decrypt(uint8_t AES_Type, uint8_t* EncryptedByteStream, uint32_t Size_EncryptedByteStream, const uint8_t* key, uint32_t* Size_DecryptedByteStream);
