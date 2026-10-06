---
title: "Error Theory - Laboratory Physics (PHY1921)"
course: "PHY1921"
tags:
  - physics
  - lab
  - error-theory
  - cheatsheet
---

# Error Theory & Measurement Analysis

> Reference: Based on Department of Physics, Faculty of Science, University of Peradeniya lab manual [[PHY1921/Error Theory 2026.pdf]].

---

## ⚡ Quick Reference Cheatsheet

### 1. Final Result Format: $x = (x_{\text{best}} \pm \Delta x) \text{ unit}$
1. **Error Sig Figs**:
   - If first sig fig of $\Delta x$ is **1** $\rightarrow$ keep **2 significant figures** (e.g., $0.0163 \to \mathbf{0.016}$).
   - If first sig fig of $\Delta x$ is **2–9** $\rightarrow$ keep **1 significant figure** (e.g., $0.0271 \to \mathbf{0.03}$).
2. **Value Decimal Places**:
   - Round $x_{\text{best}}$ to have the **exact same number of decimal places** as $\Delta x$.
   - *Example 1*: $4.1864 \pm 0.01325 \rightarrow \mathbf{4.186 \pm 0.013}$
   - *Example 2*: $4.1864 \pm 0.02714 \rightarrow \mathbf{4.19 \pm 0.03}$

### 2. Error Propagation Summary
Assuming independent variables with small fractional uncertainties ($\Delta x / x \ll 1$):

| Operation | Relation | Uncertainty Formula |
| :--- | :--- | :--- |
| **Scalar multiplication** | $Z = cX$ | $\Delta Z = c \Delta X$ |
| **Addition / Subtraction** | $Z = X \pm Y$ | $\Delta Z = \sqrt{(\Delta X)^2 + (\Delta Y)^2}$ |
| **Multiplication / Division** | $Z = X \times Y$ or $\frac{X}{Y}$ | $\frac{\Delta Z}{Z} = \sqrt{\left(\frac{\Delta X}{X}\right)^2 + \left(\frac{\Delta Y}{Y}\right)^2}$ |
| **Powers** | $Z = X^n$ | $\frac{\Delta Z}{Z} = n \left(\frac{\Delta X}{X}\right)$ |
| **Natural Log** | $Z = \ln X$ | $\Delta Z = \frac{\Delta X}{X}$ |
| **General Function** | $Z = f(X, Y, \dots)$ | $\Delta Z = \sqrt{\left(\frac{\partial f}{\partial X} \Delta X\right)^2 + \left(\frac{\partial f}{\partial Y} \Delta Y\right)^2 + \dots}$ |

---

## 1. Fundamentals of Error & Uncertainty

- **No measurement is exact**: Physical quantities always carry uncertainty.
- **Misconception**: Error is *not* simply $|\text{measured} - \text{standard}|$. Standard values themselves are experimentally derived and have errors.
- **Definition**: Error is the difference between the true value (which is fundamentally unknowable) and the measured value. Thus, we perform **error estimation**.
- **Complete Measurement**: Always specify:
  $$\text{Measurement} = (\text{Numerical Value} \pm \text{Uncertainty}) \times 10^k \text{ Unit}$$
  *Example*: $(54.5 \pm 0.1)\text{ cm}$ or $(5.45 \pm 0.01) \times 10^{-1}\text{ m}$.

### Three Types of Limitations
1. **Instrumental limitations**: Limited by instrument resolution / least count.
2. **Systematic errors & blunders**: Constant directional offset (e.g., zero-error on a balance or micrometer).
   - *Do not average out*. Must be identified and corrected/eliminated.
3. **Random errors**: Environmental fluctuations, human reaction times.
   - Affects *precision*. Reduced by repeating measurements and averaging.

---

## 2. Significant Figures (SF) & Operations

### Determining Significant Figures
- **Rule 1**: The leftmost non-zero digit is the **most significant**.
- **Rule 2**: 
  - Without a decimal point: rightmost non-zero digit is least significant ($3060700 \rightarrow 5$ SF, unless scientific notation says otherwise).
  - With a decimal point: rightmost digit is least significant, even if zero ($11.020 \rightarrow 5$ SF).
- **Rule 3**: All digits between most and least significant are significant.

### Mathematical Rules with SF

| Operation | Governing Rule | Example |
| :--- | :--- | :--- |
| **$\times$ and $\div$** | Keep the **fewest significant figures** of the inputs | $23.4 \times 18.2 = 425.88 \rightarrow \mathbf{426}$ (3 SF) |
| **$+$ and $-$** | Keep the **fewest decimal places** of the inputs | $88.932 + 4.24 = 93.172 \rightarrow \mathbf{93.17}$ (2 d.p.) |
| **$\log_{10}$ / $\ln$** | Number of **decimal places** of result = **SF of input** (the integer part is just the scale exponent) | $\log(24.3) = 1.3856\dots \rightarrow \mathbf{1.386}$ (3 d.p.)<br>$\ln(0.068) = -2.6882\dots \rightarrow \mathbf{-2.69}$ (2 d.p.) |
| **Antilog / $e^x$** | Number of **SF** in result = **decimal places** of exponent | $\text{antilog}(23.32) = 10^{23.32} \rightarrow \mathbf{2.1 \times 10^{23}}$ (2 SF)<br>$e^{-1.873} \rightarrow \mathbf{0.154}$ (3 SF) |
| **Angles ($\deg \to \text{rad}$)** | SF in radians = SF of the angle measured in degrees | $38^\circ 46' \text{ (4 SF)} \rightarrow \frac{\pi \times 38^\circ 46'}{180^\circ} = \mathbf{0.6767}\text{ rad}$ (4 SF) |

---

## 3. Statistical Error Estimation (Repeated Measurements)

When human reaction time or environmental fluctuations dominate (e.g., stopwatch timing):

### 1. Mean (Best Estimate)
$$\bar{x} = \frac{1}{N} \sum_{i=1}^N x_i$$

### 2. Sample Standard Deviation ($s_x$)
Quantifies the spread/scatter of an individual single measurement:
$$s_x = \sqrt{\frac{1}{N-1} \sum_{i=1}^N (x_i - \bar{x})^2}$$

### 3. Standard Error of the Mean ($\Delta x$)
Uncertainty of the mean value $\bar{x}$:
$$\Delta x = \frac{s_x}{\sqrt{N}} = \sqrt{\frac{1}{N(N-1)} \sum_{i=1}^N (x_i - \bar{x})^2}$$

> [!important] Final Quoted Error vs. Instrument Least Count
> Always report the **maximum possible error**:
> - If $\Delta x_{\text{stat}} < \text{Least Count} \implies \text{Quoted Error} = \textbf{Least Count}$
> - If $\Delta x_{\text{stat}} > \text{Least Count} \implies \text{Quoted Error} = \mathbf{\Delta x_{\text{stat}}}$
> 
> *Example*: Micrometer diameter measurements give mean $d = 1.413\text{ mm}$, $\Delta d_{\text{stat}} = 0.005\text{ mm}$. Since least count is $0.01\text{ mm}$, report:  
> $d = \mathbf{(1.41 \pm 0.01) \times 10^{-3}\text{ m}}$.

---

## 4. Error Propagation in Calculations

- **Fractional (Relative) Error**: $\frac{\Delta x}{x}$
- **Percentage Error**: $\frac{\Delta x}{x} \times 100\%$

### Independent Variables (Quadrature)
1. **Sum / Difference**: $Z = A + B - C$
   $$\Delta Z = \sqrt{(\Delta A)^2 + (\Delta B)^2 + (\Delta C)^2}$$

2. **Product / Quotient**: $Z = \frac{A^a \cdot B^b}{C^c}$
   $$\frac{\Delta Z}{Z} = \sqrt{\left(a \frac{\Delta A}{A}\right)^2 + \left(b \frac{\Delta B}{B}\right)^2 + \left(c \frac{\Delta C}{C}\right)^2}$$

3. **General Multivariable Relation**: $Z = f(x_1, x_2, \dots, x_n)$
   $$\Delta Z = \sqrt{\sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \Delta x_i \right)^2}$$

---

## 5. Linear Graphs & Least Squares Analysis

For a straight-line fit: $y = mx + c$

### Method A: Simplified Centroid Method (Standard Lab Practice)
1. **Calculate Centroid**:
   $$\bar{x} = \frac{1}{N} \sum_{i=1}^N x_i, \quad \bar{y} = \frac{1}{N} \sum_{i=1}^N y_i$$
2. **Draw Best-Fit Line**: Force the line to pass through the centroid $(\bar{x}, \bar{y})$.
3. **Extract Best Values**: Read gradient $m$ and intercept $c$ from this line.
4. **Individual Slopes & Intercepts for each point $(x_i, y_i)$**:
   $$m_i = \frac{y_i - \bar{y}}{x_i - \bar{x}}, \quad c_i = y_i - m_i x_i$$
5. **Calculate Uncertainties**:
   $$\Delta m = \sqrt{\frac{1}{N(N-1)} \sum_{i=1}^N (m_i - m)^2}$$
   $$\Delta c = \sqrt{\frac{1}{N(N-1)} \sum_{i=1}^N (c_i - c)^2}$$

---

### Method B: Rigorous Least Squares Formulas
Assuming uniform random Gaussian errors in $y$ only:
$$\Delta = N \sum x_i^2 - \left(\sum x_i\right)^2$$
$$m = \frac{1}{\Delta}\left[ N \sum x_i y_i - \left(\sum x_i\right)\left(\sum y_i\right) \right]$$
$$c = \frac{1}{\Delta}\left[ \left(\sum y_i\right)\left(\sum x_i^2\right) - \left(\sum x_i\right)\left(\sum x_i y_i\right) \right]$$

Uncertainties:
$$\Delta y = \sqrt{\frac{1}{N}\sum (y_i - m x_i - c)^2}$$
$$\Delta m = \Delta y \sqrt{\frac{N}{\Delta}}, \quad \Delta c = \Delta y \sqrt{\frac{\sum x_i^2}{\Delta}}$$

---

## 6. How to State Your Final Result (The 2-Rule Algorithm)

When presenting final calculated parameters:
```
              Calculate calculated value x and error Δx
                               │
                               ▼
               Round Δx to 2 significant figures
                               │
            ┌──────────────────┴──────────────────┐
            ▼                                     ▼
   First digit is '1'                    First digit is '2' - '9'
            │                                     │
   Keep 2 Significant Figures             Round to 1 Significant Figure
            │                                     │
            └──────────────────┬──────────────────┘
                               │
                               ▼
        Match decimal places of x to the decimal places of Δx
                               │
                               ▼
               Quote as: (x ± Δx) [Unit]
```

### Examples
- **Example A**: Raw $x = 4.1864\text{ J}$, raw $\Delta x = 0.01325\text{ J}$
  1. $\Delta x \approx 0.013$ (Starts with `1` $\rightarrow$ keep 2 sig figs: $0.013$, 3 d.p.)
  2. Round $x$ to 3 d.p.: $4.1864 \to 4.186$
  3. **Final Result**: $\mathbf{4.186 \pm 0.013\text{ J}}$

- **Example B**: Raw $x = 4.1864\text{ J}$, raw $\Delta x = 0.02714\text{ J}$
  1. $\Delta x \approx 0.027$ (Starts with `2` $\rightarrow$ round to 1 sig fig: $0.03$, 2 d.p.)
  2. Round $x$ to 2 d.p.: $4.1864 \to 4.19$
  3. **Final Result**: $\mathbf{4.19 \pm 0.03\text{ J}}$
