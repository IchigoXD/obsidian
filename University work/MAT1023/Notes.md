# MAT 1023 / MT 105: Real Analysis I — Comprehensive End-Exam Study Guide

**Course:** MAT 1023 / MT 105 — Real Analysis I  
**Department:** Department of Mathematics, Faculty of Science, University of Peradeniya  
**Lecturer:** Dr. Rajitha Ranasinghe  
**Core Reference:** Terence Tao, *Analysis I* (3rd Edition) & Course Lecture Notes (Chapters 1–5)

---

## Table of Contents
1. [Exam Blueprint & High-Yield Topic Matrix](#1-exam-blueprint--high-yield-topic-matrix)
2. [Chapter 1: Logic, Quantifiers, and Proof Techniques](#2-chapter-1-logic-quantifiers-and-proof-techniques)
3. [Chapter 2: The Real Number System & Completeness](#3-chapter-2-the-real-number-system--completeness)
4. [Chapter 3: Sequences of Real Numbers](#4-chapter-3-sequences-of-real-numbers)
5. [Chapter 4: Limits of Functions & Continuity](#5-chapter-4-limits-of-functions--continuity)
6. [Chapter 5: Differentiation & Mean Value Theorems](#6-chapter-5-differentiation--mean-value-theorems)
7. [Standard Proof Protocols & Master Templates](#7-standard-proof-protocols--master-templates)
8. [Comprehensive Past Exam Solutions (End 22/23 & End 23/24)](#8-comprehensive-past-exam-solutions-end-2223--end-2324)
9. [Quick-Fire MCQ & True/False Revision Bank](#9-quick-fire-mcq--truefalse-revision-bank)

---

# 1. Exam Blueprint & High-Yield Topic Matrix

### Exam Format
* **Duration:** 3 Hours
* **Total Marks:** 400 Marks (scaled to 100%)
* **Structure:**
  * **Part A (60 Marks):** 10 Multiple Choice Questions (6 marks each) testing definitions, core implications, necessary vs. sufficient conditions, and boundary counterexamples.
  * **Part B (340 Marks):** 3–4 Long Structured Questions with rigorous step-by-step proofs, $\epsilon-\delta$ derivations, and induction arguments.

### High-Yield Exam Question Matrix
| Topic / Chapter | Recurring Exam Question Types | Past Exam Appearance |
| :--- | :--- | :--- |
| **Ch 2: Completeness & Bounds** | • $\sup(A+B)$ and $\sup(A-B)$ properties (True/False + Proofs/Counterexamples)<br>• Calculating $\sup, \inf, \max, \min$ using algebraic manipulation & AM-GM<br>• Archimedean Principle: proving existence of $n \in \mathbb{Z}^+$ such that $r < -1/n < 0$ or $1/n < \epsilon$ | End 22/23 Q1(a,b,c)<br>End 23/24 Part A Q1–Q4 |
| **Ch 3: Sequences & MCT** | • Statements and implications: $x_n \to \infty \implies 1/x_n \to 0$ vs. $x_n \to 0 \implies 1/x_n \to \infty$<br>• State Monotone Convergence Theorem (MCT)<br>• Recursive sequence analysis: $x_1 = \sqrt{c}, x_{n+1} = \sqrt{c + x_n}$. Induction for upper bound, Induction for increasing, finding $\lim x_n$<br>• Limits involving $(1 + 1/n^2)^{2n^2} \to e^2$ | End 22/23 Q2(a,b,c)<br>End 23/24 Part B Q1(b)<br>End 23/24 Part A Q5–Q7 |
| **Ch 4: Limits & $\epsilon-\delta$** | • Precise $\epsilon-\delta$ proofs for rational functions: $\lim_{x\to 1}\frac{2x^2-3x+1}{x-1} = 1$, $\lim_{x\to -6}\frac{x+4}{2-x} = -\frac{1}{4}$<br>• Dirichlet Function: nowhere continuous (proof via density)<br>• Thomae's Function: discontinuous on $\mathbb{Q}$, continuous on $\mathbb{R}\setminus\mathbb{Q}$<br>• Cauchy Functional Equation: $f(x+y) = f(x)+f(y)$ ($f(nx)=nf(x), f(qx)=qf(x)$, continuity at 0 $\iff$ continuous everywhere) | End 22/23 Q3(a,c)<br>End 23/24 Part B Q1(a), Q2(a,b) |
| **Ch 4: EVT & IVT** | • State EVT; provide counterexamples when domain is not closed or not bounded<br>• State IVT; prove existence of roots (e.g., $e^x = 1 + 2\cos x$, $f(x_0)=g(x_0)$) | End 22/23 Q3(b,d)<br>End 23/24 Part B Q2(c) |
| **Ch 5: Derivatives & MVT** | • Differentiability limit manipulation: $\lim_{x\to 0}\frac{1}{x}\sum_{j=1}^k f(x/j) = \sum \frac{1}{j} f'(0)$<br>• Pathological example: $f(x) = x^2\sin(1/x)$ differentiable at 0 ($f'(0)=0$), but $f'$ discontinuous at 0<br>• State Rolle's Theorem & MVT with geometric interpretations<br>• Prove MVT from Rolle's Theorem using auxiliary function $h(x)$<br>• Check Rolle's / MVT conditions on intervals (check continuity on $[a, b]$, differentiability on $(a, b)$)<br>• MVT applications to inequalities ($1+x < e^x$) and sign changes ($f''(c) > 0$) | End 22/23 Q4(a,b,c,d)<br>End 23/24 Part B Q3(a,b) |

---

# 2. Chapter 1: Logic, Quantifiers, and Proof Techniques

### 1.1 Statements & Logical Connectives
* **Statement (Proposition):** A declarative sentence that is either **True** or **False**, but not both.
  * *Open sentence / Predicate:* $p(x): x^2 - 4x + 4 = 0$ is not a statement until $x$ is specified or quantified.
* **Truth Tables & Logical Operators:**
  * **Conjunction ($p \wedge q$):** True only when both $p$ and $q$ are True.
  * **Disjunction ($p \vee q$):** False only when both $p$ and $q$ are False.
  * **Implication (Conditional, $p \implies q$):** False **only** when antecedent $p$ is True and consequent $q$ is False. If $p$ is False, $p \implies q$ is **vacuously True**.
    * *Terminology:* "$p$ is sufficient for $q$", "$q$ is necessary for $p$", "$p$ only if $q$", "$q$ whenever $p$", "$q$ provided that $p$".
  * **Biconditional ($p \iff q$):** True when $p$ and $q$ have identical truth values.

### 1.2 Converse, Inverse, and Contrapositive
Given the conditional statement $p \implies q$:
1. **Converse:** $q \implies p$ *(NOT logically equivalent to $p \implies q$! Confusing them is the Fallacy of the Converse).*
2. **Inverse:** $\neg p \implies \neg q$ *(Logically equivalent to the converse).*
3. **Contrapositive:** $\neg q \implies \neg p$ *(Logically equivalent to the original statement: $(p \implies q) \equiv (\neg q \implies \neg p)$).*
4. **Negation of an Implication:**
   $$\neg(p \implies q) \equiv p \wedge \neg q$$
   *(Crucial: The negation of an "if-then" is NOT another "if-then"; it is an "AND" statement!)*

### 1.3 Quantifiers and Order
* **Universal Quantifier ($\forall$):** "For all", "for every", "for each".
* **Existential Quantifier ($\exists$):** "There exists at least one", "for some".
* **Such that ($\ni$ or $:$, s.t.):** Separates quantifier from condition.
* **Negation Rules (De Morgan for Quantifiers):**
  $$\neg[\forall x \in S, P(x)] \equiv \exists x \in S \text{ s.t. } \neg P(x)$$
  $$\neg[\exists x \in S \text{ s.t. } P(x)] \equiv \forall x \in S, \neg P(x)$$
* **Order of Quantifiers Matters:**
  $$\exists y \ \forall x, P(x, y) \implies \forall x \ \exists y, P(x, y) \quad (\text{Strictly stronger, converse is FALSE!})$$
  * *Example:* $\forall x \in \mathbb{R}, \exists y \in \mathbb{R} \text{ s.t. } y = x^2$ is **True** (every number has a square).  
    $\exists y \in \mathbb{R} \text{ s.t. } \forall x \in \mathbb{R}, y = x^2$ is **False** (there is no single universal square).

### 1.4 Proof Techniques
1. **Direct Proof:** Assume $p$ is true; through definitions, axioms, and established theorems, deduce $q$.
2. **Contrapositive Proof:** To prove $p \implies q$, assume $\neg q$ is true and deduce $\neg p$. Highly effective when $q$ contains negatives or non-divisibility.
   * *Example:* Prove if $n^2$ is even, then $n$ is even. (Assume $n$ is odd: $n = 2k+1 \implies n^2 = 4k^2+4k+1 = 2(2k^2+2k)+1$, which is odd. Hence by contrapositive, if $n^2$ is even, $n$ is even.)
3. **Proof by Contradiction (Reductio ad Absurdum):** To prove $p \implies q$, assume $p \wedge \neg q$. Deduce a logical contradiction ($c$, e.g., $0=1$ or $r \wedge \neg r$).
4. **Counterexamples:** A universal statement $\forall x, P(x)$ is disproved by providing a single concrete element $x_0$ for which $P(x_0)$ is false.

---

# 3. Chapter 2: The Real Number System & Completeness

### 2.1 The Axiomatic Foundations of $\mathbb{R}$
The real number system $(\mathbb{R}, +, \cdot, <)$ is a **complete ordered field**.

#### Axiom Set 1: Field Axioms
For all $a, b, c \in \mathbb{R}$:
1. **Closure:** $a+b \in \mathbb{R}$ and $a \cdot b \in \mathbb{R}$.
2. **Associativity:** $a + (b + c) = (a + b) + c$ and $a \cdot (b \cdot c) = (a \cdot b) \cdot c$.
3. **Commutativity:** $a + b = b + a$ and $a \cdot b = b \cdot a$.
4. **Distributivity:** $a \cdot (b + c) = a \cdot b + a \cdot c$.
5. **Additive Identity:** Unique element $0 \in \mathbb{R}$ such that $0 + a = a$.
6. **Multiplicative Identity:** Unique element $1 \in \mathbb{R}$ ($1 \neq 0$) such that $1 \cdot a = a$.
7. **Additive Inverse:** For each $x \in \mathbb{R}$, unique $-x \in \mathbb{R}$ such that $x + (-x) = 0$.
8. **Multiplicative Inverse:** For each $x \in \mathbb{R} \setminus \{0\}$, unique $x^{-1} = \frac{1}{x} \in \mathbb{R}$ such that $x \cdot x^{-1} = 1$.

*Key Algebraic Deduction (Mid 23/24 Q3):*
> **Theorem:** Prove $(-a) \cdot (-b) = a \cdot b$.  
> **Proof:**  
> First note that $0 \cdot x = 0$ since $0 \cdot x = (0+0)\cdot x = 0\cdot x + 0\cdot x \implies 0\cdot x = 0$.  
> Then $a + (-1)a = 1\cdot a + (-1)\cdot a = (1 + (-1))a = 0\cdot a = 0 \implies -a = (-1)a$.  
> Thus $(-a)\cdot (-b) = [(-1)a][(-1)b] = [(-1)(-1)](ab)$.  
> Since $(-1) + 1 = 0 \implies (-1)(-1) + (-1)\cdot 1 = 0 \implies (-1)(-1) + (-1) = 0 \implies (-1)(-1) = 1$.  
> Therefore, $(-a)\cdot (-b) = 1 \cdot (ab) = ab$. $\blacksquare$

#### Axiom Set 2: Order Axioms
There exists a relation $<$ on $\mathbb{R}$ satisfying:
1. **Trichotomy:** For any $a, b \in \mathbb{R}$, exactly one holds: $a < b$, $b < a$, or $a = b$.
2. **Transitivity:** $a < b$ and $b < c \implies a < c$.
3. **Additive Property:** $a < b \implies a + c < b + c$ for all $c \in \mathbb{R}$.
4. **Multiplicative Properties:**
   * $a < b$ and $c > 0 \implies ac < bc$.
   * $a < b$ and $c < 0 \implies bc < ac$.

*Key Order Deduction (Mid 23/24 Q4):*
> **Theorem:** If $0 < x < y$, prove $0 < \frac{1}{y} < \frac{1}{x}$.  
> **Proof:**  
> 1. Since $x > 0$, if $\frac{1}{x} \le 0$, then by multiplying by $x > 0$, $1 \le 0$, contradiction. Thus $\frac{1}{x} > 0$. Similarly $\frac{1}{y} > 0$.  
> 2. Since $\frac{1}{x} > 0$ and $\frac{1}{y} > 0$, their product $\frac{1}{xy} > 0$.  
> 3. Multiply the inequality $x < y$ by the positive element $\frac{1}{xy}$:  
>    $$x \cdot \frac{1}{xy} < y \cdot \frac{1}{xy} \implies \frac{1}{y} < \frac{1}{x}.$$  
> Combined with $\frac{1}{y} > 0$, we get $0 < \frac{1}{y} < \frac{1}{x}$. $\blacksquare$

### 2.2 Absolute Values and Neighborhoods
* **Definition:** $|x| = \begin{cases} x & \text{if } x \ge 0 \\ -x & \text{if } x < 0 \end{cases}$
* **Fundamental Theorem:** $|a| \le M \iff -M \le a \le M$.
* **Triangle Inequality:** $|a + b| \le |a| + |b|$ for all $a, b \in \mathbb{R}$.
* **Reverse Triangle Inequality:** $||a| - |b|| \le |a - b|$.
* **$\epsilon$-Neighborhood:** $V_\epsilon(a) = \{x \in \mathbb{R} : |x - a| < \epsilon\} = (a - \epsilon, a + \epsilon)$.
* **Zero Lemma:** If $a \in \mathbb{R}$ satisfies $0 \le a < \epsilon$ for every $\epsilon > 0$, then $a = 0$.

### 2.3 The Completeness Axiom & Bounds
* **Upper Bound / Lower Bound:**
  * $M$ is an upper bound of $E \subseteq \mathbb{R}$ if $x \le M$ for all $x \in E$.
  * $m$ is a lower bound of $E$ if $x \ge m$ for all $x \in E$.
* **Supremum (Least Upper Bound, $\sup E$):**
  $s = \sup E$ iff:
  1. $s$ is an upper bound of $E$ ($\forall x \in E, x \le s$).
  2. If $M$ is any upper bound of $E$, then $s \le M$.
* **Infimum (Greatest Lower Bound, $\inf E$):**
  $t = \inf E$ iff:
  1. $t$ is a lower bound of $E$ ($\forall x \in E, x \ge t$).
  2. If $m$ is any lower bound of $E$, then $m \le t$.
* **Maximum / Minimum:**
  * $\max E = \sup E$ iff $\sup E \in E$.
  * $\min E = \inf E$ iff $\inf E \in E$.

#### The Completeness Axiom (Least Upper Bound Property)
> **Every nonempty subset of $\mathbb{R}$ that is bounded above has a finite supremum in $\mathbb{R}$.**  
> *(Equivalent: Every nonempty subset of $\mathbb{R}$ bounded below has a finite infimum: $\inf E = -\sup(-E)$).*

#### Approximation Property for Suprema & Infima
* **Supremum:** $s = \sup E \iff s$ is an upper bound and $\forall \epsilon > 0, \exists a \in E \text{ s.t. } s - \epsilon < a \le s$.
* **Infimum:** $t = \inf E \iff t$ is a lower bound and $\forall \epsilon > 0, \exists a \in E \text{ s.t. } t \le a < t + \epsilon$.

#### Integer Supremum Theorem (End 23/24 Part A Q2)
> If $E \subset \mathbb{Z}$ is nonempty and bounded above, then $\sup E \in E$ (and hence $\sup E$ is an integer).

#### Archimedean Principle & Density Theorems
1. **Archimedean Principle (End 23/24 Part A Q3):**  
   For any $a > 0$ and any $b \in \mathbb{R}$, there exists $n \in \mathbb{Z}^+$ such that $na > b$.
   * *Consequence:* For every $\epsilon > 0$, there exists $n \in \mathbb{Z}^+$ such that $\frac{1}{n} < \epsilon$.
   * *Past Exam Problem (End 22/23 Q1(c)):* Let $r < 0$. Prove $\exists n \in \mathbb{Z}^+$ s.t. $r < -\frac{1}{n} < 0$.  
     *Proof:* Since $r < 0$, $-r > 0$. By the Archimedean Principle consequence with $\epsilon = -r > 0$, there exists $n \in \mathbb{Z}^+$ such that $\frac{1}{n} < -r$. Multiplying by $-1$ flips the inequality: $-\frac{1}{n} > r$. Since $n \in \mathbb{Z}^+$, $-\frac{1}{n} < 0$. Hence $r < -\frac{1}{n} < 0$. $\blacksquare$
2. **Density of $\mathbb{Q}$ in $\mathbb{R}$:** Between any two real numbers $a < b$, there exists a rational $q \in \mathbb{Q}$ such that $a < q < b$.
3. **Density of $\mathbb{R} \setminus \mathbb{Q}$ in $\mathbb{R}$:** Between any two real numbers $a < b$, there exists an irrational number $r \in \mathbb{R} \setminus \mathbb{Q}$ such that $a < r < b$.

### 2.4 Bounds under Set Operations (End 22/23 Exam Focus)
Let $A, B \subset \mathbb{R}$ be nonempty bounded sets:
1. **Sum of Sets:** $A + B := \{a + b : a \in A, b \in B\}$.
   $$\sup(A + B) = \sup A + \sup B \quad \text{and} \quad \inf(A + B) = \inf A + \inf B$$
   *Proof:* For any $a \in A, b \in B$, $a \le \sup A$ and $b \le \sup B \implies a + b \le \sup A + \sup B$. Thus $\sup A + \sup B$ is an upper bound, so $\sup(A+B) \le \sup A + \sup B$.  
   For any $\epsilon > 0$, by Approximation Property, $\exists a \in A$ with $a > \sup A - \epsilon/2$ and $\exists b \in B$ with $b > \sup B - \epsilon/2$. Then $a + b > \sup A + \sup B - \epsilon$. Thus $\sup(A+B) \ge a+b > \sup A + \sup B - \epsilon$. Letting $\epsilon \to 0$ gives $\sup(A+B) \ge \sup A + \sup B$. Hence equality holds. $\blacksquare$
2. **Difference of Sets:** $A - B := \{a - b : a \in A, b \in B\}$.
   $$\sup(A - B) = \sup A - \inf B \quad (\mathbf{NOT} \ \sup A - \sup B!)$$
   *Counterexample for $\sup(A - B) = \sup A - \sup B$ (End 22/23 Q1(a)(ii)):*  
   Let $A = [0, 1]$ and $B = [0, 1]$.  
   $\sup A = 1$, $\sup B = 1 \implies \sup A - \sup B = 1 - 1 = 0$.  
   However, $A - B = [0-1, 1-0] = [-1, 1]$, so $\sup(A - B) = 1 \neq 0$. The statement is **False**!
3. **Product by Scalar:**
   * If $k \ge 0$: $\sup(kA) = k \sup A$, $\inf(kA) = k \inf A$.
   * If $k < 0$: $\sup(kA) = k \inf A$, $\inf(kA) = k \sup A$.

---

# 4. Chapter 3: Sequences of Real Numbers

### 3.1 Definition of Limit ($\epsilon-N$)
* A sequence $\{x_n\}$ converges to $L \in \mathbb{R}$ (written $\lim_{n\to\infty} x_n = L$ or $x_n \to L$) iff:
  $$\forall \epsilon > 0, \ \exists N \in \mathbb{Z}^+ \text{ such that } n \ge N \implies |x_n - L| < \epsilon$$
* **Fundamental Theorems:**
  1. The limit of a convergent sequence is **unique**.
  2. Every convergent sequence is **bounded**. *(Converse is false: $\{(-1)^n\}$ is bounded but diverges).*
  3. If $x_n \to L$, then every subsequence $\{x_{n_k}\}$ converges to the same limit $L$. *(Contrapositive: If two subsequences converge to different limits, the sequence diverges).*
  4. If $x_n \to 0$ and $\{y_n\}$ is bounded, then $x_n y_n \to 0$.

### 3.2 Limit Theorems & Squeeze Theorem
* **Squeeze Theorem:** If $x_n \le y_n \le z_n$ for all $n \ge N_0$, and $\lim x_n = \lim z_n = L$, then $\lim y_n = L$.
* **Algebra of Limits:** If $x_n \to x$ and $y_n \to y$, then $x_n \pm y_n \to x \pm y$, $c x_n \to c x$, $x_n y_n \to x y$, and $x_n/y_n \to x/y$ (provided $y \neq 0$).
* **Order Preservation (Comparison Theorem):**
  If $x_n \le y_n$ for $n \ge N_0$, then $\lim x_n \le \lim y_n$.  
  *(Warning: Strict inequality $x_n < y_n$ does NOT imply strict limit inequality! Example: $0 < 1/n$, but $\lim 0 = \lim 1/n = 0$).*

### 3.3 The Monotone Convergence Theorem (MCT)
> **Theorem (MCT):**  
> A monotone sequence of real numbers converges if and only if it is bounded:
> 1. If $\{x_n\}$ is **increasing** and **bounded above**, then $\lim_{n\to\infty} x_n = \sup\{x_n : n \in \mathbb{Z}^+\}$.
> 2. If $\{x_n\}$ is **decreasing** and **bounded below**, then $\lim_{n\to\infty} x_n = \inf\{x_n : n \in \mathbb{Z}^+\}$.

### 3.4 Bounded Recursive Sequences (Exam Blueprint Template)
Every recent end-exam features a recursive sequence of the form:
$$x_1 = \sqrt{c}, \quad x_{n+1} = \sqrt{c + x_n} \quad (c = 3 \text{ in 22/23}, c = 5 \text{ in 23/24})$$
**Standard 3-Step Solution Template:**
1. **Step 1: Prove bounded above by $M$ (by Induction on $n$)**
   * *Base Step:* $x_1 = \sqrt{c} < c$ (since $c > 1$). True.
   * *Inductive Hypothesis:* Assume $x_k \le c$ for some $k \ge 1$.
   * *Inductive Step:* $x_{k+1} = \sqrt{c + x_k} \le \sqrt{c + c} = \sqrt{2c}$. Since $2c \le c^2$ (for $c \ge 2$), $\sqrt{2c} \le c$. Thus $x_{k+1} \le c$.  
   By PMI, $x_n \le c$ for all $n \in \mathbb{Z}^+$.
2. **Step 2: Prove increasing (by Induction on $n$)**
   * *Base Step:* $x_2 = \sqrt{c + \sqrt{c}} > \sqrt{c} = x_1$. True for $n=1$.
   * *Inductive Hypothesis:* Assume $x_k > x_{k-1}$ for some $k \ge 2$.
   * *Inductive Step:* $x_{k+1} = \sqrt{c + x_k} > \sqrt{c + x_{k-1}} = x_k$ (since square root is strictly increasing).  
   By PMI, $x_{n+1} > x_n$ for all $n \ge 1$.
3. **Step 3: Compute the limit**
   * By MCT, since $\{x_n\}$ is increasing and bounded above, $L = \lim_{n\to\infty} x_n$ exists.
   * Take limits on both sides of $x_{n+1}^2 = c + x_n$:
     $$L^2 = c + L \implies L^2 - L - c = 0 \implies L = \frac{1 \pm \sqrt{1 + 4c}}{2}$$
   * Since $x_n \ge \sqrt{c} > 0$, $L > 0$. Thus:
     $$L = \frac{1 + \sqrt{1 + 4c}}{2}$$
     *(For $c=3$: $L = \frac{1 + \sqrt{13}}{2}$. For $c=5$: $L = \frac{1 + \sqrt{21}}{2}$).*

### 3.5 Bolzano-Weierstrass Theorem & Cauchy Sequences
* **Bolzano-Weierstrass Theorem:** Every bounded sequence in $\mathbb{R}$ contains a convergent subsequence.
* **Cauchy Sequence:** $\{x_n\}$ is Cauchy iff $\forall \epsilon > 0, \exists N \in \mathbb{Z}^+$ such that $m, n \ge N \implies |x_n - x_m| < \epsilon$.
* **Completeness of $\mathbb{R}$:** In $\mathbb{R}$, a sequence converges if and only if it is a Cauchy sequence.

---

# 5. Chapter 4: Limits of Functions & Continuity

### 5.1 Two-Sided Limit Definition ($\epsilon-\delta$)
* Let $f: I \setminus \{a\} \to \mathbb{R}$. We say $\lim_{x\to a} f(x) = L$ iff:
  $$\forall \epsilon > 0, \ \exists \delta > 0 \text{ such that } 0 < |x - a| < \delta \implies |f(x) - L| < \epsilon$$
* **Sequential Characterization of Limits:**  
  $\lim_{x\to a} f(x) = L \iff$ for every sequence $(x_n)$ in the domain with $x_n \neq a$ and $x_n \to a$, we have $f(x_n) \to L$.
  * *Disproving limits:* Find two sequences $x_n \to a, y_n \to a$ such that $\lim f(x_n) \neq \lim f(y_n)$.

### 5.2 The 5-Step $\epsilon-\delta$ Proof Protocol (Rational Functions)
*Example from End 23/24 Q2(a):* Prove $\lim_{x\to -6} \frac{x+4}{2-x} = -\frac{1}{4}$.
1. **Write the target error expression:**
   $$\left| \frac{x+4}{2-x} - \left(-\frac{1}{4}\right) \right| = \left| \frac{4(x+4) + (2-x)}{4(2-x)} \right| = \left| \frac{3x + 18}{4(2-x)} \right| = \frac{3|x + 6|}{4|x - 2|}$$
2. **Restrict $\delta \le 1$ to bound the denominator:**
   Assume $|x - (-6)| = |x + 6| < 1$.  
   Then $-1 < x + 6 < 1 \implies -7 < x < -5$.
3. **Bound the term $|x - 2|$ from below:**
   For $-7 < x < -5$, subtract $2$:
   $$-9 < x - 2 < -7 \implies 7 < |x - 2| < 9 \implies \frac{1}{|x - 2|} < \frac{1}{7}$$
4. **Assemble the overall inequality:**
   $$\frac{3|x + 6|}{4|x - 2|} < \frac{3}{4} \cdot \frac{1}{7} |x + 6| = \frac{3}{28} |x + 6| < \epsilon \iff |x + 6| < \frac{28}{3}\epsilon$$
5. **Formal choice of $\delta$:**
   Given $\epsilon > 0$, choose $\delta = \min\left\{1, \frac{28}{3}\epsilon\right\}$.  
   Then whenever $0 < |x - (-6)| < \delta$, we have $|x + 6| < 1$ (so $\frac{1}{|x-2|} < \frac{1}{7}$) and $|x + 6| < \frac{28}{3}\epsilon$.  
   Therefore:
   $$\left| \frac{x+4}{2-x} - \left(-\frac{1}{4}\right) \right| = \frac{3|x+6|}{4|x-2|} < \frac{3}{28} \left(\frac{28}{3}\epsilon\right) = \epsilon. \quad \blacksquare$$

### 5.3 Continuity Definitions
* $f$ is continuous at $a \in \text{Dom}(f)$ iff $\lim_{x\to a} f(x) = f(a)$.
  $$\forall \epsilon > 0, \exists \delta > 0 \text{ s.t. } |x - a| < \delta \text{ and } x \in \text{Dom}(f) \implies |f(x) - f(a)| < \epsilon$$
* **Sequential Criterion for Continuity:** $f$ is continuous at $a \iff$ for every sequence $x_n \to a$, $f(x_n) \to f(a)$.

### 5.4 Benchmark Pathological Functions
#### 1. The Dirichlet Function
$$f(x) = \begin{cases} 1 & x \in \mathbb{Q} \\ 0 & x \in \mathbb{R} \setminus \mathbb{Q} \end{cases}$$
* **Theorem:** $f$ is nowhere continuous on $\mathbb{R}$.
* **Proof (Sequential):** Let $c \in \mathbb{R}$.
  * By density of $\mathbb{Q}$, there exists a sequence of rationals $r_n \to c$. Then $f(r_n) = 1 \to 1$.
  * By density of $\mathbb{R}\setminus\mathbb{Q}$, there exists a sequence of irrationals $s_n \to c$. Then $f(s_n) = 0 \to 0$.
  * If $f$ were continuous at $c$, then $\lim f(r_n) = \lim f(s_n) = f(c)$, implying $1 = 0$, a contradiction. Thus $f$ is discontinuous at every point of $\mathbb{R}$. $\blacksquare$

#### 2. Thomae’s (Ruler / Popcorn) Function
$$f(x) = \begin{cases} \frac{1}{q} & x = \frac{p}{q} \in \mathbb{Q} \cap (0, 1) \text{ in lowest terms } (q > 0) \\ 0 & x \in (0, 1) \setminus \mathbb{Q} \end{cases}$$
* **Theorem:** $f$ is **discontinuous** at every rational in $(0, 1)$ and **continuous** at every irrational in $(0, 1)$.
* **Proof:**
  1. *Discontinuity at rationals:* Let $a \in \mathbb{Q} \cap (0, 1)$. Then $f(a) = 1/q > 0$. Choose a sequence of irrationals $x_n \to a$. Then $f(x_n) = 0 \to 0 \neq f(a)$. Thus $f$ is discontinuous at $a$.
  2. *Continuity at irrationals:* Let $a \in (0, 1) \setminus \mathbb{Q}$, so $f(a) = 0$. Given $\epsilon > 0$, choose $M \in \mathbb{Z}^+$ such that $1/M < \epsilon$. The set of fractions $p/q \in (0, 1)$ in lowest terms with $q \le M$ is finite. Let $\delta = \min\{|a - p/q| : q \le M\} > 0$. Then for all $x \in (0, 1)$ with $|x - a| < \delta$:
     * If $x$ is irrational, $|f(x) - f(a)| = |0 - 0| = 0 < \epsilon$.
     * If $x = p/q$ is rational, its denominator must satisfy $q > M$, so $|f(x) - f(a)| = 1/q < 1/M < \epsilon$.  
     Hence $f$ is continuous at $a$. $\blacksquare$

### 5.5 Cauchy Functional Equation (End 23/24 Q1(a))
Suppose $f: \mathbb{R} \to \mathbb{R}$ satisfies $f(x + y) = f(x) + f(y)$ for all $x, y \in \mathbb{R}$.
1. **$f(nx) = nf(x)$ for all $n \in \mathbb{Z}$:**
   * *For $n \in \mathbb{Z}^+$:* Base $n=1$: $f(1\cdot x) = 1\cdot f(x)$. Induction: $f((k+1)x) = f(kx + x) = f(kx) + f(x) = kf(x) + f(x) = (k+1)f(x)$.
   * *For $n = 0$:* $f(0) = f(0+0) = f(0) + f(0) \implies f(0) = 0 = 0 \cdot f(x)$.
   * *For $n < 0$:* Let $n = -m$ ($m > 0$). Then $0 = f(0) = f(mx + (-mx)) = f(mx) + f(-mx) = mf(x) + f(nx) \implies f(nx) = -mf(x) = nf(x)$.
2. **$f(qx) = qf(x)$ for all $q \in \mathbb{Q}$:**
   * Let $q = m/n$ with $m \in \mathbb{Z}, n \in \mathbb{Z}^+$.
   * Then $f(mx) = f(n \cdot (m/n)x) = n f((m/n)x)$.
   * But $f(mx) = m f(x)$.
   * Equating: $n f(qx) = m f(x) \implies f(qx) = \frac{m}{n} f(x) = q f(x)$.
3. **Continuity at $0 \iff$ Continuity on $\mathbb{R}$:**
   * $(\Leftarrow)$ Trivial (continuity on $\mathbb{R}$ implies continuity at $0$).
   * $(\Rightarrow)$ Assume $f$ is continuous at $0$, so $\lim_{h\to 0} f(h) = f(0) = 0$.  
     Let $x_0 \in \mathbb{R}$. Then for any $x$:
     $$f(x) - f(x_0) = f(x - x_0)$$
     Taking the limit as $x \to x_0$ (let $h = x - x_0 \to 0$):
     $$\lim_{x\to x_0} f(x) = \lim_{h\to 0} [f(x_0) + f(h)] = f(x_0) + 0 = f(x_0)$$
     Thus $f$ is continuous at every $x_0 \in \mathbb{R}$. $\blacksquare$

### 5.6 Core Global Theorems on Intervals
#### Intermediate Value Theorem (IVT)
> **Theorem:** If $f: [a, b] \to \mathbb{R}$ is continuous and $y_0$ lies between $f(a)$ and $f(b)$, then there exists $x_0 \in (a, b)$ such that $f(x_0) = y_0$.
* **Standard Proof Outline (via Completeness):**
  Assume $f(a) < y_0 < f(b)$. Define $E = \{x \in [a, b] : f(x) < y_0\}$. $E \neq \emptyset$ (since $a \in E$) and $E$ is bounded above by $b$. By Completeness Axiom, $x_0 = \sup E$ exists. Using continuity of $f$ and sequence convergence, prove $f(x_0) \le y_0$ and $f(x_0) \ge y_0 \implies f(x_0) = y_0$.
* **Application 1: Root Finding ($e^x = 1 + 2\cos x$ on End 23/24 Q2(c)):**  
  Define $h(x) = e^x - 1 - 2\cos x$. $h$ is continuous on $\mathbb{R}$.  
  $h(0) = 1 - 1 - 2 = -2 < 0$.  
  $h(\pi) = e^\pi - 1 - 2(-1) = e^\pi + 1 > 0$.  
  By IVT on $[0, \pi]$, there exists $c \in (0, \pi)$ such that $h(c) = 0 \iff e^c = 1 + 2\cos c$.
* **Application 2: Intersection of Functions ($f(x_0) = g(x_0)$ on End 22/23 Q3(d)):**  
  Define $h(x) = f(x) - g(x)$. $h$ is continuous on $[a, b]$.  
  $h(a) = f(a) - g(a) < 0$ and $h(b) = f(b) - g(b) > 0$.  
  By IVT, $\exists x_0 \in (a, b)$ such that $h(x_0) = 0 \iff f(x_0) = g(x_0)$.

#### Extreme Value Theorem (EVT)
> **Theorem:** If $f: [a, b] \to \mathbb{R}$ is continuous on a **closed and bounded** interval, then $f$ is bounded on $[a, b]$ and attains its maximum and minimum values:
> $$\exists x_m, x_M \in [a, b] \text{ such that } f(x_m) = \inf_{x\in [a, b]} f(x) \quad \text{and} \quad f(x_M) = \sup_{x\in [a, b]} f(x)$$
* **Counterexamples when hypotheses fail (End 22/23 Q3(b)):**
  1. *Interval is NOT closed:* $f(x) = \frac{1}{x}$ on $(0, 1]$ (unbounded, no max); or $f(x) = x$ on $(0, 1)$ (bounded, but $\sup f = 1$ and $\inf f = 0$ are not attained in $(0, 1)$).
  2. *Interval is NOT bounded:* $f(x) = x$ on $[0, \infty)$ (unbounded); or $f(x) = \frac{x}{1+x}$ on $[0, \infty)$ (bounded with $\sup f = 1$, but $f(x) < 1$ for all $x$, so maximum is never attained).

---

# 6. Chapter 5: Differentiation & Mean Value Theorems

### 6.1 Definition & Properties of Derivatives
* **Derivative:** $f'(a) = \lim_{h\to 0} \frac{f(a+h) - f(a)}{h} = \lim_{x\to a} \frac{f(x) - f(a)}{x - a}$.
* **Theorem: Differentiability $\implies$ Continuity.**  
  *Proof:* $\lim_{x\to a} [f(x) - f(a)] = \lim_{x\to a} \left[ \frac{f(x) - f(a)}{x - a} \cdot (x - a) \right] = f'(a) \cdot 0 = 0 \implies \lim_{x\to a} f(x) = f(a)$.  
  *(Converse is false: $f(x) = |x|$ is continuous at $0$ but not differentiable at $0$).*

### 6.2 Pathological Example: $f(x) = x^2 \sin(1/x)$ (End 23/24 Q3(a))
Consider $f(x) = \begin{cases} x^2 \sin\left(\frac{1}{x}\right) & x \neq 0 \\ 0 & x = 0 \end{cases}$
1. **Differentiability at $0$:**
   $$f'(0) = \lim_{h\to 0} \frac{f(h) - f(0)}{h} = \lim_{h\to 0} \frac{h^2 \sin(1/h) - 0}{h} = \lim_{h\to 0} h \sin\left(\frac{1}{h}\right)$$
   Since $|\sin(1/h)| \le 1$, $-|h| \le h \sin(1/h) \le |h|$. By Squeeze Theorem, $f'(0) = 0$.
2. **Derivative for $x \neq 0$:**
   By Product and Chain rules:
   $$f'(x) = 2x \sin\left(\frac{1}{x}\right) - \cos\left(\frac{1}{x}\right)$$
3. **Discontinuity of $f'$ at $0$ (Sequential Criterion):**
   Choose the sequence $x_n = \frac{1}{2n\pi} \to 0$ as $n \to \infty$.  
   $$f'(x_n) = 2\left(\frac{1}{2n\pi}\right)\sin(2n\pi) - \cos(2n\pi) = 0 - 1 = -1 \to -1 \neq f'(0) = 0$$
   Thus $\lim_{x\to 0} f'(x)$ does not exist, so $f'$ is **not continuous at $0$**.  
   *Conclusion:* $f$ is not continuously differentiable ($\mathcal{C}^1$) on any interval containing $0$.

### 6.3 Rolle's Theorem
> **Theorem:** If $f$ is continuous on $[a, b]$, differentiable on $(a, b)$, and $f(a) = f(b)$, then there exists at least one $c \in (a, b)$ such that $f'(c) = 0$.
* **Proof:** By EVT, $f$ attains maximum $M$ and minimum $m$ on $[a, b]$.
  * If $M = m$, $f$ is constant, so $f'(x) = 0$ for all $x \in (a, b)$.
  * If $M \neq m$, since $f(a) = f(b)$, at least one of $M$ or $m$ is attained at an interior point $c \in (a, b)$.
  * If maximum at $c$: for $h > 0$, $\frac{f(c+h)-f(c)}{h} \le 0 \implies f'(c) \le 0$. For $h < 0$, $\frac{f(c+h)-f(c)}{h} \ge 0 \implies f'(c) \ge 0$.  
    Hence $f'(c) = 0$. $\blacksquare$

### 6.4 The Mean Value Theorem (Lagrange MVT)
> **Theorem:** If $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists $c \in (a, b)$ such that:
> $$f(b) - f(a) = f'(c)(b - a) \iff f'(c) = \frac{f(b) - f(a)}{b - a}$$

* **Geometric Interpretation:** The slope of the secant line between $(a, f(a))$ and $(b, f(b))$ equals the slope of the tangent line at $(c, f(c))$. There is at least one point where the tangent is parallel to the chord.
* **Proof of MVT using Rolle's Theorem (Standard Exam Question):**
  1. Define the auxiliary function $h: [a, b] \to \mathbb{R}$ by:
     $$h(x) = f(x) - f(a) - \frac{f(b) - f(a)}{b - a}(x - a)$$
  2. Check Rolle's conditions:
     * $h$ is continuous on $[a, b]$ (linear combination of continuous functions).
     * $h$ is differentiable on $(a, b)$ with $h'(x) = f'(x) - \frac{f(b) - f(a)}{b - a}$.
     * $h(a) = f(a) - f(a) - 0 = 0$.
     * $h(b) = f(b) - f(a) - \frac{f(b) - f(a)}{b - a}(b - a) = 0$.
     * Since $h(a) = h(b) = 0$, by Rolle's Theorem there exists $c \in (a, b)$ such that $h'(c) = 0$.
  3. Conclusion:
     $$h'(c) = 0 \implies f'(c) - \frac{f(b) - f(a)}{b - a} = 0 \implies f(b) - f(a) = f'(c)(b - a). \quad \blacksquare$$

### 6.5 Generalized (Cauchy) Mean Value Theorem
> If $f, g$ are continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists $c \in (a, b)$ such that:
> $$[f(b) - f(a)] g'(c) = [g(b) - g(a)] f'(c)$$
* *Proof:* Apply Rolle's Theorem to $h(x) = f(x)[g(b) - g(a)] - g(x)[f(b) - f(a)]$.

### 6.6 High-Frequency Applications of MVT
1. **Inequality Proof ($1 + x < e^x$ for $x > 0$, End 22/23 Q4(c)):**  
   Apply MVT to $f(t) = e^t$ on $[0, x]$. $f$ is continuous on $[0, x]$ and differentiable on $(0, x)$.  
   By MVT, there exists $c \in (0, x)$ such that:
   $$\frac{e^x - e^0}{x - 0} = f'(c) = e^c \implies e^x - 1 = x e^c$$
   Since $c > 0$, $e^c > 1$. Thus $x e^c > x \cdot 1 = x$.  
   Therefore $e^x - 1 > x \implies e^x > 1 + x$. $\blacksquare$
2. **Derivative Changes Signs (End 22/23 Q4(d)):**  
   Suppose $f$ is differentiable on $(a, b)$, continuous on $[a, b]$, $f(a) = f(b) = 0$, and $f(c) \neq 0$ for some $c \in (a, b)$.  
   * Proof:
     * Apply MVT on $[a, c]$: $\exists x_1 \in (a, c)$ s.t. $f(c) - f(a) = (c - a)f'(x_1) \implies f'(x_1) = \frac{f(c)}{c - a}$.
     * Apply MVT on $[c, b]$: $\exists x_2 \in (c, b)$ s.t. $f(b) - f(c) = (b - c)f'(x_2) \implies f'(x_2) = \frac{-f(c)}{b - c}$.
     * Since $c - a > 0$ and $b - c > 0$:
       * If $f(c) > 0$, then $f'(x_1) > 0$ and $f'(x_2) < 0$.
       * If $f(c) < 0$, then $f'(x_1) < 0$ and $f'(x_2) > 0$.  
     In both cases, one derivative is positive and the other is negative. $\blacksquare$
3. **Twice Differentiable Strict Convexity (End 23/24 Q3(b)(iv)):**  
   Let $x_1 < x_2 < x_3$ in $(a, b)$ with $f(x_1) > f(x_2)$ and $f(x_3) > f(x_2)$. Prove $\exists c \in (a, b)$ with $f''(c) > 0$.  
   * Proof:
     * Apply MVT on $[x_1, x_2]$: $\exists c_1 \in (x_1, x_2)$ s.t. $f'(c_1) = \frac{f(x_2) - f(x_1)}{x_2 - x_1} < 0$.
     * Apply MVT on $[x_2, x_3]$: $\exists c_2 \in (x_2, x_3)$ s.t. $f'(c_2) = \frac{f(x_3) - f(x_2)}{x_3 - x_2} > 0$.
     * Notice $c_1 < x_2 < c_2$. Now apply MVT to $f'$ on $[c_1, c_2]$:
       $$\exists c \in (c_1, c_2) \text{ s.t. } f''(c) = \frac{f'(c_2) - f'(c_1)}{c_2 - c_1}$$
       Since $f'(c_2) > 0$ and $f'(c_1) < 0$, the numerator $f'(c_2) - f'(c_1) > 0$. Since $c_2 > c_1$, the denominator is positive.  
       Hence $f''(c) > 0$. $\blacksquare$

---

# 7. Standard Proof Protocols & Master Templates

### Protocol 1: Bounding a Rational Sequence / Function $\epsilon-\delta$
* Goal: Show $\lim_{x\to a} \frac{P(x)}{Q(x)} = L$.
* Step 1: Form $\left|\frac{P(x)}{Q(x)} - L\right| = |x - a| \cdot \frac{|R(x)|}{|Q(x)|}$.
* Step 2: Set initial radius $\delta_0 = 1$ (or smaller if $a$ is close to a root of $Q(x)$).
* Step 3: From $|x - a| < \delta_0$, establish upper bound $M_1$ for $|R(x)|$ and positive lower bound $M_2$ for $|Q(x)|$.
* Step 4: Then $\left|\frac{P(x)}{Q(x)} - L\right| < |x - a| \frac{M_1}{M_2} < \epsilon \iff |x - a| < \frac{M_2}{M_1}\epsilon$.
* Step 5: Choose $\delta = \min\left\{\delta_0, \frac{M_2}{M_1}\epsilon\right\}$.

### Protocol 2: Recursive Sequence Convergence via MCT
* Given $x_1 = A, x_{n+1} = g(x_n)$.
* Step 1 (Boundedness): Use induction to prove $x_n < M$ for all $n$.
* Step 2 (Monotonicity): Use induction to prove $x_{n+1} > x_n$ (show $x_2 > x_1$, assume $x_k > x_{k-1}$, deduce $g(x_k) > g(x_{k-1})$).
* Step 3 (MCT Application): State MCT $\implies L = \lim x_n$ exists.
* Step 4 (Solve for limit): Solve $L = g(L)$ and discard roots outside the established bounds.

### Protocol 3: Root Existence via IVT
* Step 1: Identify or construct the function $h(x) = f(x) - g(x)$ (or $f(x) - C$).
* Step 2: State that $h$ is continuous on the chosen closed interval $[a, b]$ by the algebra of continuous functions.
* Step 3: Compute explicit values showing $h(a) < 0$ and $h(b) > 0$ (or vice-versa).
* Step 4: Quote IVT: there exists $c \in (a, b)$ such that $h(c) = 0 \iff f(c) = g(c)$.

---

# 8. Comprehensive Past Exam Solutions (End 22/23 & End 23/24)

### End-Semester 2022/2023 Solutions
#### Question 1(a) (40 Points)
* **(i) $\sup(A + B) = \sup A + \sup B$:** **TRUE.** (See full proof in Chapter 2, Section 2.4).
* **(ii) $\sup(A - B) = \sup A - \sup B$:** **FALSE.**  
  * *Counterexample:* Let $A = [0, 1]$ and $B = [0, 1]$. Then $\sup A = 1, \sup B = 1 \implies \sup A - \sup B = 0$. But $A - B = [-1, 1]$, so $\sup(A - B) = 1 \neq 0$. (The correct theorem is $\sup(A - B) = \sup A - \inf B$).

#### Question 1(b) (40 Points)
* **(i) Find $\sup$ and $\inf$ of $A = \left\{ \frac{m}{n} + \frac{4n}{m} : m, n \in \mathbb{Z}^+ \right\}$:**
  * By AM-GM inequality, for $a = \frac{m}{n} > 0$ and $b = \frac{4n}{m} > 0$:
    $$\frac{a + b}{2} \ge \sqrt{ab} = \sqrt{\frac{m}{n} \cdot \frac{4n}{m}} = \sqrt{4} = 2 \implies a + b \ge 4$$
  * To see if $4 \in A$: set $\frac{m}{n} = \frac{4n}{m} \implies m^2 = 4n^2 \implies m = 2n$.  
    Taking $n = 1, m = 2 \in \mathbb{Z}^+$ gives $\frac{2}{1} + \frac{4(1)}{2} = 2 + 2 = 4 \in A$.
  * Thus $\inf A = \min A = 4$.
  * Since taking $n = 1$ and $m \to \infty$ gives $\frac{m}{1} + \frac{4}{m} \to \infty$, $A$ is unbounded above.
  * Thus $\sup A$ does not exist (or $\sup A = +\infty$), and $\max A$ does not exist.
* **(ii) Find $\sup$ and $\inf$ of $B = \left\{ \frac{mn}{4m^2 + n^2} : m \in \mathbb{Z}, n \in \mathbb{Z}^+ \right\}$:**
  * Divide numerator and denominator by $mn$ (for $m \neq 0$):
    $$\frac{mn}{4m^2 + n^2} = \frac{1}{\frac{4m}{n} + \frac{n}{m}}$$
  * Notice the denominator is $\frac{4m}{n} + \frac{n}{m}$, which is the expression from part (i) when $m > 0$.
  * By part (i), for $m > 0$, $\frac{4m}{n} + \frac{n}{m} \ge 4$, with minimum $4$ at $m = 1, n = 2$.  
    Thus for $m > 0$, $\frac{mn}{4m^2 + n^2} \le \frac{1}{4}$, attained at $m = 1, n = 2 \implies \sup B = \max B = \frac{1}{4}$.
  * For $m = 0$: the value is $0$.
  * For $m < 0$: let $m = -k$ ($k \in \mathbb{Z}^+$). Then $\frac{mn}{4m^2 + n^2} = -\frac{kn}{4k^2 + n^2} \ge -\frac{1}{4}$, attained at $m = -1, n = 2 \implies \inf B = \min B = -\frac{1}{4}$.

#### Question 2(a) (40 Points)
* **(i) $x_n \to \infty \implies \frac{1}{x_n} \to 0$:** **TRUE.**  
  *Proof:* Let $\epsilon > 0$. Set $M = 1/\epsilon > 0$. Since $x_n \to \infty$, $\exists N \in \mathbb{Z}^+$ s.t. $n \ge N \implies x_n > M = 1/\epsilon$. Since $x_n > 1/\epsilon > 0$, we have $0 < \frac{1}{x_n} < \epsilon$, which implies $\left|\frac{1}{x_n} - 0\right| < \epsilon$. Thus $\frac{1}{x_n} \to 0$. $\blacksquare$
* **(ii) $x_n \to 0 \implies \frac{1}{x_n} \to \infty$:** **FALSE.**  
  *Counterexample:* Let $x_n = -\frac{1}{n}$. As $n \to \infty$, $x_n \to 0$. However, $\frac{1}{x_n} = -n \to -\infty \neq +\infty$.  
  *(Another counterexample: $x_n = \frac{(-1)^n}{n} \to 0$, but $\frac{1}{x_n} = (-1)^n n$ oscillates and diverges).*

#### Question 2(b) (20 Points)
* Evaluate $\lim_{n\to\infty} \left(1 + \frac{1}{n^2}\right)^{2n^2}$:  
  Let $k = n^2$. As $n \to \infty$, $k \to \infty$.  
  $$\lim_{n\to\infty} \left(1 + \frac{1}{n^2}\right)^{2n^2} = \lim_{k\to\infty} \left[ \left(1 + \frac{1}{k}\right)^k \right]^2 = e^2.$$

#### Question 4(a) (20 Points)
* Prove $\lim_{x\to 0} \frac{1}{x} \sum_{j=1}^k f(x/j) = \left(\sum_{j=1}^k \frac{1}{j}\right) f'(0)$ given $f(0)=0$:  
  *Proof:* Since $f(0) = 0$, for each $j \in \{1, 2, \dots, k\}$:
  $$\frac{1}{x} f(x/j) = \frac{1}{j} \cdot \frac{f(x/j) - f(0)}{x/j}$$
  Let $u = x/j$. As $x \to 0$, $u \to 0$. Since $f$ is differentiable at $0$:
  $$\lim_{x\to 0} \frac{f(x/j) - f(0)}{x/j} = \lim_{u\to 0} \frac{f(u) - f(0)}{u} = f'(0)$$
  By the sum rule for limits:
  $$\lim_{x\to 0} \frac{1}{x} \sum_{j=1}^k f(x/j) = \sum_{j=1}^k \frac{1}{j} \lim_{x\to 0} \frac{f(x/j) - f(0)}{x/j} = \left(\sum_{j=1}^k \frac{1}{j}\right) f'(0). \quad \blacksquare$$

#### Question 4(b) (30 Points)
* **(i) $f(x) = (x+4)^2(x-3)$ on $[-4, 3]$:**  
  * Continuity: $f$ is a polynomial, hence continuous on $[-4, 3]$.
  * Differentiability: $f$ is differentiable on $(-4, 3)$.
  * Boundary values: $f(-4) = 0, f(3) = 0 \implies f(-4) = f(3) = 0$.
  * Rolle's Theorem **applies**.
  * Find $c$: $f'(x) = 2(x+4)(x-3) + (x+4)^2 = (x+4)[2x - 6 + x + 4] = (x+4)(3x - 2)$.  
    $f'(c) = 0 \implies c = -4$ or $c = 2/3$.  
    Since $c \in (-4, 3)$, the unique value is $c = \frac{2}{3}$.
* **(ii) $f(x) = 3 - |x-3|$ on $[0, 6]$:**  
  * $f(0) = 3 - 3 = 0, f(6) = 3 - 3 = 0$. $f$ is continuous on $[0, 6]$.
  * However, $f$ is **NOT differentiable at $x = 3 \in (0, 6)$** (sharp corner; left derivative is $+1$, right derivative is $-1$).
  * Rolle's Theorem **cannot be applied**.

---

### End-Semester 2023/2024 Solutions
#### Part A — Multiple Choice Questions (Keys & Explanations)
1. **Least upper bound property:** **(C)** $\sup E \in \mathbb{R}$ exists. *(By Completeness Axiom; need not be in $\mathbb{Q}$, need not be in $E$).*
2. **$E \subset \mathbb{Z}$ bounded above:** **(B)** $\sup E \in E$. *(Integer supremum property; $\sup E$ must be an integer and belong to $E$).*
3. **Archimedean Principle ($a > 0$):** **(B)** $\exists n \in \mathbb{Z}^+$ s.t. $b < na$.
4. **Density of $\mathbb{Q}$ in $\mathbb{R}$:** **(A)** Between any two real numbers there is a rational number.
5. **Subsequence of convergent sequence:** **(C)** Converges to $L$.
6. **Every bounded sequence in $\mathbb{R}$:** **(C)** Has a convergent subsequence *(Bolzano-Weierstrass Theorem)*.
7. **$x_n \to 0$ and $\{y_n\}$ bounded:** **(B)** $x_n y_n \to 0$.
8. **Extreme Value Theorem:** **(A)** Continuous $f$ on $[a, b]$ is bounded and attains max/min.
9. **One-sided limits equal $L$:** **(B)** $\lim_{x\to a} f(x) = L$. *(Note: does NOT imply $f(a) = L$, which is continuity).*
10. **Differentiable at $a$:** **(A)** $f$ is continuous at $a$.

#### Part B, Question 3(b)(iii) (MVT Application)
* Determine if MVT applies to $f(x) = x^2 - x^{2/3}$ on $[-1, 8]$:
  * Check differentiability: $f'(x) = 2x - \frac{2}{3} x^{-1/3} = 2x - \frac{2}{3x^{1/3}}$.
  * At $x = 0 \in (-1, 8)$, $f'(0)$ does not exist (division by zero, vertical tangent / cusp).
  * Since $f$ is **not differentiable at $x = 0 \in (-1, 8)$**, the Mean Value Theorem **cannot be applied** to $f$ on $[-1, 8]$.

---

# 9. Quick-Fire MCQ & True/False Revision Bank

| Statement | Truth Value | Critical Reason / Counterexample |
| :--- | :---: | :--- |
| If a nonempty subset of $\mathbb{R}$ has an upper bound, it has a least upper bound. | **TRUE** | Completeness Axiom of $\mathbb{R}$. |
| If a nonempty subset of $\mathbb{R}$ has an infimum, it is bounded. | **FALSE** | It is only bounded *below* (e.g., $[0, \infty)$ has infimum $0$ but is unbounded). |
| Every nonempty bounded subset of $\mathbb{R}$ has a maximum and a minimum. | **FALSE** | Open interval $(0, 1)$ is bounded, but has no maximum or minimum. |
| The negation of a universal statement is another universal statement. | **FALSE** | $\neg(\forall x, P(x)) \equiv \exists x, \neg P(x)$ (existential statement). |
| If $x_n < y_n$ for all $n$, then $\lim x_n < \lim y_n$. | **FALSE** | Inequality becomes weak: $0 < 1/n$ for all $n$, but $\lim 0 = \lim 1/n = 0$. |
| If $\{x_n\}$ converges, then $\{x_n/n\}$ converges. | **TRUE** | $x_n \to L$ and $1/n \to 0 \implies x_n(1/n) \to L \cdot 0 = 0$. |
| If $\{x_n y_n\}$ converges and $\{x_n\}$ converges, then $\{y_n\}$ converges. | **FALSE** | Let $x_n = 0$ (converges to $0$) and $y_n = (-1)^n$ (diverges); $x_n y_n = 0$ converges. |
| If $f$ is continuous on $(a, b)$, then $f$ attains a maximum on $(a, b)$. | **FALSE** | Requires closed and bounded interval $[a, b]$ by EVT. Counterexample: $f(x) = x$ on $(0, 1)$. |
| If $f'(x) = 0$ for all $x \in (a, b)$, then $f$ is constant on $(a, b)$. | **TRUE** | Consequence of Mean Value Theorem ($f(x_2) - f(x_1) = f'(c)(x_2 - x_1) = 0$). |
| If $f$ is differentiable at $a$, then $|f|$ is differentiable at $a$. | **FALSE** | Let $f(x) = x$ (differentiable at $0$). Then $|f(x)| = |x|$ is not differentiable at $0$. |
| Continuous functions preserve intervals: if $I$ is an interval, $f(I)$ is an interval. | **TRUE** | Direct consequence of the Intermediate Value Theorem. |
| Differentiable implies continuous; continuous implies integrable. | **TRUE** | Standard hierarchy of real analysis. |
