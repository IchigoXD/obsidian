# MAT1063 / STA1023: Introduction to Probability Theory
## Complete End-Semester Exam Revision Guide & Short Notes

> **Course**: STA1023 / MAT1063 / ST102 / MT102 — *Introduction to Probability Theory*  
> **Target**: Comprehensive, Clean, Chapter-by-Chapter End-Semester Revision Sheet

---

## 📋 Course Syllabus Overview
1. **Chapter 1: Counting Techniques** (Multiplication Rule, Permutations, Combinations, Partitions)
2. **Chapter 2: Probability Concepts & Axioms** (Sample Spaces, Events, Axioms, Conditional Probability, Bayes' Theorem)
3. **Chapter 3: Probability Distributions** (Random Variables, Discrete & Continuous, PMF, PDF, CDF)
4. **Chapter 4: Mathematical Expectation & Moments** (Expectation, Variance, Moments, MGFs, Chebyshev's & Markov's Inequalities)
5. **Chapter 5: Special Discrete Probability Distributions** (Uniform, Bernoulli, Binomial, Negative Binomial, Geometric, Hypergeometric, Multinomial, Poisson)
6. **Chapter 6: Special Continuous Probability Distributions** (Continuous Uniform, Gamma, Exponential, Normal Distribution & Approximations)

---

# CHAPTER 1: COUNTING TECHNIQUES

### 1.1 Basic Principles of Counting
* **Multiplication Rule (Fundamental Principle)**:
  If a task consists of $k$ consecutive steps, where step 1 can be done in $n_1$ ways, step 2 in $n_2$ ways, ..., and step $k$ in $n_k$ ways:
  $$\text{Total ways} = n_1 \times n_2 \times \cdots \times n_k$$
* **Addition Rule**:
  If task $A$ can be done in $m$ ways and mutually exclusive task $B$ can be done in $n$ ways:
  $$\text{Total ways} = m + n$$

---

### 1.2 Permutations (Order Matters)
An arrangement of objects in a specific order.

1. **Permutations of $n$ distinct objects**:
   $$P_n = n! = n(n-1)(n-2)\cdots 3 \cdot 2 \cdot 1 \quad (\text{with } 0! = 1)$$
2. **Permutations of $n$ distinct objects taken $r$ at a time**:
   $$_n P_r = P(n, r) = \frac{n!}{(n-r)!}$$
3. **Permutations with Non-Distinct (Repetitive) Objects**:
   The number of permutations of $n$ items containing $n_1$ of type 1, $n_2$ of type 2, ..., $n_k$ of type $k$ (where $\sum n_i = n$):
   $$\frac{n!}{n_1! \, n_2! \cdots n_k!}$$
4. **Circular Permutations**:
   Arranging $n$ distinct objects around a circle (where rotations are identical):
   $$P_{\text{circle}} = (n-1)!$$
   *(If flipped over like beads on a necklace/keychain: $\frac{(n-1)!}{2}$)*.

---

### 1.3 Combinations (Order Does NOT Matter)
Selecting $r$ objects from $n$ distinct objects:
$$\binom{n}{r} = _n C_r = C(n, r) = \frac{n!}{r!(n-r)!}$$

#### Essential Algebraic Identities
* **Symmetry**: $\binom{n}{r} = \binom{n}{n-r}$
* **Pascal's Identity** *(frequent exam proof)*:
  $$\binom{n}{r} = \binom{n-1}{r-1} + \binom{n-1}{r}$$
  *Proof*:
  $$\begin{aligned}
  \binom{n-1}{r-1} + \binom{n-1}{r} &= \frac{(n-1)!}{(r-1)!(n-r)!} + \frac{(n-1)!}{r!(n-1-r)!} \\
  &= \frac{(n-1)! \cdot r}{r!(n-r)!} + \frac{(n-1)! \cdot (n-r)}{r!(n-r)!} \\
  &= \frac{(n-1)![r + n - r]}{r!(n-r)!} = \frac{n!}{r!(n-r)!} = \binom{n}{r} \quad \blacksquare
  \end{aligned}$$

---

### 1.4 Partitions of a Set
The number of ways to partition $n$ distinct objects into $k$ distinct cells containing $n_1, n_2, \dots, n_k$ objects (with $\sum_{i=1}^k n_i = n$):
$$\binom{n}{n_1, n_2, \dots, n_k} = \frac{n!}{n_1! \, n_2! \cdots n_k!}$$

---

### 🎯 High-Yield Exam Problem Patterns (Ch. 1)
1. **Circular Table Seating with Restrictions**:
   * *Alternate boys and girls ($n$ boys, $n$ girls)*: Seat the $n$ boys in $(n-1)!$ ways. The $n$ girls then sit in the $n$ distinct spaces between boys in $n!$ ways $\implies (n-1)! \times n!$.
   * *Two specific people refuse to sit together*:
     $$\text{Allowed} = \text{Total circular arrangements} - \text{Arrangements where they sit together}$$
     $$\text{Total} = (N-1)!$$
     Treat the 2 as a single block: $(N-2)! \times 2! \implies \text{Result} = (N-1)! - 2(N-2)! = (N-3)(N-2)!$.
2. **Book Arranging on a Shelf**:
   * Books of same subject must stay together: Arrange the subjects as blocks, then permute books internally within each block.

---

# CHAPTER 2: PROBABILITY CONCEPTS & AXIOMS

### 2.1 Basic Terminology & Sample Spaces
* **Random Experiment**: A process yielding unpredictable individual outcomes, but with a well-defined set of all possible outcomes.
* **Sample Space ($S$ or $\Omega$)**: The set of all possible outcomes.
  * *Discrete*: Finite or countably infinite.
  * *Continuous*: Intervals of real numbers.
* **Event ($A \subseteq S$)**: Any subset of the sample space.

---

### 2.2 Axioms of Probability (Kolmogorov's Axioms)
For any event $A$ in sample space $S$:
1. **Axiom 1 (Non-negativity)**: $P(A) \ge 0$
2. **Axiom 2 (Certainty)**: $P(S) = 1$
3. **Axiom 3 (Additivity)**: For mutually exclusive events $A_1, A_2, \dots$ ($A_i \cap A_j = \emptyset$ for $i \ne j$):
   $$P\left(\bigcup_{i=1}^\infty A_i\right) = \sum_{i=1}^\infty P(A_i)$$

#### Derived Probability Rules
* $P(\emptyset) = 0$
* **Complement Rule**: $P(A') = 1 - P(A)$
* $0 \le P(A) \le 1$
* If $A \subseteq B \implies P(A) \le P(B)$ and $P(B - A) = P(B \cap A') = P(B) - P(A)$
* **General Addition Rule**:
  $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
  For three events:
  $$P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(A \cap C) - P(B \cap C) + P(A \cap B \cap C)$$

---

### 2.3 Conditional Probability & Independence

#### Conditional Probability
The probability that event $A$ occurs given that event $B$ has already occurred ($P(B) > 0$):
$$P(A \mid B) = \frac{P(A \cap B)}{P(B)}$$

#### Multiplication Rule
$$P(A \cap B) = P(B) \cdot P(A \mid B) = P(A) \cdot P(B \mid A)$$
For $k$ events:
$$P(A_1 \cap A_2 \cap \cdots \cap A_k) = P(A_1) P(A_2 \mid A_1) P(A_3 \mid A_1 \cap A_2) \cdots P(A_k \mid A_1 \cap \cdots \cap A_{k-1})$$

#### Independence of Events
Events $A$ and $B$ are **statistically independent** if and only if:
$$P(A \cap B) = P(A) \cdot P(B) \iff P(A \mid B) = P(A) \iff P(B \mid A) = P(B)$$
> ⚠️ **Warning**: Never confuse *mutually exclusive* ($A \cap B = \emptyset \implies P(A \cap B) = 0$) with *independent* ($P(A \cap B) = P(A)P(B)$). Two non-impossible events cannot be both!

---

### 2.4 Law of Total Probability & Bayes' Theorem

#### Partition of a Sample Space
Sets $B_1, B_2, \dots, B_k$ form a partition of $S$ if:
1. $B_i \cap B_j = \emptyset$ for $i \ne j$ (pairwise mutually exclusive)
2. $\bigcup_{i=1}^k B_i = S$ (exhaustive)
3. $P(B_i) > 0$ for all $i$.

#### 1. Law of Total Probability
For any event $A$ in $S$:
$$P(A) = \sum_{i=1}^k P(B_i) \cdot P(A \mid B_i)$$

#### 2. Bayes' Theorem
Calculates the posterior probability $P(B_r \mid A)$ given evidence $A$:
$$P(B_r \mid A) = \frac{P(B_r \cap A)}{P(A)} = \frac{P(B_r) \cdot P(A \mid B_r)}{\sum_{i=1}^k P(B_i) \cdot P(A \mid B_i)}$$

---

# CHAPTER 3: PROBABILITY DISTRIBUTIONS

### 3.1 Random Variables (RVs)
A random variable $X$ is a real-valued function defined over the sample space $S$, mapping each outcome $s \in S$ to a real number $X(s) \in \mathbb{R}$.

---

### 3.2 Discrete Random Variables
$X$ takes isolated/countable values $\{x_1, x_2, \dots\}$.

1. **Probability Mass Function (PMF)**: $f(x) = P(X = x)$
   * Valid PMF conditions:
     1. $f(x) \ge 0 \quad \forall x$
     2. $\sum_x f(x) = 1$
2. **Cumulative Distribution Function (CDF)**:
   $$F(x) = P(X \le x) = \sum_{t \le x} f(t)$$
   * Step function: right-continuous, non-decreasing, $\lim_{x \to -\infty} F(x) = 0$, $\lim_{x \to \infty} F(x) = 1$.
   * Jump height at $x_i$ equals $P(X = x_i) = F(x_i) - F(x_{i}^-)$.

---

### 3.3 Continuous Random Variables
$X$ takes values in a continuous interval or union of intervals.

1. **Probability Density Function (PDF)**: $f(x)$
   * Valid PDF conditions:
     1. $f(x) \ge 0 \quad \forall x \in \mathbb{R}$
     2. $\int_{-\infty}^\infty f(x) \, dx = 1$
   * Point probability is zero: $P(X = c) = \int_c^c f(x)dx = 0$.
   * Interval probability:
     $$P(a \le X \le b) = P(a < X < b) = \int_a^b f(x) \, dx$$
2. **Cumulative Distribution Function (CDF)**:
   $$F(x) = P(X \le x) = \int_{-\infty}^x f(t) \, dt$$
   * Fundamental Theorem of Calculus:
     $$f(x) = \frac{d}{dx} F(x) \quad (\text{wherever } F \text{ is differentiable})$$
3. **Median of $X$**:
   The value $m$ such that $F(m) = 0.5 \iff \int_{-\infty}^m f(x)dx = 0.5$.

---

# CHAPTER 4: MATHEMATICAL EXPECTATION & MOMENTS

### 4.1 Expected Value $E[X]$
* **Discrete**: $E[X] = \sum_x x f(x)$
* **Continuous**: $E[X] = \int_{-\infty}^\infty x f(x) \, dx$
* *Existence Condition*: The sum/integral must converge absolutely ($\sum |x|f(x) < \infty$).

#### Properties of Expectation
* $E[c] = c$
* $E[aX + b] = a E[X] + b$
* $E[g(X)] = \begin{cases} \sum_x g(x) f(x) & \text{(discrete)} \\ \int_{-\infty}^\infty g(x) f(x) dx & \text{(continuous)} \end{cases}$
* $E\left[\sum c_i g_i(X)\right] = \sum c_i E[g_i(X)]$

---

### 4.2 Moments and Variance

| Moment Concept | Notation | Discrete Formula | Continuous Formula |
| :--- | :--- | :--- | :--- |
| **$r$-th moment about origin** | $\mu'_r = E[X^r]$ | $\sum_x x^r f(x)$ | $\int_{-\infty}^\infty x^r f(x) dx$ |
| **Mean (1st raw moment)** | $\mu = \mu'_1 = E[X]$ | $\sum_x x f(x)$ | $\int_{-\infty}^\infty x f(x) dx$ |
| **$r$-th central moment** | $\mu_r = E[(X-\mu)^r]$ | $\sum_x (x-\mu)^r f(x)$ | $\int_{-\infty}^\infty (x-\mu)^r f(x) dx$ |
| **Variance** | $\sigma^2 = \text{Var}(X) = \mu_2$ | $\sum_x (x-\mu)^2 f(x)$ | $\int_{-\infty}^\infty (x-\mu)^2 f(x) dx$ |

#### Key Computational Rules
* $\mu_0 = 1, \quad \mu_1 = 0$ (Always zero for any distribution!)
* **Working formula for variance**:
  $$\sigma^2 = \text{Var}(X) = E[X^2] - (E[X])^2 = \mu'_2 - \mu^2$$
* **Linear transformation of variance**:
  $$\text{Var}(aX + b) = a^2 \text{Var}(X)$$
  $$\text{SD}(aX + b) = |a| \sigma_X$$

---

### 4.3 Moment Generating Function (MGF)
* **Definition**:
  $$M_X(t) = E[e^{tX}] = \begin{cases} \sum_x e^{tx} f(x) & \text{(discrete)} \\ \int_{-\infty}^\infty e^{tx} f(x) dx & \text{(continuous)} \end{cases}$$
* **Maclaurin Expansion**:
  $$M_X(t) = 1 + \mu'_1 t + \mu'_2 \frac{t^2}{2!} + \dots + \mu'_r \frac{t^r}{r!} + \dots$$
  $$\mu'_r = \left. \frac{d^r M_X(t)}{dt^r} \right|_{t=0} = M_X^{(r)}(0)$$
  * $E[X] = M'_X(0)$
  * $E[X^2] = M''_X(0)$
  * $\text{Var}(X) = M''_X(0) - [M'_X(0)]^2$
* **Linear Transformation Property of MGF**:
  $$M_{aX+b}(t) = E[e^{t(aX+b)}] = e^{bt} E[e^{(at)X}] = e^{bt} M_X(at)$$
  *Special case*: $M_{\frac{X+a}{b}}(t) = e^{\frac{a}{b}t} M_X\left(\frac{t}{b}\right)$.

---

### 4.4 Chebyshev's Inequality & Markov's Inequality

#### Markov's Inequality
If $X$ is a non-negative random variable ($P(X \ge 0) = 1$) with mean $\mu$, then for any $a > 0$:
$$P(X \ge a) \le \frac{E[X]}{a} = \frac{\mu}{a}$$

#### Chebyshev's Theorem
For any random variable $X$ with finite mean $\mu$ and standard deviation $\sigma$, and any constant $k > 0$:
$$P(|X - \mu| < k\sigma) \ge 1 - \frac{1}{k^2} \iff P(\mu - k\sigma < X < \mu + k\sigma) \ge 1 - \frac{1}{k^2}$$
* **Tail probability**: $P(|X - \mu| \ge k\sigma) \le \frac{1}{k^2}$
* **Key values**:
  * $k = 2$: $P(|X-\mu| < 2\sigma) \ge 1 - \frac{1}{4} = 75\%$
  * $k = 3$: $P(|X-\mu| < 3\sigma) \ge 1 - \frac{1}{9} \approx 88.89\%$
* *Continuous Proof Step-by-Step*:
  $$\sigma^2 = \int_{-\infty}^\infty (x-\mu)^2 f(x)dx \ge \int_{|x-\mu| \ge k\sigma} (x-\mu)^2 f(x)dx \ge k^2\sigma^2 \int_{|x-\mu| \ge k\sigma} f(x)dx = k^2\sigma^2 P(|X-\mu| \ge k\sigma)$$
  Dividing by $k^2\sigma^2 \implies P(|X-\mu| \ge k\sigma) \le \frac{1}{k^2} \implies P(|X-\mu| < k\sigma) \ge 1 - \frac{1}{k^2} \quad \blacksquare$

---

# CHAPTER 5: SPECIAL DISCRETE DISTRIBUTIONS

### 5.1 Master Comparison Table

| Distribution | Physical Meaning / When to Use | PMF $P(X=x)$ | Support ($x$) | Mean $\mu$ | Variance $\sigma^2$ | MGF $M_X(t)$ |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Discrete Uniform** | $k$ equally likely outcomes | $\frac{1}{k}$ | $1, 2, \dots, k$ | $\frac{k+1}{2}$ | $\frac{k^2-1}{12}$ | — |
| **Bernoulli** | 1 trial with success probability $\theta$ | $\theta^x (1-\theta)^{1-x}$ | $x \in \{0, 1\}$ | $\theta$ | $\theta(1-\theta)$ | $1 - \theta + \theta e^t$ |
| **Binomial** $(n, \theta)$ | Number of successes in $n$ independent trials | $\binom{n}{x}\theta^x(1-\theta)^{n-x}$ | $0, 1, \dots, n$ | $n\theta$ | $n\theta(1-\theta)$ | $[1+\theta(e^t-1)]^n$ |
| **Negative Binomial** | Trial number $x$ on which the $k$-th success occurs | $\binom{x-1}{k-1}\theta^k(1-\theta)^{x-k}$ | $k, k+1, k+2, \dots$ | $\frac{k}{\theta}$ | $\frac{k(1-\theta)}{\theta^2}$ | — |
| **Geometric** $(\theta)$ | Trial number $x$ on which **1st** success occurs ($k=1$) | $\theta(1-\theta)^{x-1}$ | $1, 2, 3, \dots$ | $\frac{1}{\theta}$ | $\frac{1-\theta}{\theta^2}$ | $\frac{\theta e^t}{1-(1-\theta)e^t}$ |
| **Hypergeometric** | Successes in sample $n$ **without replacement** from $N$ (contains $M$ defectives) | $\frac{\binom{M}{x}\binom{N-M}{n-x}}{\binom{N}{n}}$ | $\max(0, n-N+M) \le x \le \min(n, M)$ | $n\frac{M}{N}$ | $n\frac{M}{N}\left(1-\frac{M}{N}\right)\left(\frac{N-n}{N-1}\right)$ | — |
| **Multinomial** | Generalization of Binomial to $k$ mutually exclusive outcomes | $\frac{n!}{x_1! \cdots x_k!} \theta_1^{x_1}\cdots\theta_k^{x_k}$ | $\sum x_i = n$ | $E[X_i] = n\theta_i$ | $\text{Var}(X_i) = n\theta_i(1-\theta_i)$ | — |
| **Poisson** $(\lambda)$ | Count of rare events over fixed continuous interval / area | $\frac{\lambda^x e^{-\lambda}}{x!}$ | $0, 1, 2, \dots$ | $\lambda$ | $\lambda$ | $e^{\lambda(e^t-1)}$ |

*(Note: In exam formulas, the course notation uses $\theta$ or $p$ interchangeably for success probability).*

---

### 5.2 Critical Chapter 5 Theorems & Identities
1. **Binomial Symmetry**:
   $$b(x; n, \theta) = b(n-x; n, 1-\theta)$$
2. **Negative Binomial to Binomial Relation**:
   $$b^*(x; k, \theta) = \frac{k}{x} b(k; x, \theta)$$
3. **Binomial MGF Derivation**:
   $$M_X(t) = \sum_{x=0}^n e^{tx} \binom{n}{x} \theta^x (1-\theta)^{n-x} = \sum_{x=0}^n \binom{n}{x}(\theta e^t)^x (1-\theta)^{n-x} = [(1-\theta) + \theta e^t]^n = [1 + \theta(e^t - 1)]^n$$
4. **Poisson MGF Derivation**:
   $$M_X(t) = \sum_{x=0}^\infty e^{tx} \frac{\lambda^x e^{-\lambda}}{x!} = e^{-\lambda} \sum_{x=0}^\infty \frac{(\lambda e^t)^x}{x!} = e^{-\lambda} e^{\lambda e^t} = e^{\lambda(e^t - 1)}$$
5. **Poisson Moment Recursive Property**:
   $$E[X^n] = \lambda E[(X+1)^{n-1}] \quad (\text{for } n \ge 1)$$
   *Proof*:
   $$E[X^n] = \sum_{x=0}^\infty x^n \frac{\lambda^x e^{-\lambda}}{x!} = \sum_{x=1}^\infty x \cdot x^{n-1} \frac{\lambda \cdot \lambda^{x-1} e^{-\lambda}}{x(x-1)!} = \lambda \sum_{x=1}^\infty x^{n-1} \frac{\lambda^{x-1} e^{-\lambda}}{(x-1)!}$$
   Let $y = x-1 \implies x = y+1$:
   $$E[X^n] = \lambda \sum_{y=0}^\infty (y+1)^{n-1} \frac{\lambda^y e^{-\lambda}}{y!} = \lambda E[(X+1)^{n-1}] \quad \blacksquare$$

---

# CHAPTER 6: SPECIAL CONTINUOUS DISTRIBUTIONS

### 6.1 Continuous Uniform Distribution $U(\alpha, \beta)$
* **PDF**: $f(x) = \frac{1}{\beta - \alpha}$ for $\alpha < x < \beta$, and $0$ elsewhere.
* **CDF**: $F(x) = \begin{cases} 0 & x < \alpha \\ \frac{x - \alpha}{\beta - \alpha} & \alpha \le x \le \beta \\ 1 & x > \beta \end{cases}$
* **Mean & Variance**:
  $$\mu = \frac{\alpha + \beta}{2}, \qquad \sigma^2 = \frac{(\beta - \alpha)^2}{12}$$

---

### 6.2 Gamma Distribution
* **Gamma Function Definition**:
  $$\Gamma(\alpha) = \int_0^\infty y^{\alpha-1} e^{-y} \, dy \quad (\alpha > 0)$$
  *Properties*: $\Gamma(1) = 1, \quad \Gamma(\alpha + 1) = \alpha \Gamma(\alpha), \quad \Gamma(n) = (n-1)! \text{ for integer } n, \quad \Gamma\left(\frac{1}{2}\right) = \sqrt{\pi}$.
* **PDF**:
  $$f(x) = \frac{1}{\beta^\alpha \Gamma(\alpha)} x^{\alpha-1} e^{-x/\beta} \quad (x > 0; \, \alpha > 0, \, \beta > 0)$$
* **$r$-th Moment about Origin**:
  $$\mu'_r = \beta^r \frac{\Gamma(\alpha + r)}{\Gamma(\alpha)}$$
* **Mean, Variance & MGF**:
  $$\mu = \alpha\beta, \qquad \sigma^2 = \alpha\beta^2, \qquad M_X(t) = (1 - \beta t)^{-\alpha} \quad (t < 1/\beta)$$
* **Poisson Connection**: Waiting time until the $r$-th Poisson event with rate $\lambda$:
  $$\text{Gamma with } \alpha = r, \quad \beta = \frac{1}{\lambda}$$

---

### 6.3 Exponential Distribution
Special case of Gamma where $\alpha = 1$ and $\beta = \theta$ (or rate parameter $\lambda = \frac{1}{\theta}$):
* **PDF**: $f(x) = \frac{1}{\theta} e^{-x/\theta}$ for $x > 0$.
* **CDF**: $F(x) = 1 - e^{-x/\theta}$ for $x > 0$.
* **Mean & Variance**:
  $$\mu = \theta, \qquad \sigma^2 = \theta^2$$
* **Key Role**: Models the waiting time until the **first** Poisson event, or time between consecutive events.
* **Memoryless Property**: $P(X > s + t \mid X > s) = P(X > t)$.

---

### 6.4 Normal (Gaussian) Distribution $N(\mu, \sigma^2)$
* **PDF**:
  $$f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x - \mu}{\sigma}\right)^2} \quad (-\infty < x < \infty)$$
* **MGF**:
  $$M_X(t) = e^{\mu t + \frac{1}{2}\sigma^2 t^2}$$
* **Standardization**:
  $$Z = \frac{X - \mu}{\sigma} \sim N(0, 1) \implies P(a \le X \le b) = P\left(\frac{a - \mu}{\sigma} \le Z \le \frac{b - \mu}{\sigma}\right) = \Phi(z_2) - \Phi(z_1)$$
* **Symmetry Property**:
  $$\Phi(-z) = 1 - \Phi(z)$$
* **Empirical Rule**:
  * $\mu \pm 1\sigma \approx 68.26\%$
  * $\mu \pm 2\sigma \approx 95.44\%$
  * $\mu \pm 3\sigma \approx 99.74\%$

---

### 6.5 Distribution Approximations & Continuity Correction

| Approximation | Conditions | Parameters to Use | Continuity Correction Rule |
| :--- | :--- | :--- | :--- |
| **Poisson approx to Binomial** | $n \ge 20$ and $\theta \le 0.05$ (or $n \ge 100, n\theta < 10$) | $\lambda = n\theta$ | Discrete to Discrete (no correction needed) |
| **Normal approx to Binomial** | $n\theta > 5$ and $n(1-\theta) > 5$ | $\mu = n\theta$, $\sigma = \sqrt{n\theta(1-\theta)}$ | $P(X \le k) \approx P(Y \le k + 0.5)$<br>$P(X \ge k) \approx P(Y \ge k - 0.5)$<br>$P(X = k) \approx P(k - 0.5 \le Y \le k + 0.5)$ |
| **Normal approx to Poisson** | $\lambda > 20$ (or large $\lambda \ge 15$) | $\mu = \lambda$, $\sigma = \sqrt{\lambda}$ | Same $\pm 0.5$ continuity correction |

---

# 🎯 END-SEMESTER EXAM: FREQUENT QUESTION TYPES & STEP-BY-STEP CHECKLIST

| Question Type                                 | Standard Strategy & Steps                                                                                                                                                                                                                                                                                                                       |
| :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Find constant $k$ or $a$ for PDF / PMF** | Set $\sum f(x) = 1$ (discrete) or $\int_{-\infty}^\infty f(x)dx = 1$ (continuous), evaluate the definite integral and solve for constant.                                                                                                                                                                                                       |
| **2. Derive CDF from PDF**                    | Integrate piecewise: $F(x) = \int_{-\infty}^x f(t)dt$. Write clearly using piecewise brackets for all domains ($x < a$, $a \le x \le b$, $x > b$).                                                                                                                                                                                              |
| **3. Derive MGF and Moments**                 | 1. Compute $M_X(t) = E[e^{tX}]$.<br>2. Differentiate: $E[X] = M'_X(0)$, $E[X^2] = M''_X(0)$.<br>3. Calculate $\text{Var}(X) = M''_X(0) - (M'_X(0))^2$.                                                                                                                                                                                          |
| **4. Chebyshev's Bound**                      | 1. Identify/calculate $\mu$ and $\sigma$.<br>2. Set interval $(\mu - k\sigma, \mu + k\sigma)$ to find $k$.<br>3. Apply lower bound: $P \ge 1 - \frac{1}{k^2}$.                                                                                                                                                                                  |
| **5. Identifying Discrete Distribution**      | • Fixed $n$ trials, count successes $\implies$ **Binomial**<br>• Count trials until 1st success $\implies$ **Geometric**<br>• Count trials until $k$-th success $\implies$ **Negative Binomial**<br>• Sampling *without replacement* from finite lot $\implies$ **Hypergeometric**<br>• Counts over continuous time/area $\implies$ **Poisson** |
| **6. Normal Distribution Problems**           | 1. State $X \sim N(\mu, \sigma^2)$.<br>2. Convert to $Z = \frac{X - \mu}{\sigma}$.<br>3. Look up $\Phi(z)$ in standard normal tables. If negative, use $\Phi(-z) = 1 - \Phi(z)$.                                                                                                                                                                |

---

*Compiled from STA1023 / MAT1063 lecture notes, tutorial solutions, and past end-semester examination papers (2023 & 2024).*
