
---
### Course Information
* **Problem Sheet 1:** Logic and Proof
* **Lecturer:** Dr. Rajitha Ranasinghe
* **Tutors:** Mr. Lakmina Dilshan, Ms. Shavindhya Jayatilake, Mr. Salinda Perera

> "A mathematician, like a painter or a poet, is a maker of patterns... The mathematician's patterns, like the painter's or the poet's must be beautiful; the ideas, like the colours or the words, must fit together in a harmonious way."  
> — **G. H. HARDY**, *A Mathematician's Apology*

---
## Part A: Logical Connectives

### 1. Mathematical Statements
Determine whether each of the following sentences is a mathematical statement (proposition). If it is not a statement, provide a brief explanation why.
* **(a)** Every prime number strictly greater than 2 is an odd integer.
	* True. Every even Number greater than 2 is divisible by 2. 
* **(b)** $x^2 - 4x + 4 = 0$
	* True for x=
* **(c)** There exists a real number $x$ such that $x^2 = -1$.
* **(d)** Is the set of rational numbers countable?
* **(e)** Real analysis is the most beautiful subject in mathematics.
* **(f)** Every even integer greater than 2 can be expressed as the sum of two prime numbers.
* **(g)** There are infinitely many prime numbers $p$ such that $p + 2$ is also a prime number.
* **(h)** The Banach space $X$ is uniformly convex.

### 2. Identifying Antecedents and Consequents
For each of the following mathematical implications, identify the antecedent (hypothesis) and the consequent (conclusion).
* **(a)** A sequence $(x_n)$ of real numbers is convergent only if it is a Cauchy sequence.
* **(b)** A function $f : \mathbb{R} \to \mathbb{R}$ is continuous at $c \in \mathbb{R}$, provided that it is differentiable at $c$.
* **(c)** The infinite series $\sum a_n$ converges absolutely whenever the limit superior of $\sqrt[n]{|a_n|}$ is strictly less than 1.
* **(d)** A sufficient condition for a subset $K$ of $\mathbb{R}$ to be compact is that $K$ is both closed and bounded.
* **(e)** Assuming $f$ is differentiable at $x_0$, a necessary condition for a real-valued function $f$ to have a local extremum at $x_0$ in its open domain is that $f'(x_0) = 0$.
* **(f)** Uniform continuity of a function $f$ on an interval $I$ implies that $f$ is continuous on $I$.

### 3. Analyzing Deduced Implications
Consider the following true mathematical theorem regarding a real-valued function $f$ and a point $x_0$ in its open domain:
$$\text{"If } f \text{ is differentiable at } x_0 \text{ and } f \text{ has a local extremum at } x_0, \text{ then } f'(x_0) = 0\text{"}$$
Based on the logical structure of this theorem, determine whether each of the following deduced implications is True or False. If an implication is false, provide a brief explanation or a counterexample showing why.
* **(a)** If $f'(x_0) = 0$, then $f$ has a local extremum at $x_0$.
* **(b)** If $f$ is differentiable at $x_0$ and $f'(x_0) \neq 0$, then $f$ does not have a local extremum at $x_0$.
* **(c)** If $f$ has a local extremum at $x_0$, then $f'(x_0) = 0$.
* **(d)** If $f'(x_0) \neq 0$, then $f$ is not differentiable at $x_0$ or $f$ does not have a local extremum at $x_0$.

### 4. Truth Tables
Construct truth tables for the following compound propositions. For each, clearly determine whether it is a tautology, a contradiction, or a contingency (neither).
* **(a)** $(P \Rightarrow Q) \vee (Q \Rightarrow P)$
* **(b)** $(P \vee Q) \Rightarrow (P \wedge Q)$
* **(c)** $P \Rightarrow (Q \Rightarrow R)$
* **(d)** $(P \wedge Q) \Rightarrow (P \vee R)$
* **(e)** $(P \Rightarrow Q) \wedge \neg(P \Rightarrow (Q \vee R))$

### 5. Converse, Negation, and Contrapositive
For each of the following mathematical statements, write its converse, negation, and contrapositive.  
*Hint: Before starting, it may help to translate the statement into standard "If P, then Q" form. If a statement is fundamentally not an implication, state that the converse and contrapositive do not apply, and simply write its negation.*
* **(a)** A sequence of real numbers $(x_n)$ is convergent only if it is bounded.
* **(b)** The infinite series $\sum a_n$ converges whenever the sequence of its partial sums is bounded.
* **(c)** Every monotonically decreasing sequence that is bounded below is convergent.
* **(d)** A necessary condition for a real-valued function $f$ to have a local extremum at $x_0$ is that $f'(x_0) = 0$.
* **(e)** There exists a positive real number $M$ such that $|f(x)| \le M$ for all $x \in \mathbb{R}$.

### 6. Truth Value Assessment
Indicate whether each statement is True or False.
* **(a)** If 3 is odd or $4 > 6$, then $9 \le 5$.
* **(b)** If both $5 - 3 = 2$ and $5 + 3 = 2$, then $9 = 4$.
* **(c)** It is not the case that 5 is even or 7 is prime.
* **(d)** If $2 + 5 = 7$ only if $3 + 4 = 8$, then $32 = 9$.
* **(e)** If both $5 - 3 = 2$ and $5 + 3 = 8$, then $8 - 3 = 4$.
* **(f)** It is not the case that 5 is not prime and 3 is odd.

### 7. Logical Reasoning Scenario
Consider the following relatable, everyday scenario about life and relationships:
* **Premise 1:** If I receive my first salary, then I will buy a gift for my significant other.
* **Premise 2:** If I buy a gift for my significant other, then they will be happy.
* **Conclusion:** Therefore, if I receive my first salary, then they will be happy.

* **(a)** Identify the three fundamental declarative statements in this everyday scenario and label them $P$, $Q$, and $R$.
* **(b)** Translate the two premises and the conclusion into formal logical language. Then, write the entire scenario as a single compound implication in the form: $((P_1 \wedge P_2) \to C)$.
* **(c)** Construct a truth table for your compound proposition from part (b). By demonstrating that it is a tautology, logically conclude that this everyday reasoning is perfectly valid.
* **(d)** Suppose someone changes the reasoning to say:  
  *"If I receive my first salary, they will be happy. They are happy today. Therefore, I must have received my first salary."*  
  Translate this new argument into logical symbols and use a truth table to show that this outcome is a contingency (this logical flaw is known as the *Fallacy of the Converse*). Briefly explain what this means in real life.
* **(e)** Finally, imagine a situation where someone claims:  
  *"I received my first salary, and both original premises are perfectly true, but my significant other is not happy."*  
  Formulate this entire claim logically as a single conjunction (AND statement). Use a truth table to prove it is a contradiction, thereby proving that this specific emotional outcome is logically impossible under the given rules.

### 8. Converses, Negations, and Contrapositives (Everyday Context)
For each of the following everyday statements, write its converse, negation, and contrapositive.
* **(a)** You can board the international flight only if you have a valid passport.
* **(b)** The campus Wi-Fi network crashes whenever it rains heavily.
* **(c)** Every student who submits their assignment late receives a grade penalty.
* **(d)** A necessary condition for getting a driver's license is passing the practical road test.
* **(e)** There exists a master key that unlocks every classroom in the mathematics department.

### 9. Cricket Tournament Implication Analysis
Consider the following true statement regarding a local cricket tournament:
$$\text{"If it rains heavily, then the match is delayed or the match is canceled."}$$
Based on the logical structure of this statement, determine whether each of the following deduced implications is True or False. If an implication is false, provide a brief explanation.
* **(a)** If the match is delayed or canceled, then it rained heavily.
* **(b)** If it rains heavily and the match is not delayed, then the match is canceled.
* **(c)** If the match is not canceled, then it did not rain heavily.
* **(d)** If the match is not delayed and the match is not canceled, then it did not rain heavily.

---

## Part B: Quantifiers

### 10. Formal Logic Translation
Write each statement using $\exists$, $\forall$, and $\ni$ (or structural layout) as appropriate, along with the negation of each statement.
* **(a)** There exists a positive number $x$ such that $x^2 = 5$.
* **(b)** For every positive number $M$, there is a positive number $N$ such that $N < \frac{1}{M}$.
* **(c)** If $n \ge N$ then $|f_n(x) - f(x)| \le 3$ for all $x \in A$.
* **(d)** No positive number $x$ satisfies the equation $f(x) = 5$.

### 11. Core Concept True/False
Mark each statement True or False. Justify each answer.
* **(a)** The symbol "$\forall$" means "for every."
* **(b)** The negation of a universal statement is another universal statement.
* **(c)** The symbol "$\ni$" is read "such that."
* **(d)** The symbol "$\exists$" means "there exist several."
* **(e)** If a variable is used in the antecedent of an implication without being quantified, then the universal quantifier is assumed to apply.
* **(f)** The order in which quantifiers are used affects the truth value.

### 12. Truth Values of Quantified Real Analysis Statements
Determine the truth value of each statement, assuming $x$ is a real number. Justify your answer.
* **(a)** $\exists x \in [3,5] \ni x \ge 4$.
* **(b)** $\forall x \in [3,5], x \ge 4$.
* **(c)** $\exists x \ni x^2 = 3$.
* **(d)** $\forall x, x^2 \neq 3$.
* **(e)** $\exists x \ni x^2 = -5$.
* **(f)** $\forall x, x^2 = -5$.
* **(g)** $\exists x \ni x - x = 0$.
* **(h)** $\forall x, x - x = 0$.

### 13. Logical Proof Strategy Selection
Below are two strategies for determining the truth value of a statement involving a positive number $x$ and another statement $P(x)$.
* **(i)** Find some $x > 0$ such that $P(x)$ is true.
* **(ii)** Let $x$ be any number greater than 0 and show $P(x)$ is true.

For each statement below, indicate which strategy is more appropriate.
* **(a)** $\forall x > 0, P(x)$.
* **(b)** $\exists x > 0 \ni P(x)$.
* **(c)** $\exists x > 0 \ni \neg P(x)$.
* **(d)** $\forall x > 0, \neg P(x)$.

### 14. Real Analysis Definitions
The question gives certain properties of functions. You are to do two things:
1. Rewrite the defining conditions in logical symbolism using $\forall$, $\exists$, and structural implications as appropriate.
2. Write the negation of part (1) using the same symbolism.

*Example: A function $f$ is odd if for every $x$, $f(-x) = -f(x)$.*
* *(i) defining condition: $\forall x, f(-x) = -f(x)$.*
* *(ii) negation: $\exists x \ni f(-x) \neq -f(x)$.*

* **(a)** A function $f$ is even if for every $x$, $f(-x) = f(x)$.
* **(b)** A function $f$ is periodic if there exists a $k > 0$ such that for every $x$, $f(x+k) = f(x)$.
* **(c)** A function $f$ is increasing if for every $x$ and $y$, if $x \le y$, then $f(x) \le f(y)$.
* **(d)** A function $f$ is strictly decreasing if for every $x$ and $y$, if $x < y$ then $f(x) > f(y)$.
* **(e)** A function $f : A \to B$ is injective if for every $x$ and $y$ in $A$, if $f(x) = f(y)$ then $x = y$.
* **(f)** A function $f : A \to B$ is surjective if for every $y$ in $B$ there exists an $x$ in $A$ such that $f(x) = y$.
* **(g)** A function $f : D \to \mathbb{R}$ is continuous at $c \in D$ if for every $\epsilon > 0$ there is a $\delta > 0$ such that $|f(x) - f(c)| < \epsilon$ whenever $|x - c| < \delta$ and $x \in D$.
* **(h)** A function $f$ is uniformly continuous on a set $S$ if for every $\epsilon > 0$ there is a $\delta > 0$ such that $|f(x) - f(y)| < \epsilon$ whenever $x, y \in S$ and $|x - y| < \delta$.
* **(i)** The real number $L$ is the limit of the function $f : D \to \mathbb{R}$ at the point $c$ if for each $\epsilon > 0$ there exists a $\delta > 0$ such that $|f(x) - L| < \epsilon$ whenever $x \in D$ and $0 < |x - c| < \delta$.

### 15. Identification of Error in Quantifier Negation
Identify the error in each of the following claims about negation or quantifier use, and write the correct version.
* **(a)** The negation of "$\forall x, f(x) > 0$" is "$\forall x, f(x) \le 0$".
* **(b)** The negation of "$\exists x \ni P(x) \text{ and } Q(x)$" is "$\forall x, \neg P(x) \text{ and } \neg Q(x)$".
* **(c)** The statements $\forall x \exists y \ni y = x^2$ and $\exists y \ni \forall x, y = x^2$ are logically equivalent over $\mathbb{R}$.

### 16. Logical Equivalence vs. Strength Comparisons
For each pair of statements, determine whether they are logically equivalent. If they are not, state which is stronger and provide a justification or counterexample.
* **(a)** $\forall x \in \mathbb{R}, \exists y \in \mathbb{R} \ni x^2 + y^2 = 1$ vs. $\exists y \in \mathbb{R} \ni \forall x \in \mathbb{R}, x^2 + y^2 = 1$.
* **(b)** $\forall \epsilon > 0, \exists \delta > 0 \ni \forall x, |x - c| < \delta \Rightarrow |f(x) - f(c)| < \epsilon$ vs. $\exists \delta > 0 \ni \forall \epsilon > 0, \forall x, |x - c| < \delta \Rightarrow |f(x) - f(c)| < \epsilon$.
* **(c)** $\forall m \in \mathbb{N}, \exists n \in \mathbb{N} \ni n > m$ vs. $\exists n \in \mathbb{N} \ni \forall m \in \mathbb{N}, n > m$.
* **(d)** $\forall x > 0, \exists n \in \mathbb{N} \ni \frac{1}{n} < x$ vs. $\exists n \in \mathbb{N} \ni \forall x > 0, \frac{1}{n} < x$.
* **(e)** $\exists M > 0 \ni \forall x \in S, |f(x)| \le M$ vs. $\forall x \in S, \exists M > 0 \ni |f(x)| \le M$.
* **(f)** $\forall \epsilon > 0, \exists N \in \mathbb{N} \ni \forall m, n > N, |a_m - a_n| < \epsilon$ vs. $\forall \epsilon > 0, \forall m, \exists N \in \mathbb{N} \ni \forall n \ge N, |a_m - a_n| < \epsilon$.

### 17. Writing Using Symbols
Write each statement using symbols $\forall$, $\exists$, and $\Rightarrow$, and then write its negation.
* **(a)** Every real number greater than 1 has a square greater than 1.
* **(b)** There exists a natural number $n$ such that $n^2 + n + 1$ is even.
* **(c)** No real number satisfies the equation $x^2 + 1 = 0$.

### 18. Evaluative Truth/False Problems
Determine whether each statement is True or False. Justify your answer.
* **(a)** $\forall x \in \mathbb{R}, x^2 \ge 0$.
* **(b)** $\exists x \in \mathbb{R} \ni x^2 = -1$.
* **(c)** $\forall x \in \mathbb{R}, x + 1 > x$.
* **(d)** $\exists x \in \mathbb{R} \ni x^2 = 2$.

### 19. Defining Conditions and Negations
For each definition: (i) Write the statement using logical symbols. (ii) Write the negation.
* **(a) Bounded Function:** A function $f : S \to \mathbb{R}$ is bounded if there exists a number $M > 0$ such that for every $x \in S$, $|f(x)| \le M$.
* **(b) Constant Function:** A function $f : \mathbb{R} \to \mathbb{R}$ is constant if there exists a real number $c$ such that for every real number $x$, $f(x) = c$.
* **(c) Positive Function:** A function $f$ is positive on a set $A$ if for every $x \in A$, $f(x) > 0$.

### 20. Translation into Conversational English
Let $f : (0,1) \to \mathbb{R}$ be a real-valued function defined on the open interval $I = (0,1)$. Consider the following mathematical statements and translate the mathematical logic into plain, conversational English:
* **(a)** $\forall x \in I, \exists M > 0 \text{ such that } |f(x)| < M$
* **(b)** $\exists M > 0 \text{ such that } \forall x \in I, |f(x)| < M$
* **(c)** $\forall x \in I, \forall \epsilon > 0, \exists \delta > 0 \text{ such that } \forall y \in I, \text{ if } |x - y| < \delta, \text{ then } |f(x) - f(y)| < \epsilon.$
* **(d)** $\forall \epsilon > 0, \exists \delta > 0 \text{ such that } \forall x, y \in I, \text{ if } |x - y| < \delta, \text{ then } |f(x) - f(y)| < \epsilon.$

### 21. Multi-Quantifier Error Identification
Identify the logical error in each of the following claims concerning quantifiers, negations, and implications. Write the logically correct version and provide a brief explanation of the flaw.
* **(a)** The negation of "$\forall \epsilon > 0, \exists \delta > 0 \ni \forall x \in D, |x - c| < \delta \Rightarrow |f(x) - f(c)| < \epsilon$" is "$\exists \epsilon > 0 \ni \forall \delta > 0, \exists x \in D \ni |x - c| \ge \delta \text{ and } |f(x) - f(c)| \ge \epsilon$".
* **(b)** The statement "$\forall x \in \mathbb{R}, \exists M > 0 \ni |f(x)| \le M$" is logically equivalent to "$\exists M > 0 \ni \forall x \in \mathbb{R}, |f(x)| \le M$".
* **(c)** The negation of "$\exists x \in \mathbb{R} \ni (f(x) > 0 \Rightarrow \forall y \in \mathbb{R}, g(x,y) = 0)$" is "$\forall x \in \mathbb{R}, f(x) \le 0 \text{ and } \exists y \in \mathbb{R} \ni g(x,y) \neq 0$".

---

## Part C: Techniques of Proof: I

### 22. Foundational Proof Terminology
Mark each statement True or False. Justify each answer.
* **(a)** When an implication $p \Rightarrow q$ is used as a theorem, we refer to $p$ as the antecedent.
* **(b)** The contrapositive of $p \Rightarrow q$ is $\neg p \Rightarrow \neg q$.
* **(c)** The inverse of $p \Rightarrow q$ is $\neg q \Rightarrow \neg p$.
* **(d)** To prove "$\forall n, P(n)$" is true, it takes only one example.
* **(e)** To prove "$\exists n \text{ such that } P(n)$" is true, it takes only one example.
* **(f)** When an implication $p \Rightarrow q$ is used as a theorem, we refer to $q$ as the conclusion.

### 23. Disproving Universals via Counterexamples
Provide a counterexample for each statement.
* **(a)** For every real number $x$, if $x^2 > 9$ then $x > 3$.
* **(b)** For every integer $n$, we have $n^3 \ge n$.
* **(c)** For all real numbers $x \ge 0$, we have $x^2 \le x^3$.
* **(d)** Every triangle is a right triangle.
* **(e)** For every positive integer $n$, $n^2 + n + 41$ is prime.
* **(f)** Every prime is an odd number.
* **(g)** No integer greater than 100 is prime.
* **(h)** $3n + 2$ is prime for all positive integers $n$.
* **(i)** For every integer $n > 3$, $3n$ is divisible by 6.
* **(j)** If $x$ and $y$ are unequal positive integers and $xy$ is a perfect square, then $x$ and $y$ are perfect squares.
* **(k)** For every real number $x$, there exists a real number $y$ such that $xy = 2$.
* **(l)** The reciprocal of a real number $x > 1$ is a real number $y$ such that $0 < y < 1$.
* **(m)** No rational number satisfies the equation $x^3 + (x-1)^2 = x^2 + 1$.
* **(n)** The equation $x^4 + \frac{1}{x} - \sqrt{x+1} = 0$ has no rational solution.

### 24. Direct Algebraic Proofs (Parity of Integers)
Suppose $p$ and $q$ are integers. Recall that an integer $m$ is even iff $m = 2k$ for some integer $k$, and $m$ is odd iff $m = 2k+1$ for some integer $k$.  
Prove the following. [You may use the fact that the sum of integers and the product of integers are again integers.]
* **(a)** If $p$ is odd and $q$ is odd, then $p + q$ is even.
* **(b)** If $p$ is odd and $q$ is odd, then $pq$ is odd.
* **(c)** If $p$ is odd and $q$ is odd, then $p + 3q$ is even.
* **(d)** If $p$ is odd and $q$ is even, then $p + q$ is odd.
* **(e)** If $p$ is even and $q$ is even, then $p + q$ is even.
* **(f)** If $p$ is even or $q$ is even, then $pq$ is even.
* **(g)** If $pq$ is odd, then $p$ is odd and $q$ is odd.
* **(h)** If $p^2$ is even, then $p$ is even.
* **(i)** If $p^2$ is odd, then $p$ is odd.

### 25. Formal Proof Matrix (Sports Scenario)
Assume that the following two hypotheses are true:
1. **Hypothesis A:** If the basketball center is healthy or the point guard is hot, then the team will win and the fans will be happy.
2. **Hypothesis B:** If the fans are happy or the coach is a millionaire, then the college will balance the budget.

* **Conclusion to prove:** If the basketball center is healthy, then the college will balance the budget.
* **Task:** Using the hypotheses above, derive the conclusion in a formal proof. You must write your proof in a step-by-step format and clearly indicate which logical tautology or rule of inference is used at each step.

### 26. Formal Proof Matrix (Academic Scenario)
Assume the following hypotheses are true:
1. **Hypothesis A:** If the library is open or the internet is working, then students will study and the assignment will be submitted on time.
2. **Hypothesis B:** If students study or the lecturer extends the deadline, then the course pass rate will increase.
3. **Hypothesis C:** If the assignment is submitted on time, then the lecturer extends the deadline.

* **Conclusion to prove:** If the library is open, then the course pass rate will increase.
* **Task:** Using the hypotheses above, construct a formal step-by-step proof of the conclusion. At each step, clearly state the logical tautology or rule of inference used.

### 27. Logical Form Conversions
For each of the following statements, determine the converse, inverse, and contrapositive. Clearly rewrite each statement in correct logical form. You may assume all variables range over real numbers unless otherwise stated.
* **(a)** For all $x \in \mathbb{R}$, if $x > 2$, then $x^2 > 4x$.
* **(b)** For all functions $f : \mathbb{R} \to \mathbb{R}$, if $f$ is continuous at $a$, then for every $\epsilon > 0$, there exists $\delta > 0$ such that $|x - a| < \delta \Rightarrow |f(x) - f(a)| < \epsilon$.
* **(c)** For all integers $n$, if $n^2$ is even, then $n$ is even.
* **(d)** For all sequences $(a_n)$, if $(a_n)$ is Cauchy, then $(a_n)$ is bounded.
* **(e)** For all matrices $A \in M_{n \times n}(\mathbb{R})$, if $A^2 = I$, then $A$ is invertible and $A^{-1} = A$.

### 28. Philosophical Essay Component
Consider the following sentences:
* **(a)** The nucleus of a carbon atom consists of protons and neutrons.
* **(b)** Jesus Christ rose from the dead and is alive today.
* **(c)** Every differentiable function is continuous.

Each of these sentences has been affirmed by some people at some time as being "true." Write an essay on the nature of truth, comparing and contrasting its meaning in these (and possibly other) contexts.  
You might also want to consider some of the following questions:
* To what extent is truth absolute?
* To what extent can truth change with time?
* To what extent is truth based on opinion?
* To what extent are people free to accept as true anything they wish?

### 29. Proof Evaluation Case Study (Induction/Summation)
A student attempts to prove the following theorem using a chain of implications:
$$\text{Theorem: If a sequence } \{a_n\} \text{ is defined by } a_n = 2n - 1 \text{ for all } n \in \mathbb{Z}^+, \text{ then the sum of the first } n \text{ terms satisfies } S_n = n^2.$$
The student's proof is as follows:
> "We verify for small values:  
> $S_1 = 1 = 1^2 \quad \checkmark$  
> $S_2 = 1 + 3 = 4 = 2^2 \quad \checkmark$  
> $S_3 = 1 + 3 + 5 = 9 = 3^2 \quad \checkmark$  
> **Step 1:** The terms of the sequence are 1, 3, 5, 7, ..., which are odd numbers.  
> **Step 2:** Adding odd numbers always gives a perfect square, as seen above.  
> **Step 3:** Therefore $S_n = n^2$ for all $n \in \mathbb{Z}^+$."

* **(a)** Identify the hypothesis $p$ and conclusion $q$ of the theorem.
* **(b)** Is the student's verification of small cases sufficient to prove the theorem for all $n \in \mathbb{Z}^+$? What type of reasoning is being used in Steps 1–3?
* **(c)** Step 2 is stated without rigorous justification. Construct a correct proof using a direct algebraic approach by writing $S_n = \sum_{k=1}^n (2k - 1)$ and evaluating it using summation formulas.
* **(d)** The student's conclusion happens to be correct. Does that mean the proof is valid? Explain the difference between a true statement and a proved statement, using ideas from the course notes.

### 30. Counterexample Evaluation (Injective vs. Monotone)
A student attempts to disprove the following statement using a counterexample:
$$\text{Statement: For every function } f : \mathbb{R} \to \mathbb{R}, \text{ if } f \text{ is one-to-one, then } f \text{ is an increasing function.}$$
The student's argument is as follows:
> "We try $f(x) = x^2$. We note that $f(2) = 4$ and $f(3) = 9$, so $f(2) \neq f(3)$. Since different inputs give different outputs, $f$ is one-to-one. But $f(-1) = 1$ and $f(1) = 1$ which contradicts the conclusion. Therefore the statement is false."

* **(a)** What is the student trying to show? Is the general approach of using a counterexample appropriate here?
* **(b)** The student claims $f(x) = x^2$ is one-to-one. Is this correct? Justify your answer carefully, and if it is wrong, explain why this makes the student's counterexample invalid.
* **(c)** Find a valid counterexample to disprove the statement. (*Hint: Think of a one-to-one function that is not increasing everywhere.*)
* **(d)** Write the contrapositive of the original statement.

### 31. Proof Evaluation Case Study (Contrapositive Parity)
A student claims to have proved the following theorem using proof by contrapositive:
$$\text{Theorem: If } 7m \text{ is an odd number, then } m \text{ is an odd number.}$$
The student's proof is as follows:
> "We use the contrapositive. The contrapositive is: If $7m$ is an even number, then $m$ is an even number. Assume $7m$ is even. Then $7m = 2k$ for some $k \in \mathbb{Z}$, so $m = \frac{2k}{7}$. Since $m = \frac{2k}{7}$ is a fraction divided by 7, it may not always be an integer, so we cannot conclude anything. Therefore the theorem is unproven."

* **(a)** Write the correct contrapositive of the theorem.
* **(b)** Identify the flaw in the student's reasoning. Is it valid to conclude that $\frac{2k}{7}$ is even simply because $2k$ is even?
* **(c)** Construct a correct proof of the theorem using the contrapositive.

### 32. Fallacy Analysis (Converse Fallacy in Calculus)
A student attempts to prove the following theorem using its converse:
$$\text{Theorem: If a function is differentiable, then it is continuous.}$$
The student's proof is as follows:
> "We prove the converse: If a function is continuous, then it is differentiable. Consider any continuous function $f$. Since continuity means the function has no breaks or jumps, it must be smooth everywhere, and therefore differentiable. Since the converse is true, the original theorem is also true."

* **(a)** Write the contrapositive of the original theorem.
* **(b)** From the notes, is an implication logically equivalent to its converse? What does this mean for the student's approach?
* **(c)** Is the converse itself actually true? Provide a counterexample if it is false.
* **(d)** Does the student's argument prove the original theorem? Justify your answer.

### 33. Mathematical Induction Proof
Prove by mathematical induction that for all integers $n > 1$, the following inequality holds:
$$\sum_{k=1}^{n} \frac{1}{\sqrt{k}} \le 2\sqrt{n} - 1$$

### 34. Structured Counterexamples
Provide a counterexample to prove that each of the following mathematical claims is False.
* **(e)** For any two irrational numbers $x$ and $y$, their sum $x + y$ is also an irrational number.
* **(f)** For any sets $A$, $B$, and $C$, if $A \cup B = A \cup C$ then $B = C$.
* **(g)** For all real numbers $x$ and $y$, the absolute value of their sum is equal to the sum of their absolute values: $|x + y| = |x| + |y|$.
* **(h)** If $x$ is any real number, then $\sqrt{x^2} = x$.
* **(i)** If $f : \mathbb{R} \to \mathbb{R}$ and $g : \mathbb{R} \to \mathbb{R}$ are both strictly increasing functions, then their product function $(fg)(x) = f(x)g(x)$ is also strictly increasing on $\mathbb{R}$.

---

## Part D: Techniques of Proof: II

### 35. The Proof Autopsy
A crucial part of mastering mathematical logic is learning to evaluate the validity of a proof's structure. Below are four snippets of flawed proofs submitted by a student. Each snippet contains a fundamental methodological error regarding proof techniques. For each snippet, identify the logical error and briefly explain the correct approach you would teach the student to use.

* **(a) Claim:** For all real numbers $x$, if $x > 0$, then $x + \frac{1}{x} \ge 2$.  
  *Proof:* We can easily verify this. Let $x = 2$. Since $2 > 0$, we calculate $2 + \frac{1}{2} = 2.5$. Since $2.5 \ge 2$, the statement is true. Therefore, the claim holds for all $x$.
* **(b) Claim:** There exists an even prime number.  
  *Proof:* Let $p$ be an arbitrary prime number. By the definition of primes, $p$ has exactly two distinct positive divisors. Since there are infinitely many primes, logic dictates that at least one of them must be divisible by 2. Thus, an even prime exists.
* **(c) Claim:** If a sequence $(x_n)$ is convergent, then $(x_n)$ is bounded.  
  *Proof:* We will prove this by contradiction. Assume that the sequence $(x_n)$ is divergent (not convergent) and that $(x_n)$ is bounded. We will now look for a contradiction...
* **(d) Claim:** The sum of any two odd integers is even.  
  *Proof:* Let a and b be two odd integers. If you add two numbers that cannot be cleanly divided by 2, their remainders will combine to make a number that can be divided by 2. Therefore, $a+b$ is clearly even.

### 36. Multi-Quantifier Analysis ($\epsilon$-$\delta$ Mechanics)
In Real Analysis, you will frequently encounter statements that stack multiple quantifiers together (such as "for all $\epsilon$, there exists a $\delta$"). Consider the following mathematical claim written in English:
$$\text{"For every strictly positive real number } \epsilon, \text{ there exists a strictly positive real number } \delta \text{ such that for all real numbers } x, \text{ if } |x| < \delta, \text{ then } |4x| < \epsilon.\text{"}$$

* **(a)** Translate this English statement into a formal logical proposition using the quantifiers $\forall$ and $\exists$.
* **(b)** To logically prove that a $\delta$ exists for every $\epsilon$, we must find a formula for it. Let $\epsilon > 0$ be an arbitrary real number. Perform the "scratchwork" to find a suitable candidate for $\delta$ (in terms of $\epsilon$) that guarantees the implication is true.
* **(c)** Using your candidate from part (b), write the formal, rigorous mathematical proof. Ensure your proof closely mirrors the logical structure from part (a): declaring the arbitrary $\epsilon$, explicitly choosing your $\delta$, and proving the final implication.

### 37. Parity Proof (Higher Powers)
Prove that if $n$ is an integer, then $n^2 + n^3$ is an even number.

### 38. Existential and Uniqueness Proofs
Prove that there exists an integer $n$ such that $n^2 + \frac{3n}{2} = 1$. Is this integer unique? If $n$ was allowed to be a rational number, what could you conclude?

### 39. Conditional Polynomial Inequalities
Prove that for any real number $x$, if $x^2 + x - 6 \ge 0$, then $x \le -3$ or $x \ge 2$.

### 40. Consecutive Integer Divisions
Prove or give a counterexample: The sum of any four consecutive integers is never divisible by four.

### 41. Rationality of Powers
Prove or give a counterexample: If $x$ is an irrational number, then $x^2$ is an irrational number.

### 42. Guided Structural Proof (Contrapositive Fill-in)
Consider the following fundamental theorem regarding integers:
$$\text{Theorem: For any integer } n, \text{ if } n^2 \text{ is an even number, then } n \text{ is an even number.}$$
A direct proof of this statement is somewhat messy because it requires taking the square root of $2k$. Instead, we can use our knowledge of propositional logic to make the proof much easier.

* **(a)** Let $P$ be "$n^2$ is an even number" and $Q be "n is an even number". Write the original theorem in formal logical language.
* **(b)** Restate the theorem in a logically equivalent way that is much easier to prove algebraically. What is the formal logical name for this specific restatement?
* **(c)** What is the name of the proof technique that uses this restatement? State the underlying logical tautology that makes this technique mathematically valid.
* **(d)** Fill in the blanks to complete the formal, rigorous proof of the theorem.

#### Formal Proof
We will prove this theorem by _______________________.  
Assume that $n$ is _______________________.  
By definition of this property, there exists an integer $k$ such that $n =$ _____________.  
Squaring both sides gives $n^2 = (\_\_\_\_\_\_)^2 = $ _______________________.  
We can factor out a 2 to rewrite this expression as $n^2 = 2(\_\_\_\_\_\_\_\_\_\_\_\_) + 1$.  
Since $k$ is an integer, the expression inside the parentheses is also an integer; let's call it $m$. Thus, $n^2 = 2m + 1$.  
By definition, this means that $n^2$ is _______________________.  
Therefore, we have successfully shown that if _______________________, then _______________________.  
Because this statement is logically equivalent to the original theorem, the proof is complete.

### 43. Multi-Scenario Case Parity
Prove that for any integer $n$, the expression $3n^2 + 5n + 2$ is an even integer.  
*Hint: Every integer must be either even or odd. Prove that the statement holds true in both possible scenarios.*

### 44. Nested Proof by Cases (Multiplicative Absolutes)
In Real Analysis, you often have to deal with multiple conditions simultaneously, requiring a "case within a case." Prove the following fundamental property of absolute values for any two real numbers $x$ and $y$:
$$|xy| = |x||y|$$
*Hint: Create your primary cases based on whether $x$ is positive or negative. Then, within each of those cases, create subcases based on whether $y$ is positive or negative. Do not forget to account for zero!*

### 45. Non-Constructive Existential Proof
An existential proof $(\exists x, P(x))$ usually requires us to find a specific, concrete example (a "constructive" proof). However, we can sometimes prove that an object exists without ever knowing exactly what it is! This is called an indirect or non-constructive proof. Consider the following fascinating theorem:
$$\text{Theorem: There exist irrational numbers } a \text{ and } b \text{ such that } a^b \text{ is a rational number.}$$
We will prove this theorem by analyzing the curious number $x = \sqrt{2}^{\sqrt{2}}$. (For this problem, you may assume it is a known fact that $\sqrt{2}$ is irrational).

* **(a)** Translate the theorem into a formal logical proposition.
* **(b)** In logic, a statement must be either true or false. Applying this basic principle to the rationality of the real number $x = \sqrt{2}^{\sqrt{2}}$, it must fall into one of two mutually exclusive categories. What are they?
* **(c) Case 1:** Assume $x = \sqrt{2}^{\sqrt{2}}$ is a rational number. If this case is true, explicitly state the values for $a$ and $b$ that satisfy the theorem, and explain why.
* **(d) Case 2:** Assume $x = \sqrt{2}^{\sqrt{2}}$ is an irrational number. In this scenario, let $a = x$ and let $b = \sqrt{2}$. Evaluate $a^b$ using the laws of exponents. If this case is true, explain why these specific choices for $a$ and $b$ satisfy the theorem.
* **(e)** Conclude the proof. Explain logically why the theorem is proven to be undeniably true, even though we still do not actually know which of the two cases holds in reality.

### 46. Analyzing Mathematical Conjectures
Consider the following mathematical conjecture:
$$\text{Conjecture: For every non-negative integer } n, \text{ the expression } n^2 + n + 41 \text{ produces a prime number.}$$
* **(a)** Test this conjecture by calculating the value of the expression for $n = 0, 1, 2,$ and $3$. Verify whether the results are prime numbers.
* **(b)** A student calculates the first 39 values (from $n = 0$ to $n = 39$) and discovers that every single result is indeed a prime number! Overjoyed, the student concludes that the universal statement must be mathematically true. What is the fundamental logical flaw in this reasoning?
* **(c)** Prove that the universal conjecture is actually False by finding a single counterexample.  
  *Hint: You do not need a calculator to brute-force this. Look at the expression and try to find an integer $n$ that obviously allows you to factor the expression into two integers greater than 1.*

### 47. Advanced Hybrid Proof Framework
Often, a single proof technique is not enough. You must build a primary logical framework and then use a secondary technique inside it. We will prove the following theorem using both Proof by Contradiction and Proof by Cases.
$$\text{Theorem: For every integer } n, \text{ the expression } n^2 + 2 \text{ is not divisible by 4.}$$

* **(a)** State the formal logical tautology that validates a Proof by Contradiction.
* **(b)** To begin the proof by contradiction, we must assume the negation of the theorem. Write down the precise mathematical assumption we must make to start the proof. (Translate the words "is divisible by 4" into an algebraic equation).
* **(c)** We now need to show that this assumption leads to an impossible scenario for absolutely every integer. To do this, establish two logical cases that exhaust all possible integers.
* **(d) Case 1:** Assume your first case is true. Substitute this into your algebraic assumption from part (b) and derive a mathematical contradiction. Explain why it is a contradiction.
* **(e) Case 2:** Assume your second case is true. Substitute this into your algebraic assumption from part (b) and derive a mathematical contradiction. Explain why it is a contradiction.
* **(f)** Write a concluding sentence explaining why deriving a contradiction in both cases successfully proves the original theorem.

### 48. Duplicate Problem Analysis
*(Note: This question in the source sheet duplicates the text of Question 46.)*  
Consider the following mathematical conjecture:
$$\text{Conjecture: For every non-negative integer } n, \text{ the expression } n^2 + n + 41 \text{ produces a prime number.}$$
* **(a)** Test this conjecture by calculating the value of the expression for $n = 0, 1, 2,$ and $3$. Verify whether the results are prime numbers.
* **(b)** A student calculates the first 39 values (from $n = 0$ to $n = 39$) and discovers that every single result is indeed a prime number! Overjoyed, the student concludes that the universal statement must be mathematically true. What is the fundamental logical flaw in this reasoning?
* **(c)** Prove that the universal conjecture is actually False by finding a single counterexample.

### 49. Algebraic Absolute Value Equations
Prove that there exists an integer $x$ such that $|4x - 5| = x + 4$. Is this integer unique? If $x$ was allowed to be a rational number, what could you conclude?

### 50. Piecewise Min/Max Identities
In Real Analysis, it is often necessary to express piecewise concepts using single algebraic formulas. Let $x$ and $y$ be real numbers. The maximum and minimum are formally defined as:
$$\max(x, y) = \begin{cases} x & \text{if } x \ge y \\ y & \text{if } x < y \end{cases} \quad \text{and} \quad \min(x, y) = \begin{cases} x & \text{if } x \le y \\ y & \text{if } x > y \end{cases}$$
Using a rigorous proof by cases, prove the following two analytical identities:
* **(a)** $\max(x, y) = \frac{x + y + |x - y|}{2}$
* **(b)** $\max(x, y) - \min(x, y) = |x - y|$
"""

with open("MAT1023_Problem_Sheet_1.md", "w") as f:
    f.write(md_content)

print("File successfully generated!")