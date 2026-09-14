# STA1023 / MAT1063 — Tutorial 04 Solutions

**Course:** STA1023 / MAT1063 — Probability and Statistics  
**Institution:** University of Peradeniya — Department of Statistics and Computer Science  
**Reference Document:** [[MAT1063/STA1023__MAT1063_Tutorial 04.pdf|STA1023 / MAT1063 Tutorial 04]]  

---

## Question 1

**Problem Statement:**  
The Moment Generating Function (MGF) of a Binomial random variable is:
$$M_X(t) = \left[1 + p(e^t - 1)\right]^n$$
*(or with parameter $\theta$: $M_X(t) = [1 + \theta(e^t - 1)]^n$)*.  
Use it to derive the **mean** and the **variance** of $X \sim \text{Bin}(n, p)$.

---

### Solution

Recall the relationship between the moments of a random variable and its MGF:
1. First raw moment (Mean):  
   $$\mu = E[X] = M_X'(0) = \left. \frac{d}{dt} M_X(t) \right|_{t=0}$$
2. Second raw moment:  
   $$E[X^2] = M_X''(0) = \left. \frac{d^2}{dt^2} M_X(t) \right|_{t=0}$$
3. Variance:  
   $$\text{Var}(X) = E[X^2] - (E[X])^2 = M_X''(0) - [M_X'(0)]^2$$

---

#### Step 1: Find the First Derivative $M_X'(t)$ and the Mean $E[X]$

Given:
$$M_X(t) = [1 + p(e^t - 1)]^n$$

Differentiating with respect to $t$ using the chain rule:
$$M_X'(t) = \frac{d}{dt}\left([1 + p(e^t - 1)]^n\right) = n [1 + p(e^t - 1)]^{n-1} \cdot \frac{d}{dt}\left(1 + p(e^t - 1)\right)$$

Since $\frac{d}{dt}(1 + p e^t - p) = p e^t$:
$$M_X'(t) = n p e^t [1 + p(e^t - 1)]^{n-1}$$

Now, evaluate $M_X'(t)$ at $t = 0$:
$$e^0 = 1 \implies 1 + p(e^0 - 1) = 1 + p(0) = 1$$

Therefore:
$$E[X] = M_X'(0) = n p e^0 [1 + p(e^0 - 1)]^{n-1} = n p (1) [1]^{n-1} = np$$

$$\mathbf{E[X] = np}$$

---

#### Step 2: Find the Second Derivative $M_X''(t)$ and $E[X^2]$

We differentiate $M_X'(t) = n p \cdot \left(e^t [1 + p(e^t - 1)]^{n-1}\right)$ with respect to $t$ using the product rule:
$$M_X''(t) = np \left[ \left(\frac{d}{dt} e^t\right) [1 + p(e^t - 1)]^{n-1} + e^t \frac{d}{dt}\left([1 + p(e^t - 1)]^{n-1}\right) \right]$$

Applying the chain rule to the second term:
$$\frac{d}{dt}\left([1 + p(e^t - 1)]^{n-1}\right) = (n - 1)[1 + p(e^t - 1)]^{n-2} \cdot (p e^t)$$

Substituting this back in:
$$M_X''(t) = np \left[ e^t [1 + p(e^t - 1)]^{n-1} + e^t (n - 1)[1 + p(e^t - 1)]^{n-2} (p e^t) \right]$$
$$M_X''(t) = n p e^t [1 + p(e^t - 1)]^{n-1} + n(n-1) p^2 e^{2t} [1 + p(e^t - 1)]^{n-2}$$

Now, evaluate at $t = 0$:
$$M_X''(0) = np(1)[1]^{n-1} + n(n-1)p^2(1)[1]^{n-2}$$
$$E[X^2] = np + n(n-1)p^2 = np + n^2 p^2 - n p^2$$

---

#### Step 3: Compute the Variance $\text{Var}(X)$

$$\text{Var}(X) = E[X^2] - (E[X])^2$$
$$\text{Var}(X) = (np + n^2 p^2 - n p^2) - (np)^2$$
$$\text{Var}(X) = np - np^2 = np(1 - p)$$

Setting $q = 1 - p$:
$$\mathbf{\text{Var}(X) = np(1 - p) = npq}$$

---

## Question 2

**Problem Statement:**  
If a fair coin is tossed at random five independent times, find the conditional probability of five heads given that there are at least 4 heads.

---

### Solution

Let $X$ denote the number of heads obtained in $n = 5$ independent tosses.  
Since the coin is fair, the probability of obtaining heads on any single toss is $p = \frac{1}{2} = 0.5$.

Thus, $X$ follows a Binomial distribution:
$$X \sim \text{Bin}\left(n = 5, p = \frac{1}{2}\right)$$

The probability mass function of $X$ is:
$$P(X = k) = \binom{5}{k} \left(\frac{1}{2}\right)^k \left(\frac{1}{2}\right)^{5-k} = \binom{5}{k} \left(\frac{1}{2}\right)^5 = \frac{\binom{5}{k}}{32}$$

We want to find the conditional probability:
$$P(X = 5 \mid X \ge 4)$$

By the definition of conditional probability:
$$P(X = 5 \mid X \ge 4) = \frac{P(\{X = 5\} \cap \{X \ge 4\})}{P(X \ge 4)}$$

Since $\{X = 5\} \subset \{X \ge 4\}$, the intersection $\{X = 5\} \cap \{X \ge 4\} = \{X = 5\}$.

Hence:
$$P(X = 5 \mid X \ge 4) = \frac{P(X = 5)}{P(X \ge 4)} = \frac{P(X = 5)}{P(X = 4) + P(X = 5)}$$

Calculate the individual probabilities:
- $P(X = 5) = \frac{\binom{5}{5}}{32} = \frac{1}{32}$
- $P(X = 4) = \frac{\binom{5}{4}}{32} = \frac{5}{32}$
- $P(X \ge 4) = P(X = 4) + P(X = 5) = \frac{5}{32} + \frac{1}{32} = \frac{6}{32}$

Therefore:
$$P(X = 5 \mid X \ge 4) = \frac{\frac{1}{32}}{\frac{6}{32}} = \frac{1}{6} \approx 0.1667$$

**Final Answer:**
$$\mathbf{P(X = 5 \mid X \ge 4) = \frac{1}{6} \approx 0.1667 \quad (16.67\%)}$$

---

## Question 3

**Problem Statement:**  
A fair coin is tossed 7 times. What is the probability that 6 will appear five or more times?

---

### Solution & Analysis of Question Typo

> **Note on Question Typo:**  
> In standard probability tutorials, this question is a well-known typographical error where either:
> 1. **"coin"** was written instead of **"six-sided die"** (since the number $6$ is a face on a standard die).
> 2. **"6"** was written instead of **"heads"** (or another coin face).
> 
> Both interpretations and the literal reading are provided below for complete clarity and grading criteria.

#### Interpretation A (Intended: Fair 6-sided Die rolled 7 times)
Suppose a fair six-sided die is rolled $n = 7$ times, and we want the probability that the face **6** appears 5 or more times.
- Let $X$ be the number of times face 6 appears.
- Success probability on each roll: $p = \frac{1}{6}$, failure probability: $q = \frac{5}{6}$.
- $X \sim \text{Bin}\left(7, \frac{1}{6}\right)$.
- We seek $P(X \ge 5) = P(X = 5) + P(X = 6) + P(X = 7)$.

Computing each term:
$$P(X = 5) = \binom{7}{5} \left(\frac{1}{6}\right)^5 \left(\frac{5}{6}\right)^2 = 21 \times \frac{25}{6^7} = \frac{525}{279,936} \approx 0.0018754$$
$$P(X = 6) = \binom{7}{6} \left(\frac{1}{6}\right)^6 \left(\frac{5}{6}\right)^1 = 7 \times \frac{5}{6^7} = \frac{35}{279,936} \approx 0.0001250$$
$$P(X = 7) = \binom{7}{7} \left(\frac{1}{6}\right)^7 \left(\frac{5}{6}\right)^0 = 1 \times \frac{1}{6^7} = \frac{1}{279,936} \approx 0.0000036$$

Summing these probabilities:
$$P(X \ge 5) = \frac{525 + 35 + 1}{279,936} = \frac{561}{279,936} = \frac{187}{93,312} \approx \mathbf{0.002004} \quad (0.2004\%)$$

---

#### Interpretation B (Literal Reading: Fair Coin)
A coin has only two outcomes: Heads ($H$) and Tails ($T$). The number $6$ is impossible on a coin toss.
- Probability of observing 6 on any coin toss: $p = 0$.
- Probability of 6 appearing five or more times:
  $$\mathbf{P(X \ge 5) = 0}$$

---

#### Interpretation C (Typo for Heads appearing 5 or more times in 7 tosses)
If the question intended "Heads" appearing five or more times:
- $X \sim \text{Bin}(7, 0.5)$
$$P(X \ge 5) = P(X = 5) + P(X = 6) + P(X = 7) = \frac{\binom{7}{5} + \binom{7}{6} + \binom{7}{7}}{2^7} = \frac{21 + 7 + 1}{128} = \frac{29}{128} \approx \mathbf{0.2266} \quad (22.66\%)$$

---

## Question 4

**Problem Statement:**  
During a particular period, a university's information technology office received 20 service orders for problems with printers of which 8 were laser printers and 12 were inkjet models. A sample of 5 of these service orders is to be selected for inclusion in a customer satisfaction survey. If 5 service orders are selected randomly, what is the probability that exactly two of them were inkjet printers?

---

### Solution

This problem involves sampling **without replacement** from a finite population divided into two categories. Therefore, it follows the **Hypergeometric Distribution**.

#### Parameters:
- Total population size: $N = 20$
- Total number of inkjet printers (category of interest): $K = 12$
- Total number of laser printers: $N - K = 20 - 12 = 8$
- Sample size: $n = 5$
- Desired number of inkjet printers in the sample: $k = 2$  
  *(which implies $n - k = 5 - 2 = 3$ laser printers)*

#### Hypergeometric Probability Formula:
$$P(X = k) = \frac{\binom{K}{k} \binom{N - K}{n - k}}{\binom{N}{n}}$$

Substituting the values:
$$P(X = 2) = \frac{\binom{12}{2} \binom{8}{3}}{\binom{20}{5}}$$

#### Calculate Combinations:
1. Number of ways to choose 2 inkjet printers from 12:
   $$\binom{12}{2} = \frac{12 \times 11}{2 \times 1} = 66$$

2. Number of ways to choose 3 laser printers from 8:
   $$\binom{8}{3} = \frac{8 \times 7 \times 6}{3 \times 2 \times 1} = 56$$

3. Total number of ways to choose 5 printers from 20:
   $$\binom{20}{5} = \frac{20 \times 19 \times 18 \times 17 \times 16}{5 \times 4 \times 3 \times 2 \times 1} = 15,504$$

#### Final Calculation:
$$P(X = 2) = \frac{66 \times 56}{15,504} = \frac{3,696}{15,504}$$

Simplifying the fraction:
$$\frac{3,696}{15,504} = \frac{77}{323} \approx 0.23839$$

**Final Answer:**
$$\mathbf{P(X = 2) = \frac{77}{323} \approx 0.2384 \quad (23.84\%)}$$

---

## Question 5

**Problem Statement:**  
For a basketball player, the probability of making a free throw is 0.7 during a season.  
a) What is the probability that he makes 3 free throws out of 8 shots?  
b) What is the probability that he makes his 3rd free throw on his 5th shot?  
c) What is the probability that he makes his 1st free throw on his 4th shot?  

---

### Solution

Given:
- Probability of success (making a shot): $p = 0.7$
- Probability of failure (missing): $q = 1 - p = 0.3$

---

#### Part (a): Exactly 3 free throws out of 8 shots

Here, the number of trials is fixed at $n = 8$, and each shot is independent. This follows a **Binomial Distribution**:
$$X \sim \text{Bin}(n = 8, p = 0.7)$$

The PMF is:
$$P(X = k) = \binom{n}{k} p^k (1 - p)^{n - k}$$

For $k = 3$:
$$P(X = 3) = \binom{8}{3} (0.7)^3 (0.3)^{8 - 3} = \binom{8}{3} (0.7)^3 (0.3)^5$$

Evaluating:
- $\binom{8}{3} = \frac{8 \times 7 \times 6}{3 \times 2 \times 1} = 56$
- $(0.7)^3 = 0.343$
- $(0.3)^5 = 0.00243$

$$P(X = 3) = 56 \times 0.343 \times 0.00243 = 0.04667544 \approx \mathbf{0.0467}$$

**Answer (a):**
$$\mathbf{P(X = 3) \approx 0.0467 \quad (4.67\%)}$$

---

#### Part (b): 3rd free throw on his 5th shot

This follows a **Negative Binomial Distribution**, where we observe until the $r$-th success occurs on the $k$-th trial:
- $r = 3$ (3rd success)
- $k = 5$ (5th shot)

For the 3rd success to occur on the 5th shot:
1. Exactly $r - 1 = 2$ successes must occur in the first $k - 1 = 4$ shots.
2. The 5th shot must be a success (probability $p = 0.7$).

The formula is:
$$P(\text{3rd success on 5th shot}) = \binom{k - 1}{r - 1} p^r (1 - p)^{k - r} = \binom{4}{2} (0.7)^3 (0.3)^2$$

Evaluating:
- $\binom{4}{2} = \frac{4 \times 3}{2 \times 1} = 6$
- $(0.7)^3 = 0.343$
- $(0.3)^2 = 0.09$

$$P = 6 \times 0.343 \times 0.09 = 0.18522$$

**Answer (b):**
$$\mathbf{P = 0.1852 \quad (18.52\%)}$$

---

#### Part (c): 1st free throw on his 4th shot

This follows a **Geometric Distribution**, which models the number of trials until the 1st success:
- Trial of 1st success: $k = 4$

This means the first 3 shots are failures (misses), and the 4th shot is a success (hit):
$$P(\text{1st success on 4th shot}) = (1 - p)^3 \cdot p = (0.3)^3 \cdot (0.7)$$

Evaluating:
- $(0.3)^3 = 0.027$
- $P = 0.027 \times 0.7 = 0.0189$

**Answer (c):**
$$\mathbf{P = 0.0189 \quad (1.89\%)}$$

---

## Question 6

**Problem Statement:**  
Let $X$ be the number of typos on a printed page with a mean of 3 typos per page. Find:  
a) $P(X > 4)$  
b) $P(X = 4)$  
c) Probability that three randomly selected pages would have more than 8 typos.  

---

### Solution

The number of typos on a printed page follows a **Poisson Distribution** with parameter:
$$\lambda = 3 \text{ typos/page}$$
$$X \sim \text{Poisson}(\lambda = 3)$$

The probability mass function is:
$$P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!} = \frac{e^{-3} 3^k}{k!}, \quad k = 0, 1, 2, \dots$$
*(where $e^{-3} \approx 0.049787$)*

---

#### Part (a): $P(X > 4)$

Using the complement rule:
$$P(X > 4) = 1 - P(X \le 4) = 1 - \sum_{k=0}^{4} P(X = k)$$

Calculating each term for $k = 0, 1, 2, 3, 4$:
- $P(X = 0) = \frac{e^{-3} \cdot 3^0}{0!} = e^{-3} \approx 0.049787$
- $P(X = 1) = \frac{e^{-3} \cdot 3^1}{1!} = 3 e^{-3} \approx 0.149361$
- $P(X = 2) = \frac{e^{-3} \cdot 3^2}{2!} = 4.5 e^{-3} \approx 0.224042$
- $P(X = 3) = \frac{e^{-3} \cdot 3^3}{3!} = 4.5 e^{-3} \approx 0.224042$
- $P(X = 4) = \frac{e^{-3} \cdot 3^4}{4!} = \frac{81}{24} e^{-3} = 3.375 e^{-3} \approx 0.168031$

Summing $P(X \le 4)$:
$$P(X \le 4) = e^{-3} (1 + 3 + 4.5 + 4.5 + 3.375) = 16.375 e^{-3}$$
$$P(X \le 4) \approx 16.375 \times 0.04978707 = 0.815263$$

Thus:
$$P(X > 4) = 1 - 0.815263 = 0.184737$$

**Answer (a):**
$$\mathbf{P(X > 4) \approx 0.1847 \quad (18.47\%)}$$

---

#### Part (b): $P(X = 4)$

From our previous calculation:
$$P(X = 4) = \frac{e^{-3} \cdot 3^4}{4!} = \frac{81}{24} e^{-3} = 3.375 e^{-3}$$
$$P(X = 4) \approx 3.375 \times 0.04978707 \approx 0.168031$$

**Answer (b):**
$$\mathbf{P(X = 4) \approx 0.1680 \quad (16.80\%)}$$

---

#### Part (c): Probability that three randomly selected pages would have more than 8 typos

Let $X_1, X_2, X_3$ represent the number of typos on each of the three independent pages, where each $X_i \sim \text{Poisson}(3)$.

By the **additive property of independent Poisson random variables**, the total number of typos across the 3 pages, $Y = X_1 + X_2 + X_3$, also follows a Poisson distribution:
$$\lambda_Y = \lambda_1 + \lambda_2 + \lambda_3 = 3 + 3 + 3 = 9$$
$$Y \sim \text{Poisson}(\lambda = 9)$$

We want to find $P(Y > 8)$:
$$P(Y > 8) = 1 - P(Y \le 8) = 1 - \sum_{y=0}^8 \frac{e^{-9} 9^y}{y!}$$

Note that $e^{-9} \approx 0.0001234098$.  
Evaluating $\sum_{y=0}^{8} \frac{9^y}{y!}$:

| $y$ | $\frac{9^y}{y!}$ |
| :---: | :---: |
| 0 | $1$ |
| 1 | $9$ |
| 2 | $\frac{81}{2} = 40.5$ |
| 3 | $\frac{729}{6} = 121.5$ |
| 4 | $\frac{6561}{24} = 273.375$ |
| 5 | $\frac{59049}{120} = 492.075$ |
| 6 | $\frac{531441}{720} = 738.1125$ |
| 7 | $\frac{4782969}{5040} \approx 949.001786$ |
| 8 | $\frac{43046721}{40320} \approx 1067.627009$ |
| **Sum** | **$3692.191295$** |

$$P(Y \le 8) = 3692.191295 \times e^{-9} \approx 3692.191295 \times 0.0001234098 \approx 0.455653$$

Therefore:
$$P(Y > 8) = 1 - 0.455653 = 0.544347$$

**Answer (c):**
$$\mathbf{P(Y > 8) \approx 0.5443 \quad (54.43\%)}$$

---

## Question 7

**Problem Statement:**  
An experiment of drawing a random card from an ordinary playing cards deck is done with replacing it back. This was done ten times. Find the probability of getting 2 spades, 3 diamond, 3 clubs and 2 hearts.

---

### Solution

In an ordinary deck of 52 cards, there are 4 suits, each containing 13 cards:
1. Spades ($\spadesuit$)
2. Diamonds ($\diamondsuit$)
3. Clubs ($\clubsuit$)
4. Hearts ($\heartsuit$)

Since each card is replaced and shuffled before the next draw, each draw is independent, and the probabilities remain constant across all $n = 10$ draws:
$$p_1 = P(\text{Spade}) = \frac{13}{52} = \frac{1}{4}$$
$$p_2 = P(\text{Diamond}) = \frac{13}{52} = \frac{1}{4}$$
$$p_3 = P(\text{Club}) = \frac{13}{52} = \frac{1}{4}$$
$$p_4 = P(\text{Heart}) = \frac{13}{52} = \frac{1}{4}$$

Since there are more than two mutually exclusive outcomes, this follows the **Multinomial Distribution**:
- Total trials: $n = 10$
- Desired counts: $x_1 = 2$ (spades), $x_2 = 3$ (diamonds), $x_3 = 3$ (clubs), $x_4 = 2$ (hearts)
- Notice that $\sum_{i=1}^4 x_i = 2 + 3 + 3 + 2 = 10 = n$.

#### Multinomial Probability Formula:
$$P(X_1 = x_1, X_2 = x_2, X_3 = x_3, X_4 = x_4) = \frac{n!}{x_1! \, x_2! \, x_3! \, x_4!} p_1^{x_1} p_2^{x_2} p_3^{x_3} p_4^{x_4}$$

Substituting the values:
$$P = \frac{10!}{2! \, 3! \, 3! \, 2!} \left(\frac{1}{4}\right)^2 \left(\frac{1}{4}\right)^3 \left(\frac{1}{4}\right)^3 \left(\frac{1}{4}\right)^2$$
$$P = \frac{10!}{2! \, 3! \, 3! \, 2!} \left(\frac{1}{4}\right)^{10}$$

#### Compute Factorials:
- $10! = 3,628,800$
- $2! \, 3! \, 3! \, 2! = 2 \times 6 \times 6 \times 2 = 144$
- Multinomial coefficient:
  $$\frac{10!}{2! \, 3! \, 3! \, 2!} = \frac{3,628,800}{144} = 25,200$$

#### Compute Final Probability:
$$\left(\frac{1}{4}\right)^{10} = \frac{1}{1,048,576}$$
$$P = \frac{25,200}{1,048,576} = \frac{1,575}{65,536} \approx 0.0240326$$

**Final Answer:**
$$\mathbf{P = \frac{1575}{65536} \approx 0.0240 \quad (2.40\%)}$$

---

## Question 8

**Problem Statement:**  
During a certain month, a company sold 10,000 new watches. Past experience indicates that the probability that a new watch will need repair during its warranty period is 0.002. Compute (Using Poisson Approximation), the probability that:  
a) zero watches will need warranty work.  
b) no more than 5 watches will need warranty work.  
c) no more than 10 watches will need warranty work.  
d) no more than 20 watches will need warranty work.  

---

### Solution

We are given:
- Number of watches sold: $n = 10,000$
- Probability of needing repair: $p = 0.002$

Since $n$ is very large ($n \ge 100$) and $p$ is very small ($p \le 0.01$), the Binomial distribution $X \sim \text{Bin}(n, p)$ is well-approximated by a **Poisson Distribution** with parameter:
$$\lambda = np = 10,000 \times 0.002 = 20$$

Let $Y$ be the number of watches that need warranty repair:
$$Y \sim \text{Poisson}(\lambda = 20)$$

The Poisson PMF is:
$$P(Y = y) = \frac{e^{-\lambda} \lambda^y}{y!} = \frac{e^{-20} 20^y}{y!}, \quad y = 0, 1, 2, \dots$$

Constant value:
$$e^{-20} \approx 2.0611536 \times 10^{-9}$$

---

#### Part (a): Zero watches will need warranty work ($Y = 0$)

$$P(Y = 0) = \frac{e^{-20} \cdot 20^0}{0!} = e^{-20}$$
$$P(Y = 0) \approx 2.0612 \times 10^{-9}$$

**Answer (a):**
$$\mathbf{P(Y = 0) = e^{-20} \approx 2.0612 \times 10^{-9}}$$

---

#### Part (b): No more than 5 watches will need warranty work ($Y \le 5$)

$$P(Y \le 5) = \sum_{y=0}^5 \frac{e^{-20} \cdot 20^y}{y!} = e^{-20} \sum_{y=0}^5 \frac{20^y}{y!}$$

Computing terms:
- $y = 0: \frac{20^0}{0!} = 1$
- $y = 1: \frac{20^1}{1!} = 20$
- $y = 2: \frac{20^2}{2!} = 200$
- $y = 3: \frac{20^3}{6} \approx 1333.3333$
- $y = 4: \frac{20^4}{24} \approx 6666.6667$
- $y = 5: \frac{20^5}{120} \approx 26666.6667$

Summing:
$$\sum_{y=0}^5 \frac{20^y}{y!} = 1 + 20 + 200 + 1333.3333 + 6666.6667 + 26666.6667 = 34,887.6667$$

$$P(Y \le 5) = 34,887.6667 \times 2.0611536 \times 10^{-9} \approx 7.1909 \times 10^{-5}$$

**Answer (b):**
$$\mathbf{P(Y \le 5) \approx 7.1909 \times 10^{-5} \quad (0.00719\%)}$$

---

#### Part (c): No more than 10 watches will need warranty work ($Y \le 10$)

$$P(Y \le 10) = \sum_{y=0}^{10} \frac{e^{-20} \cdot 20^y}{y!} = e^{-20} \sum_{y=0}^{10} \frac{20^y}{y!}$$

Adding terms from $y = 6$ to $y = 10$:
- $y = 6: \frac{20^6}{720} \approx 88,888.8889$
- $y = 7: \frac{20^7}{5040} \approx 253,968.2540$
- $y = 8: \frac{20^8}{40320} \approx 634,920.6349$
- $y = 9: \frac{20^9}{362880} \approx 1,410,934.7443$
- $y = 10: \frac{20^{10}}{3628800} \approx 2,821,869.4885$

Cumulative sum for $y = 0$ to $10$:
$$\sum_{y=0}^{10} \frac{20^y}{y!} \approx 5,245,469.6772$$

$$P(Y \le 10) = 5,245,469.6772 \times 2.0611536 \times 10^{-9} \approx 0.0108117$$

**Answer (c):**
$$\mathbf{P(Y \le 10) \approx 0.0108 \quad (1.08\%)}$$

---

#### Part (d): No more than 20 watches will need warranty work ($Y \le 20$)

$$P(Y \le 20) = \sum_{y=0}^{20} \frac{e^{-20} \cdot 20^y}{y!} = e^{-20} \sum_{y=0}^{20} \frac{20^y}{y!}$$

Evaluating the cumulative sum up to the mean $\lambda = 20$:
$$\sum_{y=0}^{20} \frac{20^y}{y!} \approx 271,252,262.8808$$

$$P(Y \le 20) = 271,252,262.8808 \times 2.0611536 \times 10^{-9} \approx 0.559093$$

*(Using standard Poisson distribution tables or computer computation: $P(Y \le 20) = 0.5591$)*.

> **Alternative approximation note (Normal Approximation with continuity correction):**  
> Since $\lambda = 20 \ge 10$, we can also approximate $Y \approx N(\mu = 20, \sigma^2 = 20)$:  
> $$P(Y \le 20) \approx P\left(Z \le \frac{20 + 0.5 - 20}{\sqrt{20}}\right) = P\left(Z \le \frac{0.5}{4.472}\right) = P(Z \le 0.1118) \approx 0.5445$$  
> The exact Poisson cumulative value is **$0.5591$**.

**Answer (d):**
$$\mathbf{P(Y \le 20) \approx 0.5591 \quad (55.91\%)}$$

---
