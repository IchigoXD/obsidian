# MAT1063 - Quiz Cheatsheet & 6-Hour Study Plan
**Chapters Covered**: Chapter 4 (Mathematical Expectation, Moments, MGFs, Chebyshev's Inequality) & Chapter 5 (Special Discrete Probability Distributions)
**Source Materials**:
- [[MAT1063/Chapte 4 - Notes.pdf|Chapter 4 - Notes]]
- [[MAT1063/Chapte 4 - Chebyshevs Inequality.pdf|Chapter 4 - Chebyshev's Inequality]]
- [[MAT1063/Chapter 5-Part 1 and 2.pdf|Chapter 5 - Part 1 & 2]]
- [[MAT1063/Chapter 5 Notes-Part 3.pdf|Chapter 5 - Part 3]]
- [[MAT1063/Chapter 5 Notes-Part 4.pdf|Chapter 5 - Part 4]]

---

## ⏱️ 6-Hour High-Yield Study Plan

>[!tip] Strategy
> Do not passively re-read slides. Spend 60% of each block actively deriving formulas and doing problem calculations on scratch paper.

| Time Block | Topic | High-Yield Action Items |
| :--- | :--- | :--- |
| **Hour 1** (0:00 – 1:00) | **Expectation, Moments & MGF** | • Master $E[aX+b] = aE[X]+b$ and $\text{Var}(aX+b) = a^2\text{Var}(X)$.<br>• Practice finding unknown constant $k$ in a PDF $\int f(x)dx = 1$.<br>• Practice evaluating moments from MGF: $\mu'_r = \left.\frac{d^r M_X(t)}{dt^r}\right|_{t=0}$. |
| **Hour 2** (1:00 – 2:00) | **Chebyshev’s & Markov’s Inequalities** | • **CRITICAL:** Memorize the continuous proof for Chebyshev's Theorem step-by-step (dedicated PDF in course).<br>• Calculate bounds for $2\sigma$ ($75\%$) and $3\sigma$ ($88.89\%$). |
| **Hour 3** (2:00 – 3:15) | **Binomial, Negative Binomial, Geometric** | • Memorize PMFs, means, and variances.<br>• Understand trial definitions: Binomial ($n$ trials, $x$ successes), Neg-Binomial ($x$ trials until $k$-th success), Geometric ($x$ trials until 1st success).<br>• Learn identity $b^*(x; k, \theta) = \frac{k}{x} b(k; x, \theta)$. |
| **Hour 4** (3:15 – 4:30) | **Hypergeometric, Multinomial, Poisson** | • Hypergeometric: sampling **without replacement**; finite population correction $\frac{N-n}{N-1}$.<br>• Poisson process over continuous domain: $\lambda = \alpha t$.<br>• Conditions for Binomial & Poisson approximations. |
| **Hour 5** (4:30 – 5:30) | **Active Retrieval & Proof Practice** | • Write all 4 major derivations from blank memory (Chebyshev, Binomial MGF, Poisson MGF, $b^* \leftrightarrow b$).<br>• Re-solve all slide examples independently. |
| **Hour 6** (5:30 – 6:00) | **Final Formula Flash & Sleep** | • Review the Summary Matrix table below, check calculator modes, and rest! |

---

# PART 1: CHAPTER 4 – MATHEMATICAL EXPECTATION & MOMENTS

### 1.1 Expected Value $E[X]$

* **Discrete**:
  $$E[X] = \sum_x x \cdot P(x)$$
* **Continuous**:
  $$E[X] = \int_{-\infty}^{\infty} x \cdot f(x) \, dx$$
* **Existence Condition**: The sum or integral must converge absolutely ($\sum |x|P(x) < \infty$). Otherwise, $E[X]$ is **undefined**.
* **Expectation of a Function $g(X)$**:
  * Discrete: $E[g(X)] = \sum_x g(x) P(x)$
  * Continuous: $E[g(X)] = \int_{-\infty}^{\infty} g(x) f(x) \, dx$

#### Linearity Theorems
* $E[c] = c$ (for constant $c$)
* $E[aX + b] = a E[X] + b$
* $E\left[\sum_{i=1}^n c_i g_i(X)\right] = \sum_{i=1}^n c_i E[g_i(X)]$

---

### 1.2 Moments & Variance

* **$r$-th Moment about the Origin**:
  $$\mu'_r = E[X^r]$$
  * $\mu'_0 = 1$
  * $\mu'_1 = E[X] = \mu$ (**Mean**)
* **$r$-th Moment about the Mean (Central Moment)**:
  $$\mu_r = E[(X - \mu)^r]$$
  * $\mu_0 = 1$
  * $\mu_1 = E[X - \mu] = E[X] - \mu = 0$ *(Always zero for any distribution!)*
  * $\mu_2 = E[(X - \mu)^2] = \text{Var}(X) = \sigma^2$ (**Variance**)
* **Computational Formula for Variance**:
  $$\sigma^2 = \mu'_2 - \mu^2 = E[X^2] - (E[X])^2$$
* **Variance Properties**:
  * $\text{Var}(aX + b) = a^2 \text{Var}(X) = a^2 \sigma^2$ *(Adding constant $b$ does not alter spread)*
  * Standard deviation: $\sigma_{aX+b} = |a| \sigma_X$

---

### 1.3 Moment Generating Function (MGF)

* **Definition**:
  $$M_X(t) = E[e^{tX}] = \begin{cases} \sum_x e^{tx} P(x) & \text{(discrete)} \\ \int_{-\infty}^\infty e^{tx} f(x) \, dx & \text{(continuous)} \end{cases}$$
  *(Defined for $t$ in an open neighborhood around 0)*

* **Connection to Moments (Maclaurin Expansion)**:
  $$e^{tX} = 1 + tX + \frac{t^2 X^2}{2!} + \dots + \frac{t^r X^r}{r!} + \dots$$
  $$M_X(t) = 1 + \mu'_1 t + \mu'_2 \frac{t^2}{2!} + \dots + \mu'_r \frac{t^r}{r!} + \dots$$
  >[!info] Core Insight
  > The $r$-th raw moment $\mu'_r$ is the **coefficient of $\frac{t^r}{r!}$** in the series expansion of $M_X(t)$.

* **Derivative Formula for Moments**:
  $$\mu'_r = \left. \frac{d^r M_X(t)}{dt^r} \right|_{t=0} = M_X^{(r)}(0)$$
  * $E[X] = M'_X(0)$
  * $E[X^2] = M''_X(0)$
  * $\text{Var}(X) = M''_X(0) - [M'_X(0)]^2$

---

### 1.4 Chebyshev's Theorem & Markov's Inequality

#### Chebyshev's Theorem
For **any** random variable $X$ with finite mean $\mu$ and standard deviation $\sigma$, and any constant $k > 0$:
$$P(|X - \mu| < k\sigma) \ge 1 - \frac{1}{k^2} \iff P(\mu - k\sigma < X < \mu + k\sigma) \ge 1 - \frac{1}{k^2}$$
* **Tail (outside $k$ standard deviations)**:
  $$P(|X - \mu| \ge k\sigma) \le \frac{1}{k^2}$$
* **Standard benchmark bounds**:
  * $k = 2$: $P(|X-\mu| < 2\sigma) \ge 1 - \frac{1}{4} = 75\%$
  * $k = 3$: $P(|X-\mu| < 3\sigma) \ge 1 - \frac{1}{9} = \frac{8}{9} \approx 88.89\%$
  * $k = 4$: $P(|X-\mu| < 4\sigma) \ge 1 - \frac{1}{16} = \frac{15}{16} = 93.75\%$
* *Note:* Chebyshev provides only a **lower bound**. If the true distribution is known, always calculate the exact probability.

#### Markov's Inequality
If $X$ takes only non-negative values ($f(x) = 0$ for $x < 0$) with mean $\mu$:
$$P(X \ge a) \le \frac{\mu}{a} \quad (\forall a > 0)$$

---

# PART 2: CHAPTER 5 – SPECIAL DISCRETE DISTRIBUTIONS

### 2.1 Master Comparison Table

| Distribution | What $X$ Represents | PMF $P(X=x)$ | Support ($x$) | Mean $\mu$ | Variance $\sigma^2$ | MGF $M_X(t)$ |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Discrete Uniform** | Equally likely outcomes $1..k$ | $\frac{1}{k}$ | $1, 2, \dots, k$ | $\frac{k+1}{2}$ | $\frac{k^2-1}{12}$ | — |
| **Bernoulli** | Single trial outcome (1 or 0) | $\theta^x(1-\theta)^{1-x}$ | $x \in \{0, 1\}$ | $\theta$ | $\theta(1-\theta)$ | $1 - \theta + \theta e^t$ |
| **Binomial** | Successes in $n$ independent trials | $\binom{n}{x}\theta^x(1-\theta)^{n-x}$ | $x=0, 1, \dots, n$ | $n\theta$ | $n\theta(1-\theta)$ | $[1+\theta(e^t-1)]^n$ |
| **Negative Binomial** | Trial number $x$ of the $k$-th success | $\binom{x-1}{k-1}\theta^k(1-\theta)^{x-k}$ | $x=k, k+1, \dots$ | $\frac{k}{\theta}$ | $\frac{k(1-\theta)}{\theta^2}$ | — |
| **Geometric** | Trial number $x$ of **1st** success ($k=1$) | $\theta(1-\theta)^{x-1}$ | $x=1, 2, \dots$ | $\frac{1}{\theta}$ | $\frac{1-\theta}{\theta^2}$ | — |
| **Hypergeometric** | Successes in sample $n$ **without replacement** | $\frac{\binom{M}{x}\binom{N-M}{n-x}}{\binom{N}{n}}$ | $\max(0, n-N+M) \le x \le \min(n, M)$ | $n\frac{M}{N}$ | $n\frac{M}{N}\left(1-\frac{M}{N}\right)\left(\frac{N-n}{N-1}\right)$ | — |
| **Multinomial** | Joint counts for $k$ distinct categories | $\frac{n!}{x_1! \cdots x_k!} \theta_1^{x_1} \cdots \theta_k^{x_k}$ | $\sum x_i = n$ | $E[X_i] = n\theta_i$ | $\text{Var}(X_i) = n\theta_i(1-\theta_i)$ | — |
| **Poisson** | Events in continuous interval $\lambda = \alpha t$ | $\frac{\lambda^x e^{-\lambda}}{x!}$ | $x = 0, 1, 2, \dots$ | $\lambda$ | $\lambda$ | $e^{\lambda(e^t-1)}$ |

*(Note: Course notes use $\theta$ for success probability. Often written as $p$ in standard literature).*

---

### 2.2 Key Properties & Course Theorems

#### 1. Discrete Uniform Distribution
* Sum of first $k$ integers: $\sum_{i=1}^k i = \frac{k(k+1)}{2} \implies \mu = \frac{k+1}{2}$.
* Sum of squares: $\sum_{i=1}^k i^2 = \frac{k(k+1)(2k+1)}{6} \implies \sigma^2 = \frac{k^2-1}{12}$.

#### 2. Binomial Distribution $b(x; n, \theta)$
* **Symmetry Theorem (Theorem 5.1)**:
  $$b(x; n, \theta) = b(n-x; n, 1-\theta)$$
  *Example*: $b(7; 10, 0.80) = b(3; 10, 0.20) = B(3; 10, 0.20) - B(2; 10, 0.20) = 0.8791 - 0.6778 = 0.2013$.

#### 3. Negative Binomial $b^*(x; k, \theta)$ & Geometric $g(x; \theta)$
* Logic: To have the $k$-th success on trial $x$, there must be exactly $(k-1)$ successes in the first $(x-1)$ trials, multiplied by $\theta$ on the $x$-th trial:
  $$P(X=x) = \binom{x-1}{k-1}\theta^{k-1}(1-\theta)^{x-k} \cdot \theta = \binom{x-1}{k-1}\theta^k(1-\theta)^{x-k}$$
* **Binomial Conversion Identity (Theorem 5.5)**:
  $$b^*(x; k, \theta) = \frac{k}{x} b(k; x, \theta)$$
* **Geometric Distribution**: Set $k=1 \implies g(x; \theta) = \theta(1-\theta)^{x-1}$.

#### 4. Hypergeometric Distribution $h(x; n, N, M)$
* $N$ = Population size, $M$ = Number of successes in population, $n$ = Sample size taken **without replacement**.
* Notice the **Finite Population Correction Factor** in variance: $\frac{N-n}{N-1}$.
* **Binomial Approximation**:
  * Valid when $n \le 0.05 N$ (sample size is $5\%$ or less of population).
  * Use Binomial with parameters $n$ and $\theta = \frac{M}{N}$.

#### 5. Multinomial Distribution
* Generalization of Binomial to trials with $k > 2$ possible outcomes:
  $$P(X_1=x_1, \dots, X_k=x_k) = \frac{n!}{x_1! x_2! \cdots x_k!} \theta_1^{x_1}\theta_2^{x_2}\cdots\theta_k^{x_k} \quad \left(\sum_{i=1}^k x_i = n, \, \sum_{i=1}^k \theta_i = 1\right)$$

#### 6. Poisson Distribution $p(x; \lambda)$
* Unique hallmark: $\mathbf{\mu = \sigma^2 = \lambda}$.
* **Poisson Process (Interval / Area Scaling)**:
  * If average rate is $\alpha$ per unit time/region, for interval/region of size $t$:
    $$\lambda = \alpha t \implies P(X=x) = \frac{(\alpha t)^x e^{-\alpha t}}{x!}$$
* **Poisson Approximation to Binomial**:
  * Valid when $n \ge 20$ and $\theta \le 0.05$ (limiting case as $n \to \infty, \theta \to 0$ with $n\theta = \lambda$ constant).
  * Excellent when $n \ge 100$ and $n\theta < 10$. Set $\mathbf{\lambda = n\theta}$.

---

# PART 3: TOP 4 MUST-KNOW PROOFS

### Proof 1: Continuous Chebyshev's Theorem
1. Express variance as an integral:
   $$\sigma^2 = E[(X-\mu)^2] = \int_{-\infty}^{\infty} (x-\mu)^2 f_X(x) \, dx$$
2. Split the integral into three parts:
   $$\sigma^2 = \int_{-\infty}^{\mu-k\sigma} (x-\mu)^2 f_X(x)dx + \int_{\mu-k\sigma}^{\mu+k\sigma} (x-\mu)^2 f_X(x)dx + \int_{\mu+k\sigma}^{\infty} (x-\mu)^2 f_X(x)dx$$
3. Since $(x-\mu)^2 f_X(x) \ge 0$, drop the middle interval:
   $$\sigma^2 \ge \int_{-\infty}^{\mu-k\sigma} (x-\mu)^2 f_X(x)dx + \int_{\mu+k\sigma}^{\infty} (x-\mu)^2 f_X(x)dx$$
4. In both remaining intervals, $|x-\mu| \ge k\sigma \implies (x-\mu)^2 \ge k^2\sigma^2$:
   $$\sigma^2 \ge k^2\sigma^2 \int_{-\infty}^{\mu-k\sigma} f_X(x)dx + k^2\sigma^2 \int_{\mu+k\sigma}^{\infty} f_X(x)dx$$
5. Divide by $k^2\sigma^2$:
   $$\frac{1}{k^2} \ge P(X \le \mu-k\sigma) + P(X \ge \mu+k\sigma) = P(|X-\mu| \ge k\sigma)$$
6. By the complement rule:
   $$P(|X - \mu| < k\sigma) = 1 - P(|X - \mu| \ge k\sigma) \ge 1 - \frac{1}{k^2} \quad \blacksquare$$

---

### Proof 2: Binomial MGF, Mean, and Variance
1. **Derive MGF**:
   $$M_X(t) = E[e^{tX}] = \sum_{x=0}^n e^{tx} \binom{n}{x}\theta^x(1-\theta)^{n-x} = \sum_{x=0}^n \binom{n}{x}(\theta e^t)^x (1-\theta)^{n-x}$$
   By the Binomial expansion:
   $$M_X(t) = [\theta e^t + (1-\theta)]^n = [1 + \theta(e^t - 1)]^n$$
2. **First Derivative ($E[X]$)**:
   $$M'_X(t) = n[1 + \theta(e^t - 1)]^{n-1} \cdot \theta e^t$$
   $$\mu = M'_X(0) = n[1 + 0]^{n-1}\theta(1) = n\theta$$
3. **Second Derivative ($E[X^2]$)**:
   $$M''_X(t) = n\theta e^t [1 + \theta(e^t - 1)]^{n-1} + n(n-1)\theta^2 e^{2t} [1 + \theta(e^t - 1)]^{n-2}$$
   $$\mu'_2 = M''_X(0) = n\theta + n(n-1)\theta^2$$
4. **Variance**:
   $$\sigma^2 = \mu'_2 - \mu^2 = n\theta + n^2\theta^2 - n\theta^2 - (n\theta)^2 = n\theta(1-\theta) \quad \blacksquare$$

---

### Proof 3: Poisson MGF, Mean, and Variance
1. **Derive MGF**:
   $$M_X(t) = \sum_{x=0}^\infty e^{tx} \frac{\lambda^x e^{-\lambda}}{x!} = e^{-\lambda} \sum_{x=0}^\infty \frac{(\lambda e^t)^x}{x!}$$
   Using Maclaurin series $\sum_{x=0}^\infty \frac{u^x}{x!} = e^u$:
   $$M_X(t) = e^{-\lambda} \cdot e^{\lambda e^t} = e^{\lambda(e^t - 1)}$$
2. **Mean & Variance via Derivatives**:
   * $M'_X(t) = \lambda e^t e^{\lambda(e^t-1)} \implies \mu = M'_X(0) = \lambda$
   * $M''_X(t) = \lambda e^t e^{\lambda(e^t-1)} + (\lambda e^t)^2 e^{\lambda(e^t-1)} \implies \mu'_2 = M''_X(0) = \lambda + \lambda^2$
   * $\sigma^2 = \mu'_2 - \mu^2 = (\lambda + \lambda^2) - \lambda^2 = \lambda \quad \blacksquare$

---

### Proof 4: Negative Binomial to Binomial Identity (Theorem 5.5)
$$b^*(x; k, \theta) = \binom{x-1}{k-1}\theta^k (1-\theta)^{x-k} = \frac{(x-1)!}{(k-1)!(x-k)!} \theta^k (1-\theta)^{x-k}$$
Multiply and divide by $\frac{x}{k}$:
$$= \frac{k}{x} \cdot \frac{x \cdot (x-1)!}{k \cdot (k-1)!(x-k)!}\theta^k(1-\theta)^{x-k} = \frac{k}{x} \frac{x!}{k!(x-k)!}\theta^k(1-\theta)^{x-k} = \frac{k}{x} b(k; x, \theta) \quad \blacksquare$$

---

# PART 4: WORD-PROBLEM RECOGNITION GUIDE

| Problem Phrase / Situation | Correct Distribution | Formula / Action |
| :--- | :--- | :--- |
| "At least $k$ standard deviations" / "Lower bound on probability" | **Chebyshev's Inequality** | $P(\|X-\mu\| < k\sigma) \ge 1 - \frac{1}{k^2}$ |
| $n$ independent trials, constant probability $\theta$, counting successes | **Binomial** | $P(X=x) = \binom{n}{x}\theta^x(1-\theta)^{n-x}$ |
| Counting trials until the $k$-th success ($k \ge 2$) | **Negative Binomial** | $P(X=x) = \binom{x-1}{k-1}\theta^k(1-\theta)^{x-k}$ |
| Counting trials until the very **first** success | **Geometric** | $P(X=x) = \theta(1-\theta)^{x-1}$ |
| Population $N$, $M$ successes, drawing $n$ **without replacement** | **Hypergeometric** | $P(X=x) = \frac{\binom{M}{x}\binom{N-M}{n-x}}{\binom{N}{n}}$ |
| Trials with $> 2$ possible categories (e.g., Channels A, B, C) | **Multinomial** | $P = \frac{n!}{x_1! \dots x_k!}\theta_1^{x_1} \dots \theta_k^{x_k}$ |
| Rare events per unit time / space (phone calls/hr, defects/sq ft) | **Poisson** | Compute $\lambda = \alpha t$, then $P(X=x) = \frac{\lambda^x e^{-\lambda}}{x!}$ |
| Binomial where $n \ge 20$ and $\theta \le 0.05$ | **Poisson Approximation** | Use Poisson with $\lambda = n\theta$ |
| Hypergeometric where $n \le 0.05 N$ | **Binomial Approximation** | Use Binomial with $\theta = M/N$ |
