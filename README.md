# Hash Cracker

This is a Python-based brute-force hash cracker. It attempts to find the original password from a given hash using various character sets and hashing algorithms.

## Features

- Supports multiple hashing algorithms including MD5, SHA1, SHA256, and more.
- Allows customization of character sets for password cracking.
- Multi-threaded and multi-processing for faster execution.
- Reports progress at regular intervals.

## Character Sets

- Lowercase alphabets
- Uppercase alphabets
- Mixed case alphabets
- Numeric
- Punctuation
- Combinations of the above

## Hashing Algorithms

- MD5
- MD4
- LM
- NTLM
- SHA1
- SHA224
- SHA256
- SHA384
- SHA512

## Usage

1. **Clone the repository**:
    ```sh
   git@github.com:AkashElangovan/password-hash-cracker.git
    ```

2. **Run the script**:
    ```sh
    ./hashcracker.py
    ```

3. **Follow the prompts**:
    - Select the character set.
    - Specify the maximum possible length of the password.
    - Select the hash type.
    - Enter the hash to be attacked.

4. **View results**:
    - The script will attempt to crack the hash and display the found password or a message if no match is found.
    - Progress updates will be shown at regular intervals.

## Example

```sh
Specify the character set to use:
01. abcdefghijklmnopqrstuvwxyz
02. ABCDEFGHIJKLMNOPQRSTUVWXYZ
03. abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
04. 0123456789
...
15. abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~

Enter the character set number: 07

Specify the maximum possible length of the password: 5

Specify the hash's type:
01. MD5
02. MD4
03. LM
04. NTLM
...
09. SHA512

Enter the hash type number: 01

Specify the hash to be attacked: 5d41402abc4b2a76b9719d911017c592

Trying to crack hash 5d41402abc4b2a76b9719d911017c592
Character set: abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789, iteration: 100, trying: abcde, hashes/sec: 33
Character set: abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789, iteration: 200, trying: bcdef, hashes/sec: 50
...
Match found! Password is hello
