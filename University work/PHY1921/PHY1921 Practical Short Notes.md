---
title: "PHY1921 - Elementary Laboratory II Practical Short Notes"
course: "PHY1921"
academic_year: "2024/2025"
institution: "Department of Physics, Faculty of Science, University of Peradeniya"
tags:
  - physics
  - lab
  - practicals
  - cheatsheet
  - university-of-peradeniya
---

<style>
@media print {
  /* Prevent table and formula overflow on PDF export */
  table {
    font-size: 8pt !important;
    width: 100% !important;
    table-layout: fixed !important;
    border-collapse: collapse !important;
    margin: 8px 0 !important;
  }
  th, td {
    padding: 4px 6px !important;
    word-break: break-word !important;
    overflow-wrap: break-word !important;
    line-height: 1.3 !important;
    vertical-align: top !important;
  }
  th {
    background-color: #f1f5f9 !important;
    -webkit-print-color-adjust: exact !important;
    print-color-adjust: exact !important;
  }
  h1, h2, h3 {
    page-break-after: avoid !important;
    break-after: avoid !important;
  }
}
</style>

# PHY1921 — Elementary Laboratory II: Complete Practical Short Notes

> **Source Reference**: Based on the 12 laboratory manuals of the Department of Physics, Faculty of Science, University of Peradeniya.  
> Cross-reference with: [[PHY1921/Error Theory.md]] for measurement uncertainties, rounding rules, and propagation formulas.

---

## 📑 Master Experiment Matrix

| Experiment | Target Quantity & Governing Relation | Graph ($y$ vs $x$) | Parameter Extraction |
| :--- | :--- | :--- | :--- |
| **01. [[PHY1921/01- Meter Bridge.pdf\|Meter Bridge]]** | End corrections $e_1, e_2$; Temp coeff $\alpha$<br>$R_T = (R_0 \alpha) T + R_0$ | $R_T$ vs $T$ (°C) | $m = R_0 \alpha$, $c = R_0$<br>$\alpha = \frac{m}{c}\;(\text{°C}^{-1})$ |
| **02. [[PHY1921/02 - Potentiometer.pdf\|Potentiometer]]** | EMF ratio $E_1/E_2$; Internal resistance $r_1$<br>$\frac{1}{L} = \left(\frac{k r_1}{E_1}\right)\frac{1}{R} + \frac{k}{E_1}$ | $\frac{1}{L}$ vs $\frac{1}{R}\;(\Omega^{-1})$ | $m = \frac{k r_1}{E_1}$, $c = \frac{k}{E_1}$<br>$r_1 = \frac{m}{c}\;(\Omega)$ |
| **03. [[PHY1921/03 - Magnetometer.pdf\|Magnetometer]]** | Earth's $B_0$; Magnetic moment $M$; $M_1/M_2$<br>$\frac{M}{B_0} = \frac{(d^2-l^2)^2 \tan\theta}{2d(\mu_0/4\pi)}$<br>$M B_0 = \frac{4\pi^2 I}{T^2}$ | $\theta$ vs $d$ (Tan-A)<br>Oscillation period $T$ | $M = \sqrt{(M/B_0)(M B_0)}$<br>$B_0 = \sqrt{\frac{M B_0}{M/B_0}}$<br>$\frac{M_1}{M_2} = \frac{T_2^2 + T_1^2}{T_2^2 - T_1^2}$ |
| **04. [[PHY1921/04- Properties of Matter I.pdf\|Properties of Matter I]]** | Soap surface tension $T$; Air viscosity $\eta$<br>• Part A: $h = \left(\frac{4T}{\rho g}\right)\frac{1}{R}$<br>• Part B: $R^4 = -\left(\frac{T r^4}{2\eta l}\right) t + R_0^4$ | • Part A: $h$ vs $\frac{1}{R}$<br>• Part B: $R^4$ vs $t$ (s) | • $T = \frac{m \rho g}{4}\;(\text{N/m})$<br>• $\eta = \frac{T r^4}{2 \lvert m \rvert l}\;(\text{Pa}\cdot\text{s})$ |
| **05. [[PHY1921/05- Capillary Rise Method.pdf\|Capillary Rise Method]]** | Surface tension of water $T$<br>$\frac{h}{r} = \left(\frac{2T}{\rho g}\right)\frac{1}{r^2} - \frac{1}{3}$ | $\frac{h}{r}$ vs $\frac{1}{r^2}\;(\text{m}^{-2})$ | $m = \frac{2T}{\rho g} \implies T = \frac{m \rho g}{2}$<br>Intercept $c \approx -1/3$ |
| **06. [[PHY1921/06- Youngs Modulus of a Copper wire.pdf\|Young's Modulus (Cu Wire)]]** | Young's Modulus $Y$; Clamping tension $F_0$<br>$\frac{m}{\varepsilon} = \left(\frac{Y A}{g l_0^3}\right)\varepsilon^2 + \frac{2 F_0}{g l_0}$ | $\frac{m}{\varepsilon}$ vs $\varepsilon^2$ | $m = \frac{Y A}{g l_0^3} \implies Y = \frac{m g l_0^3}{A}$<br>$c = \frac{2 F_0}{g l_0} \implies F_0 = \frac{c g l_0}{2}$ |
| **07. [[PHY1921/07 - Newtons Law of Cooling.pdf\|Newton's Law of Cooling]]** | Verification of Newton's cooling law<br>$\lvert\frac{d\theta}{dt}\rvert = k (\theta - \theta_0)$ | $\lvert\frac{d\theta}{dt}\rvert$ vs $(\theta - \theta_0)$ | Linear through $(0,0)$ verifies law;<br>$k = \frac{\varepsilon A}{m_c s_c + m_w s_w}$ |
| **08. [[PHY1921/08 - Wheatstone Bridge.pdf\|Wheatstone Bridge (Stefan's Law)]]** | Filament temp $T$; Stefan's Law ($P \propto T^4$)<br>$\ln(I^2 R) = 4\ln T + \ln(\varepsilon A \sigma)$ | $\ln(I^2 R)$ vs $\ln T$ ($T$ in K) | Gradient $m \approx 4$ verifies Stefan-Boltzmann $T^4$ relation |
| **09. [[PHY1921/09 -Tangent Galvanometer.pdf\|Tangent Galvanometer]]** | Earth's field $B_0$; Coil resistance $G$; Field $B$<br>$\cot\theta = \left(\frac{2r B_0}{\mu_0 n E}\right) R + \left(\frac{2r B_0 G}{\mu_0 n E}\right)$ | $\cot\theta$ vs $R\;(\Omega)$ | $m = \frac{2r B_0}{\mu_0 n E} \implies B_0 = \frac{m \mu_0 n E}{2r}$<br>$c = \frac{2r B_0 G}{\mu_0 n E} \implies G = \frac{c}{m}$ |
| **10. [[PHY1921/10 - Capacitor Charging and Discharging.pdf\|Capacitor Charge/Discharge]]** | Capacitance $C$; Internal resistance; $\tau = RC$<br>• 10A: $\ln(I_0 / I) = \frac{t}{R_{eff}C}$<br>• 10B: $V(t) = A e^{-C_{fit}t} + B$ | • 10A: $\ln(I_0/I)$ vs $t$<br>• 10B: $V$ vs $t$ (exp fit) | • $C = \frac{Q_{tot}}{V} = \frac{\int I dt}{V}$<br>• $\tau_{exp} = \frac{1}{C_{fit}} \approx RC$ |
| **11. [[PHY1921/11 - Melting Point of Wax.pdf\|Melting Point of Wax]]** | Melting/Freezing point $T_m$<br>Latent heat plateau: $\frac{d\theta}{dt} = 0$ | Temperature $\theta$ vs Time $t$ | Flat horizontal arrest plateau temperature gives $T_m$ |
| **12. [[PHY1921/12 - Properties of Matter II.pdf\|Properties of Matter II]]** | Viscosity of water $\eta$ (Poiseuille flow)<br>$\frac{V}{t} = \left(\frac{\pi a^4 \rho g}{8 \eta l}\right) h$ | $\frac{V}{t}$ vs $h$ (pressure head) | $m = \frac{\pi a^4 \rho g}{8 \eta l} \implies \eta = \frac{\pi a^4 \rho g}{8 l \cdot m}$ |
---

## 01. Meter Bridge
Manual: [[PHY1921/01- Meter Bridge.pdf]]

### Aims
1. Determine the end corrections ($e_1, e_2$) of the meter bridge wire.
2. Determine the first-order temperature coefficient of resistance ($\alpha$) of a given wire.

### Theory & Derivations
- **Wheatstone Bridge Principle**: At balance condition, no current flows through the galvanometer ($I_g = 0$):
  $$\frac{P}{Q} = \frac{R_1}{R_2}$$
- **End Corrections ($e_1, e_2$)**: Copper contact strips and soldering at ends $A$ ($0\text{ cm}$) and $B$ ($100\text{ cm}$) introduce small non-zero resistances equivalent to wire lengths $e_1$ and $e_2$.
- When standard resistors $P$ and $Q$ are in the left and right gaps respectively:
  $$\frac{P}{Q} = \frac{l_1 + e_1}{(100 - l_1) + e_2} \implies \frac{P}{P+Q} = \frac{l_1 + e_1}{100 + e_1 + e_2} \quad \text{--- (1)}$$
- Interchanging $P$ and $Q$ in the gaps (new balance length $l_2$ from end A):
  $$\frac{Q}{P} = \frac{l_2 + e_1}{(100 - l_2) + e_2} \implies \frac{Q}{P+Q} = \frac{l_2 + e_1}{100 + e_1 + e_2} \quad \text{--- (2)}$$
- Dividing (1) by (2):
  $$\frac{P}{Q} = \frac{l_1 + e_1}{l_2 + e_1} \implies P l_2 + P e_1 = Q l_1 + Q e_1 \implies (Q - P) e_1 = P l_2 - Q l_1$$
  $$e_1 = \frac{P l_2 - Q l_1}{Q - P}$$
  Similarly for end $B$:
  $$e_2 = \frac{Q (100 - l_2) - P (100 - l_1)}{P - Q}$$

- **Temperature Coefficient of Resistance ($\alpha$)**:
  The wire wound on the test tube is placed in a heated/cooled bath at temperature $T$ (°C).
  With standard resistor $Q$ in the right gap and wire resistance $R_T$ in the left gap:
  $$R_T = Q \left[\frac{L + e_1}{100 - L + e_2}\right]$$
  Assuming linear temperature dependence:
  $$R_T = R_0 (1 + \alpha T) = (R_0 \alpha) T + R_0$$

### Graphical Analysis
- **Plot**: $R_T$ ($\Omega$) on the Y-axis vs $T$ (°C) on the X-axis.
- **Slope**: $m = R_0 \alpha$
- **Y-intercept**: $c = R_0$
- **Extraction**:
  $$\alpha = \frac{\text{Slope}}{\text{Intercept}} = \frac{m}{c} \quad (\text{°C}^{-1})$$

### Viva Questions & Crucial Precautions
1. **Why is a high resistance $R'$ ($5000\,\Omega$) connected in series with the galvanometer initially?**
   - It limits the current flowing through the sensitive galvanometer to prevent coil burn-out or mechanical damage to the pointer when the jockey is far from the null point.
2. **How to find rough vs exact balance point?**
   - *Rough balance*: Keep key $K_2$ open (protective resistor $R'$ active) and tap the jockey lightly along the wire.
   - *Exact balance*: Once near null deflection, close key $K_2$ (shorting $R'$) to achieve maximum galvanometer sensitivity.
3. **Can $e_1$ and $e_2$ be determined without interchanging $P$ and $Q$?**
   - No. A single balance length yields one equation with two unknown variables ($e_1$ and $e_2$). Interchanging $P$ and $Q$ provides a second linearly independent equation.
4. **Why should the jockey never be scraped along the wire?**
   - Scraping cuts into the wire and deforms its cross-section non-uniformly, which destroys the fundamental assumption of constant resistance per unit length. Always tap gently.

---

## 02. Potentiometer
Manual: [[PHY1921/02 - Potentiometer.pdf]]

### Aims
1. Compare the electromotive forces (EMFs) of a Leclanché cell ($E_1$) and a Daniell cell ($E_2$).
2. Determine the internal resistance ($r_1$) of a Leclanché cell.

### Theory & Derivations
- **Working Principle**: The potentiometer measures potential differences without drawing any current from the cell under test at the balance point, yielding the true open-circuit EMF.
- For a wire of length $L_{tot}$ having potential gradient $k = \frac{V_{wire}}{L_{tot}}$:
- **Part A (Comparing EMFs)**:
  - Connecting cell $E_1$ via two-way switch: $E_1 = k L_1$
  - Connecting cell $E_2$ via two-way switch: $E_2 = k L_2$
  $$\frac{E_1}{E_2} = \frac{L_1}{L_2}$$

- **Part B (Internal Resistance $r_1$)**:
  - Cell $E_1$ (internal resistance $r_1$) is shunted by an external resistance box $R$.
  - Current drawn from the cell: $I = \frac{E_1}{R + r_1}$.
  - Terminal potential difference $V_{AB}$:
    $$V_{AB} = I R = \frac{E_1 R}{R + r_1}$$
  - At the balance point on the potentiometer wire:
    $$V_{AB} = k L \implies k L = \frac{E_1 R}{R + r_1}$$
  - Taking the reciprocal:
    $$\frac{1}{k L} = \frac{R + r_1}{E_1 R} = \frac{1}{E_1} + \frac{r_1}{E_1}\frac{1}{R}$$
    $$\frac{1}{L} = \left(\frac{k r_1}{E_1}\right) \frac{1}{R} + \frac{k}{E_1}$$

### Graphical Analysis
- **Plot**: $\frac{1}{L}$ ($\text{cm}^{-1}$) on the Y-axis vs $\frac{1}{R}$ ($\Omega^{-1}$) on the X-axis.
- **Slope**: $m = \frac{k r_1}{E_1}$
- **Y-intercept**: $c = \frac{k}{E_1} = \frac{1}{L_0}$ (where $L_0$ is the open-circuit balance length when $R \to \infty$).
- **Extraction**:
  $$r_1 = \frac{\text{Slope}}{\text{Intercept}} = \frac{m}{c} \quad (\Omega)$$

### Viva Questions & Crucial Precautions
1. **Why is a potentiometer preferred over a voltmeter for measuring EMF?**
   - A voltmeter draws current from the cell, measuring terminal voltage $V = E - I r < E$. A potentiometer draws *zero current* at the null point, measuring the exact, true EMF.
2. **What conditions must be satisfied for a balance point to exist on the wire?**
   - The driver power supply EMF ($E$) must be strictly greater than the EMF of any cell being tested ($E > E_1, E_2$).
   - The positive terminals of the driver battery and the test cells must all be connected to the same zero-end of the potentiometer wire.
3. **What happens if the driver battery runs down during the experiment?**
   - Potential gradient $k$ drifts, causing inconsistent balance lengths. A steady lead-acid accumulator or regulated DC power supply should be used.

---

## 03. Magnetometer
Manual: [[PHY1921/03 - Magnetometer.pdf]]

### Aims
1. Determine the horizontal component of the Earth's magnetic field ($B_0$) and magnetic moment ($M$) of a bar magnet using deflection and vibration magnetometers.
2. Compare the magnetic moments ($M_1 / M_2$) of two bar magnets using a vibration magnetometer.

### Theory & Derivations

#### 1. Deflection Magnetometer (Tan-A / Gauss End-On Position)
- Meter ruler is oriented perpendicular to the magnetic meridian (East-West direction).
- Magnetic field $B$ produced along the axial line of a bar magnet of length $2l$ at distance $d$ from its center:
  $$B = \frac{\mu_0}{4\pi} \frac{2 M d}{(d^2 - l^2)^2}$$
  *(Effective magnetic length $2l = \frac{5}{6} y$, where $y$ is geometric length).*
- Tangent Law: $B = B_0 \tan\theta$
  $$\frac{M}{B_0} = \frac{(d^2 - l^2)^2 \tan\theta}{2 d (\mu_0 / 4\pi)} \quad \text{--- (1)}$$

#### 2. Vibration Magnetometer
- Magnet suspended horizontally in Earth's field $B_0$ oscillates with period $T$:
  $$T = 2\pi \sqrt{\frac{I}{M B_0}} \implies M B_0 = \frac{4\pi^2 I}{T^2} \quad \text{--- (2)}$$
  where moment of inertia $I$ for a rectangular bar magnet of mass $m$, length $y$, and width $x$ is:
  $$I = \frac{m}{12}(y^2 + x^2)$$
- Combining (1) and (2):
  $$M = \sqrt{\left(\frac{M}{B_0}\right) (M B_0)} = \frac{2\pi}{T} (d^2 - l^2) \sqrt{\frac{I \tan\theta}{2d (\mu_0 / 4\pi)}}$$
  $$B_0 = \sqrt{\frac{M B_0}{(M / B_0)}} = \frac{2\pi}{T (d^2 - l^2)} \sqrt{\frac{2d (\mu_0 / 4\pi) I}{\tan\theta}}$$

#### 3. Comparison of Two Magnets (Sum & Difference Method)
- **Similar poles together**: $T_1 = 2\pi \sqrt{\frac{I_1 + I_2}{(M_1 + M_2) B_0}}$
- **Opposite poles together**: $T_2 = 2\pi \sqrt{\frac{I_1 + I_2}{|M_1 - M_2| B_0}}$
  $$\frac{M_1}{M_2} = \frac{T_2^2 + T_1^2}{T_2^2 - T_1^2}$$
- **Perpendicular configuration**: $T_3 = 2\pi \sqrt{\frac{I_1 + I_2}{B_0 \sqrt{M_1^2 + M_2^2}}}$, satisfying:
  $$\frac{2}{T_3^4} = \frac{1}{T_1^4} + \frac{1}{T_2^4}$$

### Viva Questions & Crucial Precautions
1. **How many pointer readings are taken for each distance $d$?**
   - **8 readings total**: For a given distance $d$ on one arm, read both ends of the pointer (2 readings). Reverse the magnet end-for-end ($180^\circ$) to eliminate magnetic asymmetry (2 readings). Repeat on the other side of the magnetometer (4 readings). Averaging all 8 eliminates pointer eccentricity and center misalignment errors.
2. **What is the ideal range of deflection $\theta$?**
   - Between $30^\circ$ and $60^\circ$ (ideally $45^\circ$). Since $\Delta \theta / \theta$ error propagation depends on $\frac{2 d\theta}{\sin(2\theta)}$, fractional error is minimized at $\theta = 45^\circ$.
3. **If a rectangular magnet is replaced by a cylindrical magnet of same mass, length, and diameter equal to width:**
   - Moment of inertia changes from $I = \frac{m}{12}(y^2 + x^2)$ to $I = m\left(\frac{y^2}{12} + \frac{r^2}{4}\right) = m\left(\frac{y^2}{12} + \frac{x^2}{16}\right)$. Since $\frac{1}{16} < \frac{1}{12}$, $I$ decreases slightly, leading to a slightly shorter oscillation period $T$.

---

## 04. Properties of Matter I
Manual: [[PHY1921/04- Properties of Matter I.pdf]]

### Aims
1. Determine the surface tension ($T$) of a soap solution using **Ferguson’s method**.
2. Determine the coefficient of viscosity ($\eta$) of air.

### Theory & Derivations

#### Part A: Surface Tension of Soap Solution (Ferguson's Method)
- A soap bubble has **two liquid-air surfaces** (inner and outer).
- Excess pressure inside a bubble of radius $R$:
  $$\Delta P = P_1 - P_2 = \frac{4T}{R} = \frac{8T}{d}$$
- Measured via a liquid manometer of density $\rho$:
  $$\Delta P = h \rho g$$
  $$h \rho g = \frac{4T}{R} \implies h = \left(\frac{4T}{\rho g}\right) \frac{1}{R}$$
- **Optical Projection**: Bubble diameter $d$ is projected onto a screen using a convex lens of magnification $M = \frac{v}{u}$:
  $$M = \frac{D}{d} = \frac{v}{u} \implies d = D \left(\frac{u}{v}\right) \implies R = \frac{d}{2}$$
  where $D = \frac{D_h + D_v}{2}$ (average of horizontal and vertical image diameters).

#### Part B: Viscosity of Air
- When the bubble deflates through a capillary tube (radius $r$, length $l$), air escapes under Poiseuille flow:
  $$\frac{dV}{dt} = -\frac{\pi r^4 P}{8 \eta l}$$
- With bubble volume $V = \frac{4}{3} \pi R^3 \implies \frac{dV}{dt} = 4\pi R^2 \frac{dR}{dt}$, and driving pressure $P = \frac{4T}{R}$:
  $$4\pi R^2 \frac{dR}{dt} = -\frac{\pi r^4}{8 \eta l}\left(\frac{4T}{R}\right) \implies R^3 dR = -\frac{T r^4}{8 \eta l} dt$$
- Integrating from $R = R_0$ at $t = 0$ to $R$ at time $t$:
  $$\int_{R_0}^R R^3 dR = -\frac{T r^4}{8 \eta l} \int_0^t dt \implies \frac{R^4 - R_0^4}{4} = -\frac{T r^4}{8 \eta l} t$$
  $$R^4 = -\left(\frac{T r^4}{2 \eta l}\right) t + R_0^4$$

### Graphical Analysis
- **Part A (Surface Tension)**:
  - Plot: $h$ (m) vs $\frac{1}{R}$ ($\text{m}^{-1}$).
  - Slope: $m = \frac{4T}{\rho g} \implies T = \frac{m \rho g}{4} \quad (\text{N/m})$.
- **Part B (Viscosity of Air)**:
  - Plot: $R^4$ ($\text{m}^4$) on Y-axis vs $t$ (s) on X-axis.
  - Slope: $m = -\frac{T r^4}{2 \eta l}$
  - Extraction: $\eta = \frac{T r^4}{2 |m| l} \quad (\text{Pa}\cdot\text{s})$.

### Viva Questions & Crucial Precautions
1. **Purpose of ground glass behind the light source?**
   - Diffuses light evenly to create uniform background illumination and prevent bulb filament glare from distorting the projected bubble boundary.
2. **Desirable properties of manometer liquid:**
   - Low density (to yield a large, sensitive height difference $h$), low vapor pressure (minimal evaporation), and low viscosity.
3. **Why average $D_h$ and $D_v$?**
   - Gravity causes the bubble to sag slightly into an oblate spheroid. Averaging orthogonal axes provides the best equivalent spherical radius.

---

## 05. Capillary Rise Method
Manual: [[PHY1921/05- Capillary Rise Method.pdf]]

### Aim
Determine the surface tension ($T$) of water using the capillary rise method across five capillary tubes of different bore diameters.

### Theory & Derivation
- When a clean glass capillary tube of internal radius $r$ is dipped vertically into water:
  - Upward surface tension force around circumference:
    $$F_{up} = 2\pi r T \cos\theta \approx 2\pi r T \quad (\text{for clean glass and pure water, } \theta \approx 0^\circ)$$
  - Downward weight of water column, including the curved hemispherical meniscus volume:
    $$V_{column} = \pi r^2 h + \left(\pi r^2 \cdot r - \frac{2}{3}\pi r^3\right) = \pi r^2 \left(h + \frac{r}{3}\right)$$
    $$W = m g = \pi r^2 \left(h + \frac{r}{3}\right) \rho g$$
- At static equilibrium ($F_{up} = W$):
  $$2\pi r T = \pi r^2 \left(h + \frac{r}{3}\right) \rho g \implies 2T = r \left(h + \frac{r}{3}\right) \rho g$$
- Rearranging:
  $$\frac{h}{r} + \frac{1}{3} = \frac{2T}{\rho g r^2} \implies \frac{h}{r} = \left(\frac{2T}{\rho g}\right) \frac{1}{r^2} - \frac{1}{3}$$

### Graphical Analysis
- **Plot**: $\frac{h}{r}$ (dimensionless) on Y-axis vs $\frac{1}{r^2}$ ($\text{m}^{-2}$) on X-axis.
- **Gradient**: $G = \frac{2T}{\rho g}$
- **Extraction**:
  $$T = \frac{G \rho g}{2} \quad (\text{N/m})$$
- **Theoretical Y-intercept**: $-1/3 \approx -0.333$ (confirms the meniscus volume correction term).

### Viva Questions & Crucial Precautions
1. **Cleaning protocol before starting:**
   - Capillary tubes must be washed with chromic acid / caustic soda, rinsed thoroughly with distilled water, and verified to be grease-free. Grease dramatically alters contact angle $\theta$ and lowers apparent surface tension.
2. **Measurements with Travelling Microscope:**
   - *Height $h$*: Focus on the lowest point of the concave meniscus inside the tube ($y_1$); focus on the tip of the pointer touching the liquid surface in the beaker ($y_2$); $h = y_1 - y_2$.
   - *Bore radius $r$*: Measured at the tip of the tube by focusing on the circular bore and recording two orthogonal diameters ($d_1, d_2$) using crosshairs: $r = \frac{d_1 + d_2}{4}$.

---

## 06. Young's Modulus of a Copper Wire
Manual: [[PHY1921/06- Youngs Modulus of a Copper wire.pdf]]

### Aim
Determine Young's Modulus ($Y$) of a copper wire by central loading of a horizontally clamped wire.

### Theory & Derivations
- A copper wire of initial span $2l_0$ and initial tension $F_0$ is clamped horizontally between two rigid supports.
- A central load $W = mg$ causes a vertical sag (depression) $\varepsilon$.
- Half-length after stretching:
  $$l = \sqrt{l_0^2 + \varepsilon^2} = l_0 \left(1 + \frac{\varepsilon^2}{l_0^2}\right)^{1/2} \approx l_0 \left(1 + \frac{\varepsilon^2}{2l_0^2}\right)$$
- Extension of each half: $\Delta l = l - l_0 = \frac{\varepsilon^2}{2l_0} \implies \text{Strain} = \frac{\Delta l}{l_0} = \frac{\varepsilon^2}{2l_0^2}$.
- From equilibrium of forces at center:
  $$2 F \sin\theta = mg \implies 2 F \left(\frac{\varepsilon}{l_0}\right) = mg \implies F = \frac{mg l_0}{2\varepsilon}$$
- Change in tension: $\Delta F = F - F_0 = \frac{mg l_0}{2\varepsilon} - F_0$.
- Young's Modulus:
  $$Y = \frac{\text{Stress}}{\text{Strain}} = \frac{\frac{mg l_0 / (2\varepsilon) - F_0}{A}}{\frac{\varepsilon^2}{2l_0^2}} = \frac{\left[\frac{mg l_0}{2\varepsilon} - F_0\right] 2l_0^2}{A \varepsilon^2}$$
- Rearranging:
  $$Y A \varepsilon^3 = m g l_0^3 - 2 F_0 l_0^2 \varepsilon \implies \frac{m}{\varepsilon} = \left(\frac{Y A}{g l_0^3}\right) \varepsilon^2 + \frac{2 F_0}{g l_0}$$

### Graphical Analysis
- **Plot**: $\frac{m}{\varepsilon}$ ($\text{kg/m}$) on Y-axis vs $\varepsilon^2$ ($\text{m}^2$) on X-axis.
- **Gradient**: $G = \frac{Y A}{g l_0^3} \implies Y = \frac{G g l_0^3}{A} \quad (\text{N/m}^2 \text{ or Pa})$, where $A = \frac{\pi d^2}{4}$.
- **Y-intercept**: $c = \frac{2 F_0}{g l_0} \implies F_0 = \frac{c g l_0}{2} \quad (\text{N})$ *(yields initial clamping tension)*.

### Viva Questions & Crucial Precautions
1. **Why measure both loading and unloading?**
   - Eliminates elastic hysteresis (elastic after-effect) where the wire does not instantly return to its equilibrium position upon load removal. The average of loading and unloading values is used.
2. **Measurement instruments:**
   - Central sag $\varepsilon$: Cathetometer (precision vertical travelling telescope).
   - Wire diameter $d$: Micrometer screw gauge (measured at multiple positions in mutually perpendicular directions; zero error corrected).
   - Half-span $l_0$: Meter ruler.
3. **Safety:**
   - Always wear safety goggles; thin wires under tension can snap unexpectedly.

---

## 07. Newton's Law of Cooling
Manual: [[PHY1921/07 - Newtons Law of Cooling.pdf]]

### Aim
Verify Newton's Law of Cooling for a hot liquid cooling under convection and radiation.

### Theory & Derivations
- **Newton's Law Statement**: The rate of heat loss from a body is directly proportional to the temperature excess over its surroundings, provided the temperature difference is small:
  $$\frac{dQ}{dt} = \varepsilon A (\theta - \theta_0)$$
- Heat content of the calorimeter and water system:
  $$Q = (m_c s_c + m_w s_w)(\theta - \theta_0)$$
  $$\frac{dQ}{dt} = (m_c s_c + m_w s_w) \left(-\frac{d\theta}{dt}\right)$$
- Equating heat loss rates:
  $$\left|\frac{d\theta}{dt}\right| = \left(\frac{\varepsilon A}{m_c s_c + m_w s_w}\right) (\theta - \theta_0) = k (\theta - \theta_0)$$
  where $\theta$ is hot water temperature and $\theta_0$ is constant ambient temperature.

### Procedure & Graphical Analysis
1. **Cooling Curve**: Plot temperature $\theta$ (°C) vs time $t$ (s).
2. **Tangents**: Draw geometric tangents at 6 different temperatures ($\theta_1, \theta_2, \dots$) to calculate the slope $\left|\frac{d\theta}{dt}\right|$ at each point.
3. **Verification Plot**: Plot cooling rate $\left|\frac{d\theta}{dt}\right|$ (°C/s) on Y-axis vs temperature excess $(\theta - \theta_0)$ (°C) on X-axis.
4. **Expected Result**: A straight line passing through the origin $(0,0)$, confirming $\left|\frac{d\theta}{dt}\right| \propto (\theta - \theta_0)$.

### Viva Questions & Crucial Precautions
1. **Why must the temperature excess be kept small ($\theta - \theta_0 < 30^\circ\text{C}$)?**
   - Stefan-Boltzmann radiation law states $E \propto (T^4 - T_0^4)$. Expanding as $T = T_0 + \Delta T$:
     $$(T_0 + \Delta T)^4 - T_0^4 \approx 4 T_0^3 \Delta T$$
     This linear approximation holds strictly only when $\Delta T \ll T_0$ (in Kelvin). At high temperatures, non-linear $T^4$ radiation dominates and Newton's law fails.
2. **Why use a double-walled container with a water jacket?**
   - Keeps the surrounding temperature $\theta_0$ stable and uniform, preventing draughts and environmental temperature drift from altering cooling rates.
3. **Why must the liquid be stirred continuously?**
   - Water has low thermal conductivity. Stirring ensures uniform temperature throughout the bulk liquid, so the thermometer reading represents the whole mass.

---

## 08. Wheatstone Bridge & Stefan's Law
Manual: [[PHY1921/08 - Wheatstone Bridge.pdf]]

### Aim
Investigate the temperature variation of a bulb filament with current and verify **Stefan’s Law of Radiation**.

### Theory & Derivations
- **Filament Resistance ($R_b$)**: Measured via Wheatstone bridge with bulb $B$ in one arm:
  $$\frac{X}{Y} = \frac{S}{R_b} \implies R_b(t) = \frac{Y S}{X}$$
- **Temperature Variation of Resistance**:
  Tungsten filament resistance varies with temperature $t$:
  $$R(t) = R(t_0)[1 + \alpha (t - t_0)] \implies t = t_0 + \frac{R(t) - R(t_0)}{\alpha R(t_0)}$$
  $$T = t + 273.15 \quad (\text{in Kelvin})$$
- **Stefan-Boltzmann Law**:
  Power radiated by the filament at absolute temperature $T$:
  $$P = I^2 R(t) = \varepsilon A \sigma T^4 \quad (\text{assuming } T \gg T_0)$$
- Taking natural logs:
  $$\ln(I^2 R(t)) = 4 \ln(T) + \ln(\varepsilon A \sigma)$$

### Graphical Analysis
- **Plot**: $\ln(I^2 R(t))$ on Y-axis vs $\ln(T)$ on X-axis.
- **Theoretical Gradient**: $m = 4$.
- **Verification**: If experimental gradient is close to 4 (typically between 3.5 and 4.2), Stefan's $T^4$ radiation law is verified.

### Viva Questions & Crucial Precautions
1. **How is the cold resistance $R(t_0)$ obtained accurately?**
   - Measured directly across the bulb at room temperature using a digital multimeter before powering up, ensuring negligible current flows during measurement.
2. **Why does the experimental gradient often deviate slightly from 4?**
   - Conduction losses through filament lead wires and convection losses through gas inside the bulb.
   - The emissivity $\varepsilon$ of tungsten is not strictly constant; it increases slightly with temperature.
3. **Key operational sequence:**
   - Always close the battery circuit key first and then tap the galvanometer key to prevent transient inductive deflections.

---

## 09. Tangent Galvanometer
Manual: [[PHY1921/09 -Tangent Galvanometer.pdf]]

### Aim
Determine the horizontal component of Earth’s magnetic field ($B_0$), galvanometer internal resistance ($G$), and the magnetic field of a bar magnet ($B_{mag}$).

### Theory & Derivations
- Circular coil of $n$ turns, radius $r$, carrying current $I$:
  $$B = \frac{\mu_0 n I}{2r}$$
- When coil plane is aligned along the magnetic meridian, $B \perp B_0$. The magnetic needle deflects by angle $\theta$:
  $$B = B_0 \tan\theta$$
- By Ohm's law with supply EMF $E$, variable resistance $R$, and coil resistance $G$:
  $$I = \frac{E}{R + G}$$
  $$B_0 \tan\theta = \frac{\mu_0 n E}{2r (R + G)}$$
- Rearranging in linear form ($y = mx + c$):
  $$\cot\theta = \frac{1}{\tan\theta} = \left(\frac{2r B_0}{\mu_0 n E}\right) R + \left(\frac{2r B_0 G}{\mu_0 n E}\right)$$

### Graphical Analysis
- **Plot**: $\cot\theta$ on Y-axis vs $R$ ($\Omega$) on X-axis.
- **Slope**: $m = \frac{2r B_0}{\mu_0 n E} \implies B_0 = \frac{m \mu_0 n E}{2r} \quad (\text{Tesla})$.
- **Y-intercept**: $c = \frac{2r B_0 G}{\mu_0 n E}$.
- **Galvanometer Resistance**:
  $$G = \frac{\text{Intercept}}{\text{Slope}} = \frac{c}{m} \quad (\Omega)$$

### Viva Questions & Crucial Precautions
1. **Purpose of the commutator (reversing key):**
   - Reversing current eliminates error caused by imperfect alignment of the coil plane with the magnetic meridian. Readings are taken at both ends of the pointer for both normal and reversed current (4 readings averaged per resistance $R$).
2. **Why use a spirit level?**
   - Ensures the compass box is perfectly horizontal so the needle pivots freely without friction against the glass top or dial face.
3. **Why select $R \approx 40\,\Omega$ in the magnet deflection section?**
   - Keeps current moderate and deflections within the sensitive $30^\circ - 60^\circ$ range where tangent readouts have lowest sensitivity to angle reading errors.

---

## 10. Capacitor Charging and Discharging
Manual: [[PHY1921/10 - Capacitor Charging and Discharging.pdf]]

### Aims
- **Part 10-A**: Determine capacitance ($C$) and internal leakage resistance ($r_c$) of an electrolytic capacitor using manual timing.
- **Part 10-B**: Measure time constant ($\tau = RC$), potential decay curve, and fit an exponential model using computer interface (Logger Pro / LabPro).

### Theory & Derivations
- **Charging**:
  $$q(t) = Q_0 \left(1 - e^{-t/RC}\right) \implies V(t) = V_0 \left(1 - e^{-t/RC}\right)$$
  $$I(t) = I_0 e^{-t/RC}$$
- **Discharging**:
  $$q(t) = Q_0 e^{-t/RC} \implies V(t) = V_0 e^{-t/RC}$$
  $$I(t) = I_0 e^{-t/RC}$$
- **Time Constant ($\tau$)**:
  $$\tau = R C$$
  Time required for charge/voltage to decay to $e^{-1} \approx 36.8\%$ of initial value, or reach $(1 - e^{-1}) \approx 63.2\%$ during charging.

### Graphical & Computational Analysis
- **Part 10-A (Manual)**:
  - Total charge stored: $Q = \int_0^\infty I dt = \text{Area under } I \text{ vs } t \text{ curve}$.
  - Capacitance: $C = \frac{Q}{V_0}$.
  - Discharging linear form:
    $$\ln\left(\frac{I_0}{I}\right) = \left(\frac{1}{R_{eff} C}\right) t$$
    Plot $\ln(I_0 / I)$ vs $t$. Slope $m = \frac{1}{R_{eff} C} \implies R_{eff} = \frac{1}{m C}$.
- **Part 10-B (Logger Pro Curve Fit)**:
  - Fit function: $V(t) = A e^{-C_{fit} t} + B$.
  - Experimental time constant: $\tau_{exp} = \frac{1}{C_{fit}}$.
  - Compare $\tau_{exp}$ with theoretical $\tau_{theo} = R C$.

### Viva Questions & Crucial Precautions
1. **Why must electrolytic capacitors be connected with correct polarity?**
   - Electrolytic capacitors have an ultra-thin dielectric oxide layer formed electrochemically. Reverse voltage dissolves the dielectric, causing high leakage currents, rapid overheating, and potential explosion.
2. **Why must the capacitor be fully discharged before starting?**
   - Residual charge corrupts initial boundary conditions ($q(0) \neq 0$), distorting current integrals and time constant measurements.
3. **Why does charging current drop to zero?**
   - As charge accumulates, the counter-EMF of the capacitor grows until $V_c = E_{supply}$, leaving zero net potential difference across series resistor $R$.

---

## 11. Melting Point of Wax
Manual: [[PHY1921/11 - Melting Point of Wax.pdf]]

### Aim
Determine the melting/freezing point of paraffin wax from its cooling curve.

### Theory & Principle
- Phase change is an isothermal process governed by **latent heat of fusion** ($L_f$):
  $$Q = m L_f$$
- When molten wax cools:
  1. **Liquid Cooling Region**: Temperature falls continuously as sensible heat is lost to surroundings.
  2. **Phase Transition Plateau (Freezing / Arrest Point)**: Liquid begins crystallizing into solid. Latent heat released by bond formation exactly balances heat loss to surroundings:
     $$\frac{d\theta}{dt} = 0 \implies \text{Temperature remains constant at } T_m$$
  3. **Solid Cooling Region**: Once completely solidified, temperature resumes decreasing toward ambient temperature.

### Graphical Analysis
- **Plot**: Temperature $\theta$ (°C) on Y-axis vs Time $t$ (s) on X-axis.
- **Melting Point ($T_m$)**: Read the temperature corresponding to the horizontal plateau.

### Viva Questions & Crucial Precautions
1. **Why heat wax in a water bath rather than directly over the flame?**
   - Wax has low thermal conductivity and is flammable. Direct heating creates severe localized overheating, decomposition, smoke, and fire risk. A water bath ensures gentle, uniform heating.
2. **How much water should be added to the beaker?**
   - Water level should be slightly higher than the wax level in the boiling tube so all wax melts uniformly.
3. **What is supercooling?**
   - The liquid temperature may temporarily drop slightly below $T_m$ without solidifying due to lack of crystal nucleation sites. Once crystallization initiates, latent heat release causes temperature to jump back up to $T_m$.

---

## 12. Properties of Matter II (Poiseuille Flow)
Manual: [[PHY1921/12 - Properties of Matter II.pdf]]

### Aim
Determine the coefficient of viscosity ($\eta$) of water by the horizontal capillary flow method.

### Theory & Derivation
- **Poiseuille's Law**: For steady, laminar, streamline flow of an incompressible fluid through a narrow horizontal circular tube of radius $a$ and length $l$:
  $$\frac{V}{t} = \frac{\pi a^4 \Delta P}{8 \eta l}$$
- Hydrostatic driving pressure head:
  $$\Delta P = h \rho g$$
- Substituting into Poiseuille's formula:
  $$\frac{V}{t} = \left(\frac{\pi a^4 \rho g}{8 \eta l}\right) h$$

### Graphical Analysis
- **Plot**: Volume flow rate $\frac{V}{t}$ ($\text{m}^3/\text{s}$) on Y-axis vs pressure head $h$ (m) on X-axis.
- **Expected Graph**: Straight line passing through the origin.
- **Gradient**:
  $$m = \frac{\pi a^4 \rho g}{8 \eta l}$$
- **Extraction**:
  $$\eta = \frac{\pi a^4 \rho g}{8 l \cdot m} \quad (\text{N}\cdot\text{s/m}^2 \text{ or Pa}\cdot\text{s})$$

### Viva Questions & Crucial Precautions
1. **Why must the capillary tube be strictly leveled with a spirit level?**
   - If the tube slopes downward, gravity aids flow; if it slopes upward, gravity opposes flow. Horizontal alignment ensures the measured hydrostatic head $h$ is the sole driving pressure gradient.
2. **Why must flow be streamline and not turbulent?**
   - Poiseuille’s law is derived strictly for laminar, non-turbulent flow (Reynolds number $Re < 2000$). The pressure head $h$ must be kept small to keep flow velocity below the critical velocity.
3. **Why is measuring radius $a$ the most critical step?**
   - Viscosity depends on the **fourth power of the radius** ($a^4$). By error propagation:
     $$\frac{\Delta \eta}{\eta} \approx 4 \frac{\Delta a}{a}$$
     A $1\%$ error in measuring $a$ leads to a $4\%$ error in $\eta$! Radius must be measured at both ends using a travelling microscope with orthogonal diameter averaging.
4. **Why record water temperature?**
   - The viscosity of liquids decreases substantially with temperature (approx. $2-3\%$ per °C for water). Quoting $\eta$ without recording temperature is physically meaningless.

---

## 🔬 Quick High-Yield Viva & Practical Formulas Reference

### Common Instruments & Resolution
- **Meter ruler**: Least count = $1\text{ mm} = 0.1\text{ cm}$
- **Vernier Caliper**: Least count = $0.1\text{ mm} = 0.01\text{ cm}$
- **Micrometer Screw Gauge**: Least count = $0.01\text{ mm} = 0.001\text{ cm}$
- **Travelling Microscope**: Least count = $0.01\text{ mm} = 0.001\text{ cm}$
- **Cathetometer**: Least count = $0.01\text{ mm}$
- **Stopwatch**: Least count = $0.01\text{ s}$ (human reaction time error $\sim 0.2\text{ s}$)

### Key Physics Constants & Densities
- Density of pure water ($\rho_w$): $1000\text{ kg/m}^3$ (or $1.00\text{ g/cm}^3$)
- Acceleration due to gravity ($g$): $9.81\text{ m/s}^2$
- Permeability of free space ($\mu_0$): $4\pi \times 10^{-7}\text{ T}\cdot\text{m/A}$
- Stefan-Boltzmann constant ($\sigma$): $5.670 \times 10^{-8}\text{ W}/(\text{m}^2\cdot\text{K}^4)$
