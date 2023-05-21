<h2> Task2: Encryption using Different Ciphers and Modes </h2>

<p>In this task, we will be exploring different encryption algorithms and modes to encrypt and decrypt files. To do this, we will use the `openssl enc` command, which is a command-line tool for encrypting and decrypting files using various encryption algorithms and modes.

The first step in this task is to choose different cipher types. A cipher is an algorithm used for encryption and decryption of data. There are many different types of ciphers, each with its own strengths and weaknesses. Some examples of popular ciphers include AES, Blowfish, and Triple DES.

To choose a cipher type, we can use the `-aes-256-cbc` option with the `openssl enc` command. This will use the Advanced Encryption Standard (AES) cipher with a 256-bit key and Cipher Block Chaining (CBC) mode for encryption and decryption. We can also choose other cipher types by changing the `-aes-256-cbc` option to a different cipher type, such as `-bf-cbc` for Blowfish in CBC mode or `-des-ede3-cbc` for Triple DES in CBC mode.

Once we have chosen a cipher type, we can then use the `openssl enc` command to encrypt and decrypt files. To encrypt a file, we use the following command:

```
openssl enc -aes-256-cbc -in input_file -out encrypted_file
```

This command will encrypt the `input_file` using the AES-256-CBC cipher and write the encrypted datato the `encrypted_file`. We can then decrypt the file using the following command:

```
openssl enc -aes-256-cbc -d -in encrypted_file -out decrypted_file
```

This command will decrypt the `encrypted_file` using the AES-256-CBC cipher and write the decrypted data to the `decrypted_file`.

In addition to choosing different cipher types, we can also experiment with different modes of operation. Encryption modes determine how the cipher processes the data in blocks, and there are several different modes available, such as ECB, CBC, CFB, and OFB. Each mode has its own advantages and disadvantages, and choosing the right mode can have a significant impact on the security and performance of the encryption.

To experiment with different modes, we can simply change the mode parameter in the `-aes-256-cbc` option to a different mode, such as `-aes-256-ecb` for AES-256 in ECB mode or `-aes-256-ofb` for AES-256 in OFB mode.</p>
