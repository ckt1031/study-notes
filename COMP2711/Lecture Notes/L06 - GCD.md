> October 30, 2024

## Definition

Let $a$, $b$ be integers, not both $0$. The largest integer $d$ such that $d | a$ and also $d|b$ is also the greatest common divisor (GCD) of $a$ and $b$, denoted as $\gcd(a,b)$

## Euclidean Algorithm

Let $a = bq + r$, where $a$, $b$, $q$, and $r$ are integers. Then $\text{gcd}(a, b) = \text{gcd}(b, r)$.  

### Proofing

$\text{gcd}(a, b) = \text{gcd}(b, r)$,

$a = bq + r$

$a = dk_1, b = dk_2$

Then, $r = a - bq = dk_1 - dk_2q = d(k_1 - k_2q)$, so $d|r$

## Extended Euclidean Algorithm

### Bézout's Theorem

Let $a$, $b$ be positive integers, then there exist integer $x$ and $y$ such that $ax + by = \gcd(a, b)$

$$x = y' - qx', y = x'$$

### Example

Find $\gcd(252, 198)$

$252 = 198 \cdot 1 + 54$

$198 = 54 \cdot 3 + 36$  

$54 = 36 \cdot 1 + 18$  

$36 = 18 \cdot 2 + 0$

$\gcd(252, 198) = 18$

#### Using the Extended Euclidean Algorithm

$18 = 54 - 36 \cdot 1$

> $36=198-54 \cdot 3$

> $54 = 252 - 198 \cdot 1$

$18 = 54 - (198 - 54 \cdot 3) = 54 \cdot 4 - 198$

$18 = (252 - 198 \cdot 1) \cdot 4 - 198 = 252 \cdot 4 - 198 \cdot 5$

So, $x = 4, y = -5$

#### Using Bézout's Theorem

$252 \cdot 4 + 198 \cdot (-5) = 18$

$198 \cdot (-1) + 54 \cdot 4 = 18$

$54 \cdot 1 + 36 \cdot (-1) = 18$

$36 \cdot 0 + 18 \cdot (1) = 18$

## Multiplicative Inverses

### Definition

Let $a$ be an integer, $a$ has a multiplicative inverse modulo $m$ if there exists an integer $b$ such that $ab \equiv 1 \pmod{m}$

When $\gcd(a, m) = 1$, $a$ and $m$ are coprime.

$ax + my \equiv 1 \pmod{m}$

$ax \equiv 1 \pmod{m}$

$x = a^{-1}$

### Example

Find the multiplicative inverse of $3$ modulo $7$

Using the extended Euclidean algorithm, we have $7 = 2 \cdot 3 + 1$.  
We get $-2 \cdot 3 + 1 \cdot 7 = 1$.

$-2 mod 7 = 5$ is the inverse of $3$ in $Z_7$

### Theorem

Let $a$ be an integer, then $a$ has a multiplicative inverse modulo $m$ if and only if $\gcd(a, m) = 1$

## Congruence

If $\gcd (a, m) = 1$, the linear congruence $ax \equiv b \pmod{m}$ has a unique solution modulo $m$.

## The Chinese Remainder Theorem

#cheat-sheet

### Theorem

> Make sure $n_{1}, n_{2}, \dots, n_{k}$ are relatively prime

> It is a one-to-one function

#### Proof

$x \equiv a_{1} \pmod{m_{1}}$  
$x \equiv a_{2} \pmod{m_{2}}$  
$x \equiv a_{3} \pmod{m_{3}}$

$M_{1} =  \frac{m_{1}m_{2}m_{3}}{m_{1}} = m_{2}m_{3}$

$M_{1} y_{1} \equiv 1 \pmod{m_{1}}$

$x=(a_{1}M_{1}y_{1} + a_{2}M_{2}y_{2} + a_{3}M_{3}y_{3}) \pmod{m_{1}}$

$x = a_{1}M_{1}y_{1} + a_{2}M_{2}y_{2} + a_{n}M_{n}y_{n}$

### Example

System of linear congruences:

$x \equiv 2 \pmod{3}$  
$x \equiv 3 \pmod{5}$  
$x \equiv 2 \pmod{7}$

$x = 7j + 2$

$7j + 2 \equiv 3 \pmod{5}$  
$7j \equiv 1 \pmod{5}$  
$2j \equiv 1 \pmod{5}$  
$j \equiv 3 \pmod{5}$

$j = 5k + 3$

$x = 7(5k + 3) + 2$  
$x = 35k + 21 + 2$  
$x = 35k + 23$

$35k + 23 \equiv 2 \pmod{3}$  
$2k + 2 \equiv 2 \pmod{3}$  
$2k \equiv 0 \pmod{3}$  
$k \equiv 0 \pmod{3}$

$k = 3m$

$x = 35(3m) + 23$  
$x = 105m + 23$

Therefore, $x \equiv 23 \pmod{105}$.

> https://brilliant.org/wiki/chinese-remainder-theorem

## Lecture Content

* **Introduction:**
	* The lecture emphasizes the importance of understanding the Euclidean Algorithm for finding the GCD, especially for large numbers.
	* Traditional prime factorization is impractical for very large numbers, which are common in cryptography.
	* Factoring large numbers into primes is computationally difficult (this difficulty underpins many cryptographic systems).
* **Euclidean Algorithm for GCD:**
	* Based on Euclid's division theorem:
		* Given integers A and B, there exist unique integers Q (quotient) and R (remainder) such that:  
		$$ A = BQ + R, \quad 0 \leq R < B $$
	* Key property: $\text{GCD}(A, B) = \text{GCD}(B, R)$.
	* The algorithm works recursively: We replace the pair A,B with the pair B, R where R is the remainder of A/B. We repeat until the remainder is zero.
	* The last non-zero remainder is the GCD.
	* **Example Iteration:** For finding the GCD of 820 and 70 the iteration is shown. This example shows that each application of the division algorithm leads to a smaller pair of numbers. (820,70) -> (70,32) -> (32, 6) -> (6,2) -> (2,0) hence GCD is 2.
	* This algorithm is considered simple and effective for finding GCD.
* **Proof of GCD Property:**
	* To prove $\text{GCD}(A, B) = \text{GCD}(B, R)$, it's necessary to show that if a number `D` is a common divisor of A and B, then it is also a common divisor of B and R, and vice-versa.
	* **Forward Direction:**
		* Assume D is a common divisor of A and B. Then A = DK1, and B = DK2.
		* From $R = A - BQ$
		* R = DK1 - DK2Q = D(K1 - K2Q), showing that D also divides R.
		* Therefore if D divides both A and B then it divides R, hence GCD of (A,B) is the same as the GCD of (B,R).
	* **Reverse Direction:**
		* Assume D is a common divisor of B and R, then B = DK1 and R = DK2.
		* From $A = BQ + R$.
		* A = DK1Q + DK2 = D(K1Q+K2), showing that D also divides A.
		* Therefore if D divides both B and R then it divides A, hence GCD of (B,R) is the same as the GCD of (A,B).
		* The algorithm works by repeatedly using these two facts.
* **Extended Euclidean Algorithm:**
	* Theorem: For any integers a and b, there exist integers x and y such that $ax + by = \text{GCD}(a, b)$.
	* The Extended Euclidean Algorithm provides a *constructive proof* for finding these integers x and y.
	* **Key Recurrence Relations for Cheat Sheet:**
		* **`x_new` = `y_old`**
		* **`y_new` = `x_old` - `q` \* `x_new`** (where q is the quotient from current division in the Euclidean Algorithm)
	* The algorithm extends the Euclidean algorithm, also calculating x and y during each step of division.
	* **Initialization**: Set `x=1`, `y=0` before running the normal Euclidean algorithm
	* These relations are used to update `x` and `y` values at each step.
	* The variables `x_old` and `y_old` refer to the x and y values in the previous step.
	* Each iteration computes a linear combination of the current values so we eventually derive the x and y values for the original numbers.
* **Example of Extended Algorithm:**
	* The lecture provides an in-depth walkthrough of applying the Extended Euclidean Algorithm.
	* Key steps include:
		1. Running the basic Euclidean Algorithm
		2. Initializing x and y as 1 and 0.
		3. Calculate values of x and y in reverse order by using the new x and y recurrence relations.
	* Each iteration has a corresponding check that can be done. The coefficients x and y are such that `ax+by = gcd(a,b)`.
* **Applications of Extended Euclidean Algorithm:**
	* Finding Modular Multiplicative Inverses:
	* If $\text{GCD}(a, m) = 1$ (a and m are relatively prime), then there exists a multiplicative inverse of a modulo m, denoted as $a^{-1}$, such that $a \cdot a^{-1} \equiv 1 \pmod{m}$.
	* The extended GCD algorithm can be used to find such multiplicative inverse, the x value found by the extended euclidean algorithm is the multiplicative inverse of a mod m (or x mod m to ensure it's positive and less than m).
	* Solving Linear Congruences:
		* Modular multiplicative inverse can be used to find the solution of a modular equation.  
		  For example to solve $ax \equiv b \pmod{m}$.
		* We multiply both sides by $a^{-1}$. $a^{-1}ax \equiv a^{-1}b \pmod{m}$. This reduces to $x \equiv a^{-1}b \pmod{m}$.
* **Modular Inverse Existence:**
	* An inverse exists if and only if $\text{GCD}(a, m) = 1$.
	* The lecturer explained using the linear combination from the extended Euclidean Algorithm. $ax + my = gcd(a,m)$.
	* If gcd(a,m) is 1 then ax +my = 1, Taking mod m of both sides gives
	* $ax + my \equiv 1 \pmod{m}$. Since my is 0 mod m, we have $ax \equiv 1 \pmod{m}$. Which satisfies the condition for x to be $a^{-1}$.
	* If the x value found by the extended Euclidean algorithm is negative it can be made positive by doing x mod m.
* **Examples and Applications:**
	* The lecturer also gave the example of 500 ml and 700 ml bottles, and explained how a combination can be found to measure 100 ml.
	* Modular arithmetic applications in hashing.
	* Examples for modular inverses were shown, including the inverse of 3 mod 7, which is 5.
	* Modular equations and solving modular congruences were also discussed with multiplicative inverses.
	* Unique solutions of a modular equations exist when gcd(a,m) = 1.
	* Real-world applications of modular arithmetic, such as ISBN and credit card check digits.
* **Check Digits:**
	* Used to detect errors in identification numbers.
	* Hong Kong ID card check digit calculation is presented as a real example. The calculation takes a weighted sum of digits then takes mod 11 to obtain a check digit.
	* The lecture shows how to analyze the checking procedure by considering possible errors.

**Highlights for Cheat Sheet:**

1. **Euclid's Division Theorem:** $A = BQ + R, 0 \leq R < B$
2. **GCD Property:** $\text{GCD}(A, B) = \text{GCD}(B, R)$
3. **Extended Euclidean Algorithm Recurrence Relations:**
	* **`x_new` = `y_old`**
	* **`y_new` = `x_old` - `q` \* `x_new`**
4. **Modular Inverse:** $a \cdot a^{-1} \equiv 1 \pmod{m}$
5. **Existence of Inverse:** Inverse exists if and only if $\text{GCD}(a, m) = 1$.
6. **Finding Inverse with Extended GCD:** If $ax + my = 1$, then $x \pmod{m}$ is the inverse of `a` mod `m`.
7. **Modular Congruence Rule** When taking modulo an expression, an additional term which is a multiple of the modulo base can be added to the expression. In $ax + my \equiv 1 \pmod{m}$, the term my can be dropped from the expression since $my \equiv 0 \pmod{m}$.

This detailed breakdown should help in understanding the key concepts from the lecture and preparing for any related assessments. Remember that working through examples of the extended Euclidean Algorithm is crucial for mastering the topic.

## Lecture Content 2

### Introduction to Chinese Remainder Theorem (CRT)

#### Relatively Prime Requirement

* The moduli must be pairwise relatively prime.

#### Mapping to Pairs

* **Example:** x (mod 3) and x (mod 5) maps x (mod 15) to unique pairs (mod 3, mod 5).
* **Function:** f(x) = (x mod 3, x mod 5) which is a 1-to-1 correspondence (bijective).
* Given a pair, you can find the original x.

#### Generalization

* With pairwise relatively prime moduli (M1, M2, …, Mn), unique x values that satisfy each equation can be found.

#### Theorem

* If M1, M2, …, Mn are pairwise relatively prime, then the system of congruences  
	x ≡ a1 (mod M1)  
	x ≡ a2 (mod M2)  
	…  
	x ≡ an (mod Mn)  
	has a unique solution modulo M = M1M2 … Mn.

#### Constructive Proof

* Provides an equation to calculate x.

#### Formula for X

* **Given:**  
	x ≡ a1 (mod M1)  
	x ≡ a2 (mod M2)  
	x ≡ a3 (mod M3)
* **Define:**  
	Mk = (M1M2M3) / Mk
	
	M1 = M2M3  
	M2 = M1M3  
	M3 = M1M2
* Find yk, where Mkyk ≡ 1 (mod Mk). The value of x is then:  
	x ≡ a1M1y1 + a2M2y2 + a3M3y3 (mod M1M2M3)
	* Mk excludes Mk from product of all the moduli.
	* yk is the modular inverse of Mk modulo Mk.
	* The equation works by having every term except for akykMk go to 0 mod Mk. The term akykMk is equal to ak mod Mk.

#### Key Idea

* The formula includes the relevant result and excludes all others using multiples of Mi

#### Cheat Sheet Note

* This formula is essential for the exam.

---

### 3. Example CRT Problem

* **Given:**  
	x ≡ 2 (mod 3)  
	x ≡ 3 (mod 5)  
	x ≡ 2 (mod 7)
* **Calculate** Mk:
	* M1 = 5 * 7 = 35
	* M2 = 3 * 7 = 21
	* M3 = 3 * 5 = 15
* **Find** yk (modular inverses):
	* 35y1 ≡ 1 (mod 3). y1 = 2.
	* 21y2 ≡ 1 (mod 5). y2 = 1.
	* 15y3 ≡ 1 (mod 7). y3 = 1.
* **Solution:**  
	x ≡ (2 * 35 * 2) + (3 * 21 * 1) + (2 * 15 * 1) (mod 105)  
	x ≡ 140 + 63 + 30 (mod 105)  
	x ≡ 233 (mod 105)  
	x ≡ 23 (mod 105)
* **Verification:** Check if 23 mod 3 = 2, 23 mod 5 = 3, and 23 mod 7 = 2

#### Cheat Sheet Note

* The process of applying the CRT, including finding M and y and calculating x, should be on the cheat sheet.

#### Exam Note

* CRT problems will likely involve multiple steps and be more complex than just plugging in numbers.

---

### 4. Introduction to Cryptography

#### Goal

* Send messages securely over insecure channels.

#### Encryption

* Convert plaintext to ciphertext

#### Decryption

* Convert ciphertext back to plaintext

#### Secret Key Cryptography

* Both sender and receiver share a secret key.
* Simple but less secure

##### Caesar Cipher

        - C = (P + k) (mod 26)
            - Map letters A-Z to 0-25
            - k is the shift value (the key).
            - Decryption: P = (C - k) (mod 26)
            - Vulnerable because of limited shift possibilities.

##### Affine Cipher

		- C = (aP + b) (mod 26)
			- A and B are keys
			- Decryption: P = a^-1(C-b) (mod 26)
			- Still vulnerable to brute force attacks.

#### Block Cipher

* Affine cipher but treating multiple letters as one block
	* Example: treat 10 bytes as a block (80 bits).
	* C = (aP+b) (mod 2^80)
	* Key space grows (more secure).
	* Still vulnerable to modern computer.

#### Key Exchange

* Problem of sharing keys securely.
	* Lockbox analogy: use your own lock then the other person locks with their own lock.
* Used for key exchange in cryptography

---

### 5. Modular Exponentiation

* Key operation in modern cryptography.
* Direct calculation of a^i can be computationally expensive.

#### Property Used

* (a * b) (mod n) = (a mod n) * (b mod n) (mod n)
* (a^i * a^j) (mod n) = (a^i mod n * a^j mod n) (mod n)

#### Repeated Squaring

* Efficient algorithm for calculating a^x (mod n)
* **Binary Representation:** Convert the exponent into binary.
	* Example: 50 = 110010_2
* Use binary representation to break exponentiation to multiplications by a^2, a^4, a^8, etc.
	* Example: a^50 = a^32 * a^16 * a^2
* **Algorithm:**
	1. Calculate a mod n
	2. Square this result and mod by n
	3. Repeat the process

#### Cheat Sheet Note

* Steps of repeated squaring, how to use the binary expansion of the exponent, how to compute a^2, a^4, a^8, etc., should all be on the cheat sheet.

#### Logarithm Assumption

* Given A^x = P (mod B), finding x (discrete logarithm) is computationally difficult.

---

### 6. Diffie-Hellman Key Exchange

* Protocol to share a key without directly exchanging it.
* Alice (you) has secret K1, Bob (your girlfriend) has secret K2
* **Public Parameters:** A and B (prime)
* Alice sends A^K1 (mod B) to Bob.
* Bob sends A^K2 (mod B) to Alice.
* **Shared secret key:**
	* Alice calculates (A^K2)^K1 (mod B)
	* Bob calculates (A^K1)^K2 (mod B)

	A^K1K2 (mod B) = A^K2K1 (mod B)
* Man-in-the-middle attack: Adversary can intercept messages and act as both parties.
