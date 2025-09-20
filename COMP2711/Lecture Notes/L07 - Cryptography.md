## Ciphers

### Caesar Cipher

```bash
A  B  C  D  E  F  G  H  I  J K  L  M  N  O  P  Q  R  S  T  U  V  W  X  Y  Z
0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25
```

Encrypts a message by **shifting each letter a fixed number of positions down the alphabet**, wrapping around to the beginning if necessary.

$\text{Encryption: }f(p) = (p + k) \pmod{26}$  
$\text{Decryption: }f^{-1}(p) = (p - k) \pmod{26}$

* $p$ represents the numerical equivalent of a letter ($A = 0$, $B = 1$, …, $Z = 25$).
* $k$ is the shift key, any integer from 0 to 25.

> [!Example]-  
> Let's encrypt the message "BRUH" using a key of $k = 5$.
>
> * **B (1):** $(1 + 5) \pmod{26} = 6$ (G)
> * **R (17):** $(17 + 5) \pmod{26} = 22$ (W)
> * **U (20):** $(20 + 5) \pmod{26} = 25$ (Z)
> * **H (7):** $(7 + 5) \pmod{26} = 12$ (M)
> 
> Therefore, "BRUH" encrypted with a key of 5 becomes "GWZM".

### Affine Ciphers

Encrypts letters by applying **a linear modular function (ax + b) to their numerical equivalents**, where 'a' and 'b' form the key, 'a' must be ==co-prime to the modulus (m)==, 'b' can be any integer from 0 to $m-1$.

$\text{Encyption: }f(p) = (ap + b) \pmod{26}$  
$\text{Decryption: }f^{-1}(c) = a^{-1}(c - b) \pmod{26}$

> [!Note]- Why 'a' must be co-prime to the modulus (m)  
> If 'a' and 'm' (26 in this case) are not co-prime, then 'a' does not have a multiplicative inverse modulo 'm'. The decryption function requires the multiplicative inverse ($a^{-1}$) of 'a' modulo 'm'. If 'a' and 'm' share a common factor greater than 1, this inverse does not exist. Without $a^{-1}$, the decryption process is impossible, and the original plaintext cannot be recovered.  

> $(2 \times x)\pmod{26} = 1 \implies 2x = 26k + 1 \text{ (No solution)}$

> [!Example]- Encryption  
> **Example: Encrypting "BRUH"**
>
> * **Key:** $a = 5$, $b = 8$
> * **Plaintext:** BRUH
> * **Numerical Equivalents (A=0, B=1, …, Z=25):**
> 	* B = 1
> 	* R = 17
> 	* U = 20
> 	* H = 7
> * **Encryption:**
> 	* B: $(5 * 1 + 8) \pmod{26} = 13 \pmod{26} = 13$ (N)
> 	* R: $(5 * 17 + 8) \pmod{26} = 93 \pmod{26} = 15$ (P)
> 	* U: $(5 * 20 + 8) \pmod{26} = 108 \pmod{26} = 4$ (E)
> 	* H: $(5 * 7 + 8) \pmod{26} = 43 \pmod{26} = 17$ (R)
> * **Cipher text:** NPER

> [!Example]- Decryption  
> **Example: Decrypting "NPER" (using the same key as the encryption example)**  
> We need to find a number $a^{-1}$ such that $(a \cdot a^{-1}) \pmod{26} = 1$. In our case, $a = 5$. The modular multiplicative inverse of $5 \pmod{26}$ is $21$ because $(5 \cdot 21) \pmod{26} = 105 \pmod{26} = 1$.
>
> * **Key:** $a = 5$, $b = 8$
> * **Ciphertext:** NPER
> * **Numerical Equivalents (A=0, B=1, …, Z=25):**
> 	* N = 13
> 	* P = 15
> 	* E = 4
> 	* R = 17
> * **Modular Inverse of _a_:** $5^{-1} \pmod{26} = 21$ (because $5 \cdot 21 = 105 = 4 \cdot 26 + 1$, so $105 \pmod{26} = 1$)
> * **Decryption:**
> 	* N: $21(13 - 8) \pmod{26} = 21 \cdot 5 \pmod{26} = 105 \pmod{26} = 1$ (B)
> 	* P: $21(15 - 8) \pmod{26} = 21 \cdot 7 \pmod{26} = 147 \pmod{26} = 17$ (R)
> 	* E: $21(4 - 8) \pmod{26} = 21 \cdot (-4) \pmod{26} = -84 \pmod{26} = 20$ (U)
> 	* R: $21(17 - 8) \pmod{26} = 21 \cdot 9 \pmod{26} = 189 \pmod{26} = 7$ (H)
> * **Plaintext:** BRUH

### Block Ciphers

* 1 byte = 8 bits
* Partition the message into blocks of $k$ characters
	* Treat each block as a big number of $8k$ bits.
	* Use arithmetic modulo $2^{8k}$

Choose $k = 10$:

$\text{Encyption: }f(p) = (ax + b) \pmod{2^{80}}$  
$\text{Decryption: }f^{-1}(y) = a^{-1}(y - b) \pmod{2^{80}}$

#### Advanced Encryption Standard (AES)

* Block size 128 bits
* Key lengths: 128, 192, 256 bits

## Key Exchange

### Modular Exponentiation

#### Example of Modular Exponentiation

$13^4 \equiv 6^4 \pmod{7}$  
$3^{2+4} \equiv 3^2 \cdot 3^4 \equiv 2 \cdot 4 \equiv 1 \pmod{7}$  
$3^{4(2)} \equiv (3^4)^2 \equiv 4^2 \equiv 2 \pmod{7}$

##### Modular Exponentiation of Very Large Number

$5^{117} \mod 19$  
$117 = 1110101 \text{ (Binary)}$  
$117 = 2^6 + 2^5 + 2^4 + 2^2 + 2^0 = 64 + 32 + 16 + 4 + 1$  
$5^{117} \mod 19 = (5^{64} + 5^{32}+ 5^{16}+ 5^{4}+ 5^{1}) \mod 19$

$5^1 \mod 19 = 5$  
$5^2 \mod 19 = 6$

$5^4 \mod 19 = (5^2 \cdot 5^2) \mod 19 = (5^2 \mod 19 \cdot 5^2 \mod 19) \mod 19$  
$(5^2 \mod 19 \cdot 5^2 \mod 19) \mod 19 = (6 \cdot 6) \mod 19 = 17$

$5^8 \mod 19 = 4$  
$5^{16} \mod 19 = 16$  
$5^{32} \mod 19 = 9$  
$5^{64} \mod 19 = 5$

$5^{117} \mod 19 = (5^1 \cdot 5^4 \cdot 5^{16} \cdot 5^{32} \cdot 5^{64}) \mod 19$  
$5^{117} \mod 19 = (5^1 \mod 19 \cdot 5^4 \mod 19 \cdot 5^{16} \mod 19 \cdot 5^{32} \mod 19 \cdot 5^{64} \mod 19) \mod 19$  
$5^{117} \mod 19 = (5 \cdot 17 \cdot 16 \cdot 9 \cdot 5) \mod 19$  
$5^{117} \mod 19 = 61200 \mod 19 = 1$  
$5^{117} \mod 19 = 1$

### A Hard Problem: Discrete Logarithm

### Diffe-Hellman Key Exchange

## Public Key Cryptography and RSA

### RSA (Rivest–Shamir–Adleman)

> Exam

Wikipedia: https://en.wikipedia.org/wiki/RSA_(cryptosystem)

1. Choose two very large prime number $p$ and $q$
2. Set $n=pq$ and $T = (p - 1)(q - 1)$
3. $e \neq 1$ so that $\gcd (e, T) = 1$
4. Calculate $d=e^{-1} \mod{T}$ (Extended Euclid's algorithm)
5. $(e, n)$ as public key
6. $d$ as private key.

$$\text{Encryption: }x^e \mod {n} = C$$  
$$\text{Decryption: }C^d \mod n = x$$

### Proof Plan

We want to show $C^{d} = x^{de} \equiv x \pmod n$

$$C^{d} = x^{de} \equiv x \pmod p$$  
$$C^{d} = x^{de} \equiv x \pmod q$$

$$C^{d} = x^{de} \equiv x \pmod {pq}$$

#### Fermat Little Theorem

> https://brilliant.org/wiki/fermats-little-theorem/

Let $p$ be a prime number, and $a$ be any integer. Then $a^p - a$ is always divisible by $p$.

In [modular arithmetic](https://brilliant.org/wiki/modular-arithmetic/ "modular arithmetic") notation, this can be written as $a^p \equiv a \mod p$.

$$a^{p-1} \equiv 1 \pmod p$$

> [!Example]- Proof
> 1. Consider the set $\{1, 2, …, p-1\}$. Multiply each element by $a$: $\{a, 2a, …, (p-1)a\}$.
> 2. $a \cdot 2a \cdot … \cdot (p-1)a \equiv 1 \cdot 2 \cdot … \cdot (p-1) \pmod{p}$
> 3. $a^{p-1}(p-1)! \equiv (p-1)! \pmod{p}$
> 4. $a^{p-1} \equiv 1 \pmod{p}$ (Since $(p-1)!$ is not divisible by $p$)

##### Example

$$7^{222} \mod 11$$

$$7^{220 + 2} \equiv {7 ^ {20}}^{10} \cdot 7^2 \equiv 1^{22} \cdot 49 \equiv 5\mod 11$$
