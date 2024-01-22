# Work Guide: Classical Cryptography

## Part 1: Research Topics

In this section, you will research various classical cryptography topics. Each topic has a set of questions to guide your learning.

### 1. The Substitution Cipher

1. What is the substitution cipher and how does it differ from the shift cipher?
2. How can you create a substitution cipher using a keyword or a random permutation?
3. What are the advantages and disadvantages of the substitution cipher?
4. How can frequency analysis be used to break a substitution cipher?
5. Can you provide an example of a historical use of the substitution cipher?

### 2. The Affine Cipher

1. What is the affine cipher and how does it combine the shift and substitution ciphers?
2. How can you encrypt and decrypt messages using the affine cipher?
3. What are the advantages and vulnerabilities of the affine cipher?
4. How can you break the affine cipher using known plaintext attacks?
5. Can you provide an example of a practical use of the affine cipher?

### 3. The Hill Cipher

1. What is the Hill cipher and how does it differ from previous ciphers?
2. How can you encrypt and decrypt messages using the Hill cipher?
3. What are the advantages and limitations of the Hill cipher?
4. How does the Hill cipher utilize matrix operations?
5. Can you provide an example of a real-world application of the Hill cipher?

### 4. The Permutation Cipher

1. What is the permutation cipher and how does it work?
2. How can you encrypt and decrypt messages using the permutation cipher?
3. What are the strengths and weaknesses of the permutation cipher?
4. How can you break the permutation cipher using brute force or frequency analysis?
5. Can you provide an example of a historical use of the permutation cipher?


## Part 2: Cryptanalysis Research

In this section, you will research various cryptanalysis techniques for classical ciphers. Each topic has a set of questions to guide your learning.

### 1. Introduction to Cryptanalysis

1. What is cryptanalysis and why is it important in cybersecurity?
2. What are the different types of cryptanalysis techniques?
3. How does cryptanalysis differ from cryptography?
4. Can you provide an example of a famous cryptanalysis success story?
5. What are the ethical considerations in cryptanalysis?

### 2. The Affine Cipher

1. How can you break the affine cipher using known plaintext attacks?
2. What is the vulnerability of the affine cipher to modular inverses?
3. How can you improve the security of the affine cipher?
4. Can you provide an example of a real-world attack on the affine cipher?
5. What are the limitations of cryptanalysis on the affine cipher?

### 3. The Substitution Cipher

1. How can you break the substitution cipher using frequency analysis?
2. What is the vulnerability of the substitution cipher to known plaintext attacks?
3. How can you improve the security of the substitution cipher?
4. Can you provide an example of a real-world attack on the substitution cipher?
5. What are the limitations of cryptanalysis on the substitution cipher?

### 4. The Hill Cipher

1. How can you break the Hill cipher using matrix algebra?
2. What is the vulnerability of the Hill cipher to key length?
3. How can you improve the security of the Hill cipher?
4. Can you provide an example of a real-world attack on the Hill cipher?
5. What are the limitations of cryptanalysis on the Hill cipher?

### 5. The Permutation Cipher

1. How can you break the permutation cipher using brute force or frequency analysis?
2. What is the vulnerability of the permutation cipher to known plaintext attacks?
3. How can you improve the security of the permutation cipher?
4. Can you provide an example of a real-world attack on the permutation cipher?
5. What are the limitations of cryptanalysis on the permutation cipher?



# Lab Guide: Cryptography Programming Exercises

## Classic Cryptography Topics

### 1. Substitution Cipher

#### Exercise:
Write a Python function `substitution_cipher_encrypt(plaintext, key)` that takes a plaintext string and a substitution key as input and returns the corresponding ciphertext using the substitution cipher.

#### Example:
> - Plaintext: "HELLO"
> - Key: {'H': 'X', 'E': 'Y', 'L': 'Z', 'O': 'A'}
> - Ciphertext: "XYZZA"

> - Plaintext: "WORLD"
> - Key: {'W': 'Q', 'O': 'P', 'R': 'S', 'L': 'T', 'D': 'U'}
> - Ciphertext: "QPSUT"

### 2. Affine Cipher

#### Exercise:
Write a Python function `affine_cipher_encrypt(plaintext, a, b)` that takes a plaintext string and two integer values a and b as input and returns the corresponding ciphertext using the affine cipher.

#### Example:
> - Plaintext: "HELLO"
> - a: 5
> - b: 8
> - Ciphertext: "RCLLA"

> - Plaintext: "WORLD"
> - a: 3
> - b: 7
> - Ciphertext: "VXGOQ"

### 3. Hill Cipher

#### Exercise:
Write a Python function `hill_cipher_encrypt(plaintext, key)` that takes a plaintext string and a 2x2 matrix key as input and returns the corresponding ciphertext using the Hill cipher.

#### Example:
> - Plaintext: "HELLOWORLD"
> - Key: [[2, 3], [1, 4]]
> - Ciphertext: "AXDDQYBEFX"

### 4. Permutation Cipher

#### Exercise:
Write a Python function `permutation_cipher_encrypt(plaintext, key)` that takes a plaintext string and a permutation key as input and returns the corresponding ciphertext using the permutation cipher.

#### Example:
> - Plaintext: "HELLO"
> - Key: [3, 1, 4, 2, 5]
> - Ciphertext: "LHLEO"

> - Plaintext: "WORLD"
> - Key: [2, 4, 1, 5, 3]
> - Ciphertext: "OLWDR"

## Cryptanalysis Topics

### 1. Affine Cipher

Write a Python function `break_affine_cipher(ciphertext)` that takes a string `ciphertext` as input and attempts to break the affine cipher by trying all possible combinations of `a` and `b` values. The function should return the most likely plaintext obtained by decrypting the ciphertext using the correct `a` and `b` values.

Example:
```python
ciphertext = "Czggj, Tqxxa!"
plaintext = break_affine_cipher(ciphertext)
print(plaintext)
```
Output:
```
Hello, World!
```

### 2. Substitution Cipher

Write a Python function `break_substitution_cipher(ciphertext)` that takes a string `ciphertext` as input and attempts to break the substitution cipher by performing frequency analysis on the letters in the ciphertext. The function should return the most likely plaintext obtained by decrypting the ciphertext using the correct key.

Example:
```python
ciphertext = "XYZZA, CDCFA!"
plaintext = break_substitution_cipher(ciphertext)
print(plaintext)
```
Output:
```
Hello, World!
```

### 3. Hill Cipher

Write a Python function `break_hill_cipher(ciphertext, n)` that takes a string `ciphertext` and an integer `n` as input and attempts to break the Hill cipher by performing frequency analysis on the letters in the ciphertext and using matrix algebra. The function should return the most likely plaintext obtained by decrypting the ciphertext using the correct key.

Example:
```python
ciphertext = "XZGZJ, ZJGFA!"
n = 2
plaintext = break_hill_cipher(ciphertext, n)
print(plaintext)
```
Output:
```
Hello, World!
```

