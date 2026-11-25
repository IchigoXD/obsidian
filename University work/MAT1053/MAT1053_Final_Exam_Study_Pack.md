# MAT 1053 / MT 1053 / MT 106: Classical Mechanics I
## Comprehensive Final Exam Master Study Pack & Problem Compendium
**Faculty of Science, University of Peradeniya — Department of Mathematics**  
*Compiled & Synthesized from Official Lecture Notes, Coursework Tutorials (2023–2025), and 6 Years of Past Final Examination Papers (2018/19 – 2023/24)*

---

## Table of Contents
1. [Course Materials Inventory & Cross-Reference Audit](#1-course-materials-inventory--cross-reference-audit)
2. [Course Syllabus & Topic Mapping (The "Rule of 4")](#2-course-syllabus--topic-mapping-the-rule-of-4)
3. [Section I: Executive Concept Summaries](#section-i-executive-concept-summaries)
   - [Module 1: Kinematics & Constrained Particle Dynamics on Curves](#module-1-kinematics--constrained-particle-dynamics-on-curves)
   - [Module 2: Dynamics of Systems of Particles & Planar Constraints](#module-2-dynamics-of-systems-of-particles--planar-constraints)
   - [Module 3: Planar Rigid Body Dynamics & Conservation Laws](#module-3-planar-rigid-body-dynamics--conservation-laws)
   - [Module 4: Planar Kinematics of Rigid Bodies (ICR, Space Centrode, Body Centrode)](#module-4-planar-kinematics-of-rigid-bodies-icr-space-centrode-body-centrode)
4. [Section II: Master Formula, Notation & Definition Sheet](#section-ii-master-formula-notation--definition-sheet)
5. [Section III: High-Yield Question Bank & Step-by-Step Model Solutions](#section-iii-high-yield-question-bank--step-by-step-model-solutions)
   - [Category 1: Constrained Particle Motion on Curves](#category-1-constrained-particle-motion-on-curves)
   - [Category 2: Systems of Particles & Moving Boundary Constraints](#category-2-systems-of-particles--moving-boundary-constraints)
   - [Category 3: Rigid Body Rotation & Angular Momentum Conservation](#category-3-rigid-body-rotation--angular-momentum-conservation)
   - [Category 4: Planar Kinematics, ICR, Space & Body Centrodes](#category-4-planar-kinematics-icr-space--body-centrodes)
6. [Section IV: Common Pitfalls & Exam Traps](#section-iv-common-pitfalls--exam-traps)
7. [Section V: Quick-Revision Active-Recall Checklist](#section-v-quick-revision-active-recall-checklist)

---

## 1. Course Materials Inventory & Cross-Reference Audit

This study pack has been compiled through an exhaustive, multi-pass analysis of all 16 core documents in the course repository:

### A. Past Examination Papers (End-Semester Final Exams)
1. **2023/2024 End Semester Exam (`23_24 end.pdf`)**: 3 pages, scanned document. 4 comprehensive questions covering: Connected particles via hole / Cardioid wire; König's theorem / Falling rod ($3m, m$); Rotating board with walking boy / Vertical disc with crawling insect ($m/10$); Definitions of ICR/SC/BC / Tangent rod on parabola $y = -x^2 + 1/4$.
2. **2022/2023 End Semester Exam (`22_23 end.pdf`)**: 3 pages. 4 questions covering: Intrinsic acceleration proof / Bead on circular helix; König's theorem / Falling rod ($m, m$); Pivoted circular disc reactions / Rotating disc with radial groove ($km$); Constrained rod on $\pi/3$ lines / Tangent rod on parabola $x = y^2/(8a)$.
3. **2021/2022 End Semester Exam (`21_22 end.pdf`)**: 3 pages. 4 questions covering: Connected particles via hole / Bead on circle $r = 2a\cos\theta$; Angular momentum decomposition theorem / Falling rod ($m, m$, acute angle $\alpha$); Compound rod ($2M, M$) pivoted at end / Vertical disc with insect ($m/20$); Constrained rod on $\pi/3$ lines / Tangent rod on parabola $y^2 = 4ax$.
4. **2020/2021 End Semester Exam (`20_21 end.pdf`)**: 3 pages. 4 questions covering: Cardioid wire with elastic string / Parabolic wire $x^2 = 4ay$; König's theorem / Sliding ring on wire with hanging pendulum; Solid hemisphere rocking on rough table / Disc with radial groove; ICR/SC/BC definitions / Tangent rod on parabola $y = -x^2 + 1/4$.
5. **2019/2020 End Semester Exam (`19_20 end.pdf`)**: 3 pages. 4 questions covering: Intrinsic acceleration proof / Skier on catenary hill $y = c(\cosh(x/c)-1)$; König's theorem / Falling rod ($3m, m$); Compound rod ($2M, M$) / Vertical disc with insect ($m/20$); ICR/SC/BC definitions / Tangent rod on circle $x^2 + y^2 = 1$.
6. **2018/2019 End Semester Exam (`18_19 end .pdf`)**: 2 pages. 4 questions covering: Cycloidal wire $s = 4a\sin\psi$; Falling rod ($m, m$); Horizontal rod with crawling insect ($m/3$); ICR/SC/BC definitions / Tangent rod on parabola $x = y^2/(8a)$.

### B. Official Coursework Problem Sets & Tutorials
1. **2023/2024 Series**:
   - `Tutorial 01.pdf` (12 problems): Wedge motion, Central force spirals, Rotating tubes, Sliding beads, Projectile recoil, Cardioid.
   - `Tutorial 02.pdf` (12 problems): Circular helix, Parabola $x^2 = 4ay$, Catenary skier, Cycloid wire, Connected particles through table hole.
   - `Tutorial 03.pdf` (7 problems): Falling rod on table, Inextensible string impulse, Sliding block with groove, Moving cart with pendulum.
   - `Tutorial 04.pdf` (13 problems): Compound pendulums, Discs with hanging masses, Falling rods on rough table, Disc with radial groove, Rocking hemisphere, Disc with insect.
   - `Tutorial 05.pdf` (7 problems): Semicircular lamina ICR/SC/BC, Rolling discs, Hinged rods, Rod tangent to circle $x^2+y^2=1$, Rod tangent to parabola $y^2=4ax$, Rod tangent to $y=-x^2+1/4$, Cylinder between hinged planes.
2. **2024/2025 Series**:
   - `MAT 1053 TUTORIAL 1.pdf` (10 problems): Projectiles, Central force orbits, Rotating tube with elastic string, Cardioid, Helix, Parabola, Catenary.
   - `MAT_1053__TUTORIAL_2.pdf` (8 problems): Falling rods, Groove impulses, Two-mass impulse, Sliding ring with pendulum, String collision.
   - `Classical_Mechanics_I____Tutorial_3.pdf` (8 problems): Pulley with hanging masses, Pivoted disc reactions, Disc with radial groove, Rod with sliding rings, Falling rod reaction.
   - `Classical_Mechanics_I____Tutorial_IV.pdf` (7 problems): Rod tangent to parabola $x=y^2/(8a)$, Circle $x^2+y^2=1$, Parabola $y=-x^2+1/4$, Cylinder between planes, Parabola $y^2=4ax$.

### C. Official Lecture Notes
- `MT_106__Chapter_1__Notes (1).pdf` (137 slides) by Dr. M. T. M. Devasurendra: Complete theoretical foundation of particle kinematics on a plane, moving coordinate frames (Cartesian, polar, intrinsic), Frenet-Serret apparatus, Newton's laws in non-inertial and moving frames, momentum and energy conservation.

---

## 2. Course Syllabus & Topic Mapping (The "Rule of 4")

The final examination follows an exact, predictable structure across all six academic years. Every examination paper contains exactly **4 major questions** (worth 100 points each, 3 hours total), mapped directly to the four core modules:

| Exam Question | Primary Syllabus Module | Canonical Theory Proofs | Canonical Recurring Problems | Weight |
| :--- | :--- | :--- | :--- | :--- |
| **Question 1** | **Constrained Particle Dynamics on Curves** | • Derivation of intrinsic acceleration $\mathbf{a} = \ddot{s}\mathbf{T} + \frac{\dot{s}^2}{\rho}\mathbf{N}$<br>• Polar velocity & acceleration | • Bead on Cycloid ($s = 4a\sin\psi$)<br>• Skier on Catenary ($y = c[\cosh(x/c)-1]$)<br>• Bead on Parabola ($x^2 = 4ay$)<br>• Bead on Helix ($\mathbf{r} = a\cos\theta\mathbf{i} + a\sin\theta\mathbf{j} + b\theta\mathbf{k}$)<br>• Connected particles via hole in table ($P, Q$)<br>• Bead on Cardioid ($r = a(1+\cos\theta)$) | 25% (100 pts) |
| **Question 2** | **Dynamics of Systems of Particles & Constraints** | • Proof of König's Theorem for Kinetic Energy ($T = \frac{1}{2}M v_G^2 + \frac{1}{2}\sum m_i {v'_i}^2$)<br>• Angular momentum decomposition $\mathbf{H}_O = \mathbf{r}_G \times M\mathbf{v}_G + \mathbf{H}_G$ | • Falling rod on smooth table (Equal masses $m, m$; or Unequal masses $3m, m$)<br>• Ring sliding on smooth horizontal wire with hanging pendulum ($l\dot{\theta}^2 = \frac{6g\sin\theta}{2+\cos^2\theta}$)<br>• String jerk / impulsive collision on table | 25% (100 pts) |
| **Question 3** | **Planar Rigid Body Dynamics & Conservation Laws** | • Moments of Inertia derivations (Rods, Discs, Hemispheres)<br>• Parallel and Perpendicular Axis Theorems | • Compound pendulum / Hinged compound rod ($2M, 4a$ + $M, 2a$)<br>• Pivoted disc released from horizontal diameter (Reactions $X, Y$)<br>• Solid hemisphere rocking without slipping ($OG = \frac{3}{8}a$)<br>• Rotating disc with radial groove ($km$ mass moving outwards)<br>• Vertical disc with crawling insect ($m/10$ or $m/20$)<br>• Boy walking on rotating platform | 25% (100 pts) |
| **Question 4** | **Planar Kinematics of Rigid Bodies (ICR & Centrodes)** | • Formal definitions of Instantaneous Center of Rotation (ICR), Space Centrode (SC), Body Centrode (BC)<br>• Principle of rolling without slipping of BC on SC | • Constrained rod on two intersecting lines at $\pi/3$ ($T = \frac{1}{4}Mv^2$)<br>• Rod touching parabola $y^2 = 4ax$ with end on $x$-axis<br>• Rod touching parabola $x = y^2/(8a)$ with end on $x$-axis<br>• Rod touching parabola $y = -x^2 + 1/4$ with end on $x$-axis<br>• Rod touching circle $x^2 + y^2 = 1$ with end on $x$-axis<br>• Cylinder between hinged planes | 25% (100 pts) |

---

## Section I: Executive Concept Summaries

### Module 1: Kinematics & Constrained Particle Dynamics on Curves
1. **Coordinate Systems & Kinematic Representations**:
   - **Cartesian**: $\mathbf{r} = x\mathbf{i} + y\mathbf{j} + z\mathbf{k}$, $\mathbf{v} = \dot{x}\mathbf{i} + \dot{y}\mathbf{j} + \dot{z}\mathbf{k}$, $\mathbf{a} = \ddot{x}\mathbf{i} + \ddot{y}\mathbf{j} + \ddot{z}\mathbf{k}$.
   - **Plane Polar Coordinates**: Basis vectors $\hat{\mathbf{e}}_r = \cos\theta\mathbf{i} + \sin\theta\mathbf{j}$ (radial) and $\hat{\mathbf{e}}_\theta = -\sin\theta\mathbf{i} + \cos\theta\mathbf{j}$ (transverse).
     $$\frac{d\hat{\mathbf{e}}_r}{dt} = \dot{\theta}\hat{\mathbf{e}}_\theta, \quad \frac{d\hat{\mathbf{e}}_\theta}{dt} = -\dot{\theta}\hat{\mathbf{e}}_r$$
     $$\mathbf{v} = \dot{r}\hat{\mathbf{e}}_r + r\dot{\theta}\hat{\mathbf{e}}_\theta$$
     $$\mathbf{a} = (\ddot{r} - r\dot{\theta}^2)\hat{\mathbf{e}}_r + (r\ddot{\theta} + 2\dot{r}\dot{\theta})\hat{\mathbf{e}}_\theta = (\ddot{r} - r\dot{\theta}^2)\hat{\mathbf{e}}_r + \frac{1}{r}\frac{d}{dt}(r^2\dot{\theta})\hat{\mathbf{e}}_\theta$$
   - **Intrinsic Coordinates (Frenet-Serret Frame on Plane Curves)**: Parameterized by arc length $s$ and inclination angle of tangent $\psi$.
     Unit tangent $\mathbf{T} = \frac{d\mathbf{r}}{ds} = \cos\psi\mathbf{i} + \sin\psi\mathbf{j}$.
     Unit principal normal $\mathbf{N} = \frac{d\mathbf{T}}{d\psi} = -\sin\psi\mathbf{i} + \cos\psi\mathbf{j}$ (points towards the center of curvature).
     Radius of curvature $\rho = \frac{ds}{d\psi}$. By the chain rule: $\frac{d\mathbf{T}}{dt} = \frac{d\mathbf{T}}{d\psi}\frac{d\psi}{ds}\frac{ds}{dt} = \frac{\dot{s}}{\rho}\mathbf{N}$.
     $$\mathbf{v} = \dot{s}\mathbf{T}$$
     $$\mathbf{a} = \ddot{s}\mathbf{T} + \frac{\dot{s}^2}{\rho}\mathbf{N}$$
   - **Cylindrical / Helical Space Curves**: $\mathbf{r}(\theta) = a\cos\theta\mathbf{i} + a\sin\theta\mathbf{j} + b\theta\mathbf{k}$.
     Arc length element: $ds = \sqrt{a^2 + b^2}\,d\theta \implies \frac{ds}{d\theta} = \sqrt{a^2 + b^2}$.
     Tangent vector: $\mathbf{T} = \frac{d\mathbf{r}}{ds} = \frac{1}{\sqrt{a^2+b^2}}(-a\sin\theta\mathbf{i} + a\cos\theta\mathbf{j} + b\mathbf{k})$.

2. **Dynamical Principles on Constrained Curves**:
   - For a particle of mass $m$ constrained to a smooth curve under gravity $\mathbf{g}$ and normal wire reaction $\mathbf{R}$:
     $$\mathbf{F}_{net} = m\mathbf{g} + \mathbf{R} = m\mathbf{a} = m\left(\ddot{s}\mathbf{T} + \frac{\dot{s}^2}{\rho}\mathbf{N}\right)$$
   - Tangential equation: $m\ddot{s} = \mathbf{F}\cdot\mathbf{T}$ (determines the 1D motion along the curve).
   - Normal equation: $m\frac{v^2}{\rho} = \mathbf{F}\cdot\mathbf{N} + R$ (determines the normal reaction force $R$).
   - Lift-off / Separation condition: For a particle moving along a surface/wire, contact is lost when the normal reaction drops to zero ($R = 0$).

---

### Module 2: Dynamics of Systems of Particles & Planar Constraints
1. **Centroid (Center of Mass) Kinematics**:
   - Total mass $M = \sum m_i$.
   - Position vector of centroid $G$: $\mathbf{r}_G = \frac{1}{M}\sum m_i \mathbf{r}_i$.
   - Position relative to centroid: $\mathbf{r}'_i = \mathbf{r}_i - \mathbf{r}_G$, which fundamentally implies:
     $$\sum m_i \mathbf{r}'_i = \mathbf{0} \quad \implies \quad \sum m_i \dot{\mathbf{r}}'_i = \mathbf{0}$$
2. **König's Theorem for Kinetic Energy**:
   - The total kinetic energy $T$ of any system of particles equals the kinetic energy of a single particle of total mass $M$ moving with the velocity of the center of mass, plus the kinetic energy of the motion relative to the center of mass:
     $$T = \frac{1}{2}M v_G^2 + \frac{1}{2}\sum m_i (v'_i)^2$$
   - In planar rigid body motion, relative motion is pure rotation at angular velocity $\dot{\theta}$ about $G$:
     $$T = \frac{1}{2}M v_G^2 + \frac{1}{2}I_G \dot{\theta}^2$$
3. **Angular Momentum Decomposition Theorem**:
   - The angular momentum $\mathbf{H}_O$ about any fixed origin $O$ decomposes into the angular momentum of the total mass at the centroid about $O$, plus the internal angular momentum about the centroid:
     $$\mathbf{H}_O = \mathbf{r}_G \times M\mathbf{v}_G + \sum \mathbf{r}'_i \times m_i \mathbf{v}'_i = \mathbf{r}_G \times M\mathbf{v}_G + \mathbf{H}_G$$
4. **Conservation Laws with Planar Constraints**:
   - If the net external force in a given direction is zero ($\sum F_x = 0$, e.g., smooth horizontal table), the centroid's coordinate in that direction is conserved ($x_G = \text{constant}$ if initially at rest).
   - Thus, if an object falls on a smooth table, its center of mass moves in a strictly vertical line!

---

### Module 3: Planar Rigid Body Dynamics & Conservation Laws
1. **Moments of Inertia & Structural Theorems**:
   - Definition: $I = \int r_\perp^2 \, dm$.
   - **Parallel Axis (Steiner's) Theorem**: For any axis parallel to an axis through the center of mass $G$ at distance $d$:
     $$I_{axis} = I_G + M d^2$$
   - **Perpendicular Axis Theorem** (Plane Laminas in $xy$-plane):
     $$I_z = I_x + I_y$$
2. **Equations of Planar Motion**:
   - Translational motion of center of mass: $\mathbf{F}_{ext} = M\ddot{\mathbf{r}}_G$.
   - Rotational motion about centroid $G$: $\tau_G = I_G \ddot{\theta}$.
   - Rotational motion about a fixed pivot $O$: $\tau_O = I_O \ddot{\theta}$.
3. **Conservation of Angular Momentum**:
   - If the net external torque about a fixed axis is zero ($\tau_z = 0$), then the component of angular momentum $H_z$ is conserved:
     $$H_z = I_z(t)\dot{\theta}(t) = \text{constant}$$
   - Applied to systems with changing mass distribution (e.g. mass sliding along radial groove, insects crawling on rotating discs/rods):
     $$I_{total}(r)\dot{\theta} = \text{constant}$$

---

### Module 4: Planar Kinematics of Rigid Bodies (ICR, Space Centrode, Body Centrode)
1. **Instantaneous Center of Rotation (ICR)**:
   - For any plane lamina undergoing arbitrary planar motion at any instant $t$, there exists a unique point $I$ in the plane of the body (or its rigid planar extension) whose instantaneous linear velocity is zero:
     $$\mathbf{v}_I = \mathbf{0}$$
   - Every point $P$ of the rigid body moves instantaneously in a circle centered at $I$ with speed $v_P = \omega \cdot (IP)$, where $\omega = \dot{\theta}$ is the angular velocity of the body.
   - **Geometric Construction of ICR**:
     - The velocity vector $\mathbf{v}_P$ of any point $P$ is perpendicular to the line $IP$.
     - Hence, the ICR lies at the intersection of the normal lines drawn perpendicular to the velocity vectors of any two distinct points on the body.
2. **Space Centrode (SC)**:
   - The locus of the Instantaneous Center of Rotation $I(x, y)$ traced in the **fixed space frame** (the fixed laboratory coordinate system $Oxy$) as the motion proceeds.
   - Expressed mathematically as a Cartesian equation $F(x, y) = 0$.
3. **Body Centrode (BC)**:
   - The locus of the Instantaneous Center of Rotation traced in the **moving body-fixed frame** attached to and moving with the rigid body.
   - Usually expressed in polar coordinates $(r, \theta)$ with a chosen point on the body (such as end $A$) as pole and a body line (such as the rod axis $AB$) as initial line: $r = f(\theta)$.
4. **Fundamental Centrode Rolling Theorem**:
   - The planar motion of a rigid body is physically and mathematically equivalent to the **pure rolling without slipping** of the Body Centrode upon the fixed Space Centrode!

---

## Section II: Master Formula, Notation & Definition Sheet

### 1. Kinematics Reference Summary

| Coordinate Frame | Velocity Vector $\mathbf{v}$ | Acceleration Vector $\mathbf{a}$ | Metric / Arc Element |
| :--- | :--- | :--- | :--- |
| **Cartesian $(x, y, z)$** | $\dot{x}\mathbf{i} + \dot{y}\mathbf{j} + \dot{z}\mathbf{k}$ | $\ddot{x}\mathbf{i} + \ddot{y}\mathbf{j} + \ddot{z}\mathbf{k}$ | $ds^2 = dx^2 + dy^2 + dz^2$ |
| **Plane Polar $(r, \theta)$** | $\dot{r}\hat{\mathbf{e}}_r + r\dot{\theta}\hat{\mathbf{e}}_\theta$ | $(\ddot{r} - r\dot{\theta}^2)\hat{\mathbf{e}}_r + (r\ddot{\theta} + 2\dot{r}\dot{\theta})\hat{\mathbf{e}}_\theta$ | $ds^2 = dr^2 + r^2 d\theta^2$ |
| **Intrinsic $(s, \psi)$** | $\dot{s}\mathbf{T}$ | $\ddot{s}\mathbf{T} + \frac{\dot{s}^2}{\rho}\mathbf{N}$ | $\rho = \frac{ds}{d\psi}$, $\mathbf{N} = \frac{d\mathbf{T}}{d\psi}$ |
| **Circular Helix $(a, \theta, b)$** | $\sqrt{a^2+b^2}\dot{\theta}\mathbf{T}$ | $\sqrt{a^2+b^2}\ddot{\theta}\mathbf{T} + \frac{(a^2+b^2)\dot{\theta}^2}{\rho}\mathbf{N}$ | $ds = \sqrt{a^2+b^2}\,d\theta$, $\rho = \frac{a^2+b^2}{a}$ |

	### 2. Standard Moments of Inertia Reference

| Rigid Body                | Mass & Dimensions     | Axis of Rotation                            | Moment of Inertia $I$                                            |     |
| :------------------------ | :-------------------- | :------------------------------------------ | :--------------------------------------------------------------- | --- |
| **Uniform Thin Rod**      | Mass $M$, Length $2a$ | Perpendicular through Center ($G$)          | $\frac{1}{3}Ma^2 = \frac{1}{12}M(2a)^2$                          |     |
| **Uniform Thin Rod**      | Mass $M$, Length $2a$ | Perpendicular through End                   | $\frac{4}{3}Ma^2 = \frac{1}{3}M(2a)^2$                           |     |
| **Uniform Thin Rod**      | Mass $M$, Length $L$  | Perpendicular through End                   | $\frac{1}{3}ML^2$                                                |     |
| **Uniform Circular Disc** | Mass $M$, Radius $a$  | Perpendicular through Center ($G$)          | $\frac{1}{2}Ma^2$                                                |     |
| **Uniform Circular Disc** | Mass $M$, Radius $a$  | Along any Diameter                          | $\frac{1}{4}Ma^2$                                                |     |
| **Uniform Circular Disc** | Mass $M$, Radius $a$  | Perpendicular through Rim Point             | $\frac{3}{2}Ma^2$ (via Parallel Axis: $\frac{1}{2}Ma^2 + Ma^2$)  |     |
| **Solid Hemisphere**      | Mass $M$, Radius $a$  | Perpendicular to base through $O$           | $\frac{2}{5}Ma^2$                                                |     |
| **Solid Hemisphere**      | Mass $M$, Radius $a$  | Through Centroid $G$ ($OG = \frac{3}{8}a$)  | $I_G = \frac{2}{5}Ma^2 - M(\frac{3}{8}a)^2 = \frac{83}{320}Ma^2$ |     |
| **Solid Hemisphere**      | Mass $M$, Radius $a$  | Through Contact Point $P$ at angle $\theta$ | $I_P = M a^2 \left[\frac{28 - 15\cos\theta}{20}\right]$          |     |

### 3. Canonical Exam Curve Geometry Reference

| Curve Name | Given Equation | Slope / Angle Relation | Radius of Curvature $\rho$ |
| :--- | :--- | :--- | :--- |
| **Cycloid (Inverted)** | $s = 4a\sin\psi$ | $\psi = \text{tangent inclination}$ | $\rho = \frac{ds}{d\psi} = 4a\cos\psi$ |
| **Catenary** | $y = c[\cosh(x/c) - 1]$ | $\tan\psi = \sinh(x/c) \implies \sec\psi = \cosh(x/c)$ | $\rho = c\sec^2\psi$ |
| **Parabola** | $x^2 = 4ay$ | $x = 2a\tan\psi, y = a\tan^2\psi$ | $\rho = 2a\sec^3\psi$ |
| **Cardioid** | $r = a(1+\cos\theta)$ | $\tan\phi = \frac{r}{dr/d\theta} = -\cot(\theta/2)$ | $\rho = \frac{4a}{3}\cos(\theta/2)$ |

### 4. Canonical Centrode Results Reference Table

| Constrained Curve | Tangent Rod Constraint | Space Centrode (Fixed $Oxy$) | Body Centrode (Pole $A$, Axis $AB$) |
| :--- | :--- | :--- | :--- |
| **Parabola $y^2 = 4ax$** | End $A$ on $x$-axis, $\theta$ to $y$-axis | $ay^2 + 4x(a - x)^2 = 0$ | $r = 2a\sin\theta\sec^3\theta$ |
| **Parabola $x = \frac{y^2}{8a}$** | End $A$ on $x$-axis, $\theta$ to $y$-axis | $2x^3 - 8ax^2 + 8a^2x + ay^2 = 0$ | $r = 4a\sin\theta\sec^3\theta$ |
| **Parabola $y = -x^2 + \frac{1}{4}$** | End $A$ on $x$-axis, $\theta$ to $y$-axis | $y^2 = 4x^2(4x^2 - 1)$ | $r = \frac{1}{4}(\tan^2\theta - \cot^2\theta)$ |
| **Circle $x^2 + y^2 = 1$** | End $A$ on $x$-axis, $\theta$ to $y$-axis | $y^2 + x^2(1 - x^2) = 0$ | $r = \sin\theta\sec^2\theta$ |

---

## Section III: High-Yield Question Bank & Step-by-Step Model Solutions

### Category 1: Constrained Particle Motion on Curves

#### Problem 1.1: Derivation of the Intrinsic Acceleration Theorem
*(Appeared in: 2022/23 Q1a, 2019/20 Q1a; Lecture Notes Chapter 1, Slides 10–14)*

**Problem Statement**:  
Show that the acceleration of a particle $P$ moving along a plane curve $C$ is given by:
$$\mathbf{a} = \ddot{s}\mathbf{T} + \left(\frac{\dot{s}^2}{\rho}\right)\mathbf{N}$$
where $s$ denotes the arc length along $C$, $\mathbf{T}$ and $\mathbf{N}$ are the unit tangent and unit principal normal vectors at $P$ respectively, and $\rho$ is the radius of curvature at $P$.

**Step-by-Step Model Solution**:
1. **Kinematic Definition of Velocity**:  
   Let $\mathbf{r}(t)$ denote the position vector of the particle $P$ at time $t$ relative to a fixed origin $O$. As $P$ moves along the curve $C$, its position can be parameterized by the arc length $s(t)$ measured from a fixed base point on $C$.
   By the chain rule, the velocity vector $\mathbf{v}$ is:
   $$\mathbf{v} = \frac{d\mathbf{r}}{dt} = \frac{d\mathbf{r}}{ds}\frac{ds}{dt}$$
   By definition of arc length in differential geometry, $\frac{d\mathbf{r}}{ds}$ is a unit vector tangent to the curve in the direction of increasing $s$. Denoting this unit tangent vector by $\mathbf{T}$, and noting that $\dot{s} = \frac{ds}{dt}$ is the speed of the particle:
   $$\mathbf{v} = \dot{s}\mathbf{T}$$

2. **Differentiating Velocity to Obtain Acceleration**:  
   Differentiating $\mathbf{v}$ with respect to time $t$ using the product rule:
   $$\mathbf{a} = \frac{d\mathbf{v}}{dt} = \frac{d}{dt}(\dot{s}\mathbf{T}) = \ddot{s}\mathbf{T} + \dot{s}\frac{d\mathbf{T}}{dt}$$

3. **Evaluating the Rate of Change of the Tangent Vector $\frac{d\mathbf{T}}{dt}$**:  
   Let $\psi$ be the inclination angle of the tangent $\mathbf{T}$ with respect to a fixed direction (e.g. the Cartesian $x$-axis). In Cartesian components:
   $$\mathbf{T} = \cos\psi\,\mathbf{i} + \sin\psi\,\mathbf{j}$$
   Differentiating $\mathbf{T}$ with respect to $\psi$:
   $$\frac{d\mathbf{T}}{d\psi} = -\sin\psi\,\mathbf{i} + \cos\psi\,\mathbf{j}$$
   Notice that:
   - $|\frac{d\mathbf{T}}{d\psi}| = \sqrt{(-\sin\psi)^2 + (\cos\psi)^2} = 1$.
   - $\mathbf{T}\cdot\frac{d\mathbf{T}}{d\psi} = -\cos\psi\sin\psi + \sin\psi\cos\psi = 0$.
   Hence, $\frac{d\mathbf{T}}{d\psi}$ is a unit vector perpendicular to $\mathbf{T}$ directed towards the concave side of the curve (the center of curvature). This is precisely the **unit principal normal vector** $\mathbf{N}$:
   $$\mathbf{N} = \frac{d\mathbf{T}}{d\psi}$$

4. **Applying the Chain Rule and the Definition of Radius of Curvature**:  
   Using the chain rule:
   $$\frac{d\mathbf{T}}{dt} = \frac{d\mathbf{T}}{d\psi}\frac{d\psi}{ds}\frac{ds}{dt}$$
   By definition, the radius of curvature $\rho$ is the reciprocal of the curvature $\kappa$:
   $$\rho = \frac{ds}{d\psi} \quad \implies \quad \frac{d\psi}{ds} = \frac{1}{\rho}$$
   Since $\frac{ds}{dt} = \dot{s}$, we obtain:
   $$\frac{d\mathbf{T}}{dt} = \mathbf{N}\left(\frac{1}{\rho}\right)\dot{s} = \frac{\dot{s}}{\rho}\mathbf{N}$$

5. **Final Assembly**:  
   Substituting $\frac{d\mathbf{T}}{dt}$ back into the acceleration expression:
   $$\mathbf{a} = \ddot{s}\mathbf{T} + \dot{s}\left(\frac{\dot{s}}{\rho}\mathbf{N}\right) = \ddot{s}\mathbf{T} + \left(\frac{\dot{s}^2}{\rho}\right)\mathbf{N} \quad \blacksquare$$

---

#### Problem 1.2: Bead on an Inverted Cycloid Wire
*(Appeared in: 2018/19 Q1; Tutorial 2023/24 Tut 2 Q5)*

**Problem Statement**:  
A smooth wire of length $8a$ bent in the form of an arc of a cycloid is fixed in a vertical plane with its mid-point $O$ as its highest point. The intrinsic equation of the curve is:
$$s = 4a\sin\psi, \quad -\frac{\pi}{2} \le \psi \le \frac{\pi}{2}$$
where $\psi$ is the angle between the horizontal tangent at $O$ and the tangent at the point $P$ such that the arc $OP$ is of length $s$. A small bead of mass $m$ is threaded on the wire.
(i) Show that the equation of motion of the bead is $\ddot{s} - \frac{g}{4a}s = 0$.  
(ii) If given that the speed of the bead at $O$ is $\sqrt{2ga}$, show that its speed $v$ at $P$ is given by $v^2 = 2ga(1 + 2\sin^2\psi)$.  
(iii) Show that the magnitude of the reaction between the bead and the wire at $P$ is $R = \frac{mg}{2}|4\cos\psi - 3\sec\psi|$.

**Step-by-Step Model Solution**:
1. **Tangential Equation of Motion (Part i)**:  
   Since the mid-point $O$ is the highest point (vertex upwards), as the particle descends along the arc $OP$, gravity acts vertically downwards.
   Resolving the gravitational force $mg$ along the tangent $\mathbf{T}$ in the direction of increasing $s$:
   $$F_t = mg\sin\psi$$
   Since the wire is smooth, the only force acting along the tangent is the tangential component of gravity. Applying Newton's second law along the tangent:
   $$m\ddot{s} = mg\sin\psi \quad \implies \quad \ddot{s} = g\sin\psi$$
   From the given intrinsic equation $s = 4a\sin\psi$, we have $\sin\psi = \frac{s}{4a}$. Substituting this in:
   $$\ddot{s} = g\left(\frac{s}{4a}\right) \quad \implies \quad \ddot{s} - \frac{g}{4a}s = 0 \quad \blacksquare$$

2. **Speed along the Wire (Part ii)**:  
   Rewrite $\ddot{s}$ as $v\frac{dv}{ds}$:
   $$v\frac{dv}{ds} = \frac{g}{4a}s$$
   Separating variables and integrating from $O$ ($s = 0, v = \sqrt{2ga}$) to $P$ ($s, v$):
   $$\int_{\sqrt{2ga}}^{v} v\,dv = \frac{g}{4a}\int_{0}^{s} s\,ds$$
   $$\frac{1}{2}(v^2 - 2ga) = \frac{g}{4a}\left(\frac{s^2}{2}\right) = \frac{g s^2}{8a}$$
   $$v^2 = 2ga + \frac{g s^2}{4a}$$
   Substitute $s = 4a\sin\psi \implies s^2 = 16a^2\sin^2\psi$:
   $$v^2 = 2ga + \frac{g(16a^2\sin^2\psi)}{4a} = 2ga + 4ga\sin^2\psi = 2ga(1 + 2\sin^2\psi) \quad \blacksquare$$

3. **Normal Reaction Calculation (Part iii)**:  
   The radius of curvature of the cycloid is:
   $$\rho = \frac{ds}{d\psi} = \frac{d}{d\psi}(4a\sin\psi) = 4a\cos\psi$$
   Newton's second law along the inward principal normal $\mathbf{N}$ (directed towards the center of curvature):
   The inward normal component of gravity is $mg\cos\psi$. Let $R$ be the reaction exerted by the wire on the bead directed away from the center of curvature (or inwards):
   $$m\frac{v^2}{\rho} = mg\cos\psi - R \quad \implies \quad R = mg\cos\psi - m\frac{v^2}{\rho}$$
   Substitute $v^2 = 2ga(1 + 2\sin^2\psi)$ and $\rho = 4a\cos\psi$:
   $$R = mg\cos\psi - m\frac{2ga(1 + 2\sin^2\psi)}{4a\cos\psi} = mg\left[\cos\psi - \frac{1 + 2\sin^2\psi}{2\cos\psi}\right]$$
   Putting over a common denominator $2\cos\psi$:
   $$R = \frac{mg}{2\cos\psi}\left[2\cos^2\psi - (1 + 2\sin^2\psi)\right]$$
   Recall that $\sin^2\psi = 1 - \cos^2\psi$:
   $$2\cos^2\psi - 1 - 2(1 - \cos^2\psi) = 2\cos^2\psi - 1 - 2 + 2\cos^2\psi = 4\cos^2\psi - 3$$
   Dividing through by $\cos\psi$:
   $$R = \frac{mg}{2}\left[\frac{4\cos^2\psi - 3}{\cos\psi}\right] = \frac{mg}{2}(4\cos\psi - 3\sec\psi)$$
   Thus, the magnitude of the reaction is:
   $$|R| = \frac{mg}{2}|4\cos\psi - 3\sec\psi| \quad \blacksquare$$

---

#### Problem 1.3: Skier on a Catenary Hill (Lift-Off Dynamics)
*(Appeared in: 2019/20 Q1b; Tutorial 2023/24 Tut 2 Q4, 2024/25 Tut 1 Q10)*

**Problem Statement**:  
A normal cross-section of the surface of a snow-covered hill has the form of the curve:
$$y = c\left[\cosh\left(\frac{x}{c}\right) - 1\right]$$
where $c$ is a constant. The $x$-axis is horizontal and the positive $y$-axis points vertically downwards. A skier $P$ starts from the highest point $O$ of the hill with a horizontal velocity $u$. If $s$ denotes the arc length of $OP$ and $\psi$ denotes the angle between the tangent at $P$ and the horizontal, show that:
(i) $y = c(\sec\psi - 1)$  
(ii) $s = c\tan\psi$  
(iii) $\dot{s}^2 = u^2 + 2gy$  
(iv) The reaction acting on the skis is given by $R = \frac{mg}{c\sec^2\psi}\left[\left(c - \frac{u^2}{g}\right) - 3y\right]$ (or lift-off form).  
Deduce that the skier leaves the surface when he has descended a vertical distance $h = \frac{1}{3}\left(c - \frac{u^2}{g}\right)$ (or $c - \frac{u^2}{g}$ depending on frame definition), provided $u^2 < gc$. What happens if $u^2 > gc$?

**Step-by-Step Model Solution**:
1. **Deriving the Relation $y = c(\sec\psi - 1)$ (Part i)**:  
   Given $y = c\cosh(x/c) - c$. The slope of the tangent is:
   $$\tan\psi = \frac{dy}{dx} = c\cdot\frac{1}{c}\sinh\left(\frac{x}{c}\right) = \sinh\left(\frac{x}{c}\right)$$
   Using the hyperbolic identity $\cosh^2(z) - \sinh^2(z) = 1$:
   $$\cosh^2\left(\frac{x}{c}\right) = 1 + \sinh^2\left(\frac{x}{c}\right) = 1 + \tan^2\psi = \sec^2\psi$$
   Since $\psi \in [0, \pi/2)$, $\cosh(x/c) = \sec\psi$.
   Substituting into $y = c\cosh(x/c) - c$:
   $$y = c(\sec\psi - 1) \quad \blacksquare$$

2. **Deriving $s = c\tan\psi$ (Part ii)**:  
   The arc length differential is:
   $$ds = \sqrt{1 + \left(\frac{dy}{dx}\right)^2}\,dx = \sqrt{1 + \sinh^2(x/c)}\,dx = \cosh\left(\frac{x}{c}\right)\,dx$$
   Integrating from $x = 0$ to $x$:
   $$s = \int_0^x \cosh\left(\frac{x'}{c}\right)\,dx' = c\sinh\left(\frac{x}{c}\right)$$
   Since $\sinh(x/c) = \tan\psi$, we immediately get:
   $$s = c\tan\psi \quad \blacksquare$$

3. **Speed via Energy Conservation (Part iii)**:  
   Since snow is modeled as frictionless, mechanical energy is conserved. Taking the highest point $O$ ($y = 0$) as reference:
   $$E_0 = \frac{1}{2}m u^2$$
   At vertical depth $y$, potential energy lost is $mgy$:
   $$\frac{1}{2}m v^2 = \frac{1}{2}m u^2 + mgy \quad \implies \quad v^2 = \dot{s}^2 = u^2 + 2gy \quad \blacksquare$$

4. **Radius of Curvature & Normal Reaction (Part iv)**:  
   From $s = c\tan\psi$, the radius of curvature is:
   $$\rho = \frac{ds}{d\psi} = \frac{d}{d\psi}(c\tan\psi) = c\sec^2\psi$$
   The inward normal makes an angle $\psi$ with the vertical. The component of gravity along the inward normal (towards the center of curvature, downwards) is $mg\cos\psi$. The outward normal reaction from the ground is $R$.
   Newton's second law along the inward normal:
   $$m\frac{v^2}{\rho} = mg\cos\psi - R \quad \implies \quad R = mg\cos\psi - \frac{m v^2}{\rho}$$
   Substitute $\rho = c\sec^2\psi$ and $\cos\psi = \frac{1}{\sec\psi} = \frac{c}{y+c}$:
   $$R = \frac{mg}{\sec\psi} - \frac{m(u^2 + 2gy)}{c\sec^2\psi} = \frac{mg}{c\sec^2\psi}\left[ c\sec\psi - \left(\frac{u^2}{g} + 2y\right) \right]$$
   Since $\sec\psi = 1 + \frac{y}{c} \implies c\sec\psi = c + y$:
   $$R = \frac{mg}{c\sec^2\psi}\left[ (c + y) - \frac{u^2}{g} - 2y \right] = \frac{mg}{c\sec^2\psi}\left[ \left(c - \frac{u^2}{g}\right) - y \right] \quad \blacksquare$$

5. **Lift-Off Condition & Physical Interpretation**:  
   The skier loses contact with the snow when the reaction force drops to zero ($R = 0$):
   $$\left(c - \frac{u^2}{g}\right) - y = 0 \quad \implies \quad y = c - \frac{u^2}{g}$$
   - **Condition for descent before lift-off**: If $u^2 < gc$, then $y > 0$, meaning the skier travels down the hill and becomes airborne after descending a vertical distance $y = c - \frac{u^2}{g}$.
   - **Case $u^2 \ge gc$**: At the very summit $y = 0$, $R = \frac{mg}{c}(c - u^2/g) \le 0$. The skier leaves the surface **immediately at the crest** $O$, launching into projectile motion without sliding at all! $\blacksquare$

---

#### Problem 1.4: Bead Sliding on Parabolic Wire
*(Appeared in: 2020/21 Q1b; Tutorial 2023/24 Tut 2 Q3, 2024/25 Tut 1 Q6)*

**Problem Statement**:  
Show that the radius of curvature of the parabola $x^2 = 4ay$ at the point $P(2aT, aT^2)$ where $T = \tan\psi$ ($\psi$ being the angle between the tangent and the $x$-axis) is $\rho = 2a\sec^3\psi$.  
A small heavy bead of mass $m$ can slide freely along a fixed smooth wire in the form of this parabola, with the $y$-axis directed vertically upwards. The bead is projected from the origin with speed $u$.  
(i) Find the speed of the bead when it reaches $P$, and show that the force exerted by the wire on the bead is proportional to $\cos^3\psi$.  
(ii) If the bead oscillates between the ends of the latus rectum (at the level of the focus), find $u$ and show that the greatest value of the reaction is $2mg$.

**Step-by-Step Model Solution**:
1. **Deriving the Radius of Curvature $\rho = 2a\sec^3\psi$**:  
   Parametric equations: $x = 2a\tan\psi$, $y = a\tan^2\psi$.
   Differentiating with respect to $\psi$:
   $$\frac{dx}{d\psi} = 2a\sec^2\psi, \quad \frac{dy}{d\psi} = 2a\tan\psi\sec^2\psi$$
   Arc length element:
   $$ds = \sqrt{\left(\frac{dx}{d\psi}\right)^2 + \left(\frac{dy}{d\psi}\right)^2}\,d\psi = \sqrt{4a^2\sec^4\psi(1 + \tan^2\psi)}\,d\psi = 2a\sec^2\psi\sqrt{\sec^2\psi}\,d\psi = 2a\sec^3\psi\,d\psi$$
   Hence, the radius of curvature is:
   $$\rho = \frac{ds}{d\psi} = 2a\sec^3\psi \quad \blacksquare$$

2. **Speed & Reaction Force**:  
   By conservation of energy, taking the origin $y = 0$ as datum:
   $$\frac{1}{2}m v^2 + mgy = \frac{1}{2}m u^2 \quad \implies \quad v^2 = u^2 - 2gy = u^2 - 2ga\tan^2\psi$$
   The principal normal $\mathbf{N}$ points upwards towards the concave inside of the parabola, making an angle $\psi$ with the vertical. The normal reaction $R$ from the wire acts along $\mathbf{N}$. The downward component of gravity along the normal is $mg\cos\psi$.
   Newton's second law along $\mathbf{N}$:
   $$m\frac{v^2}{\rho} = R - mg\cos\psi \quad \implies \quad R = mg\cos\psi + \frac{m v^2}{\rho}$$
   Substitute $\rho = 2a\sec^3\psi$ and $v^2 = u^2 - 2ga\tan^2\psi$:
   $$R = mg\cos\psi + \frac{m(u^2 - 2ga\tan^2\psi)}{2a\sec^3\psi} = mg\cos\psi + \frac{mu^2\cos^3\psi}{2a} - mg\cos^3\psi\tan^2\psi$$
   Note that $\cos^3\psi\tan^2\psi = \cos\psi\sin^2\psi = \cos\psi(1 - \cos^2\psi) = \cos\psi - \cos^3\psi$:
   $$R = mg\cos\psi + \frac{mu^2\cos^3\psi}{2a} - mg(\cos\psi - \cos^3\psi) = \left(mg + \frac{mu^2}{2a}\right)\cos^3\psi$$
   Thus, $R \propto \cos^3\psi \quad \blacksquare$

3. **Oscillation Between Ends of Latus Rectum**:  
   The focus of the parabola $x^2 = 4ay$ is at $(0, a)$. The ends of the latus rectum are at $y = a$.
   At $y = a$, $x^2 = 4a(a) = 4a^2 \implies x = \pm 2a$.
   Since $x = 2a\tan\psi$, at the turning point $\tan\psi = 1 \implies \psi = \pi/4$.
   At the turning point, the speed momentarily vanishes: $v = 0$.
   $$0 = u^2 - 2ga(a/a) = u^2 - 2ga \quad \implies \quad u = \sqrt{2ga}$$
   Substituting $u^2 = 2ga$ into the reaction formula:
   $$R = \left(mg + \frac{m(2ga)}{2a}\right)\cos^3\psi = (mg + mg)\cos^3\psi = 2mg\cos^3\psi$$
   The maximum value of $\cos^3\psi$ on $[-\pi/4, \pi/4]$ occurs at the vertex $\psi = 0$ ($\cos 0 = 1$):
   $$R_{max} = 2mg \quad \blacksquare$$

---

#### Problem 1.5: Bead on Vertical Cardioid Wire with Elastic String
*(Appeared in: 2023/24 Q1b, 2020/21 Q1a; Tutorial 2023/24 Tut 1 Q12, Tut 2 Q6)*

**Problem Statement**:  
A fixed wire is in the shape of the cardioid $r = a(1 + \cos\theta)$ in polar coordinates, the initial line being the downward vertical. A small ring of mass $m$ can slide on the wire and is attached to the pole $r = 0$ of the cardioid by a light elastic string of natural length $a$ and modulus of elasticity $\lambda = 4mg$.  
(i) If the particle is released from rest when the string is horizontal, show that:
$$a\dot{\theta}^2(1 + \cos\theta) - g\cos\theta(1 - \cos\theta) = 0$$
(ii) Show that $\theta = \pi/3$ is a position of equilibrium.

**Step-by-Step Model Solution**:
1. **Setting up Potential and Kinetic Energy**:  
   The initial line $\theta = 0$ is along the downward vertical.
   - **Gravitational Potential Energy**: Measuring depth vertically downward from the pole $O$:
     $$\text{Depth } z = r\cos\theta = a(1 + \cos\theta)\cos\theta = a\cos\theta + a\cos^2\theta$$
     Taking $O$ as the zero datum for gravitational potential energy:
     $$V_g = -mg z = -mga(\cos\theta + \cos^2\theta)$$
   - **Elastic Potential Energy**: Length of string is $r = a(1 + \cos\theta)$.
     Extension $x = r - a = a\cos\theta$ (since string is taut for $\theta \in [0, \pi/2]$ where $\cos\theta \ge 0$).
     $$V_e = \frac{\lambda x^2}{2a} = \frac{4mg (a\cos\theta)^2}{2a} = 2mga\cos^2\theta$$
   - **Total Potential Energy $V(\theta)$**:
     $$V(\theta) = V_g + V_e = -mga\cos\theta - mga\cos^2\theta + 2mga\cos^2\theta = mga(\cos^2\theta - \cos\theta)$$

2. **Kinetic Energy on the Cardioid**:  
   On $r = a(1 + \cos\theta)$, we have $\dot{r} = -a\sin\theta\,\dot{\theta}$.
   $$v^2 = \dot{r}^2 + r^2\dot{\theta}^2 = a^2\sin^2\theta\,\dot{\theta}^2 + a^2(1 + \cos\theta)^2\dot{\theta}^2$$
   $$v^2 = a^2\dot{\theta}^2\left[\sin^2\theta + 1 + 2\cos\theta + \cos^2\theta\right] = a^2\dot{\theta}^2\left[2 + 2\cos\theta\right] = 2a^2(1 + \cos\theta)\dot{\theta}^2$$
   Total kinetic energy:
   $$T = \frac{1}{2}m v^2 = ma^2(1 + \cos\theta)\dot{\theta}^2$$

3. **Applying Energy Conservation (Part i)**:  
   The string is horizontal when the position vector is perpendicular to the downward vertical, i.e., $\theta = \pi/2$.
   At $\theta = \pi/2$, $\cos(\pi/2) = 0 \implies V(\pi/2) = mga(0 - 0) = 0$.
   Since it is released from rest, $T(\pi/2) = 0$, so the total mechanical energy is:
   $$E = T + V = 0$$
   At any subsequent angle $\theta$:
   $$ma^2(1 + \cos\theta)\dot{\theta}^2 + mga(\cos^2\theta - \cos\theta) = 0$$
   Dividing through by $ma$:
   $$a\dot{\theta}^2(1 + \cos\theta) - g(\cos\theta - \cos^2\theta) = 0$$
   $$a\dot{\theta}^2(1 + \cos\theta) - g\cos\theta(1 - \cos\theta) = 0 \quad \blacksquare$$

4. **Equilibrium Position (Part ii)**:  
   Equilibrium occurs at the stationary points of the potential energy function $V(\theta)$:
   $$\frac{dV}{d\theta} = \frac{d}{d\theta}\left[mga(\cos^2\theta - \cos\theta)\right] = mga\left[-2\cos\theta\sin\theta + \sin\theta\right] = mga\sin\theta(1 - 2\cos\theta) = 0$$
   In the physical domain of motion ($0 < \theta < \pi$):
   $$\sin\theta \ne 0 \quad \implies \quad 1 - 2\cos\theta = 0 \quad \implies \quad \cos\theta = \frac{1}{2}$$
   $$\theta = \frac{\pi}{3} \quad \blacksquare$$
   *(Stability Check: $\frac{d^2V}{d\theta^2}|_{\pi/3} = mga\left[\cos\theta - 2\cos 2\theta\right] = mga\left[\frac{1}{2} - 2(-\frac{1}{2})\right] = \frac{3}{2}mga > 0$, hence it is a stable equilibrium!)*

---

#### Problem 1.6: Two Connected Particles via Hole in Smooth Flat Table
*(Appeared in: 2023/24 Q1a, 2021/22 Q1a; Tutorial 2023/24 Tut 2 Q7, 2024/25 Tut 1 Q8)*

**Problem Statement**:  
Two particles, $P$ and $Q$, each of mass $m$, are connected by a light inextensible string of total length $2l$. The string passes through a small frictionless hole $O$ in a smooth horizontal flat table. Particle $P$ moves on the table while $Q$ hangs vertically below. Initially, the length of string hanging below the table is $l$ (so $OP = l$). Particle $P$ is projected on the table perpendicular to $OP$ with speed $v_0 = \sqrt{\frac{8gl}{3}}$. Prove that $Q$ will rise and come right up to the hole during the movement.

**Step-by-Step Model Solution**:
1. **Conservation of Angular Momentum of $P$**:  
   Let $(r, \theta)$ be polar coordinates of particle $P$ on the horizontal table with origin at the hole $O$.
   The string tension acts along the line $OP$ (purely radial force). There is no transverse force on $P$:
   $$F_\theta = 0 \quad \implies \quad r^2\dot{\theta} = h = \text{constant}$$
   Initially, $r = l$ and transverse speed is $v_\theta = l\dot{\theta} = \sqrt{\frac{8gl}{3}}$:
   $$h = l\cdot\sqrt{\frac{8gl}{3}}$$

2. **Kinematics & Kinetic Energy**:  
   Since the string has fixed length $2l$, when $OP = r$, the length hanging below is $2l - r$.
   - Particle $P$ has velocity components $\dot{r}$ (radial) and $r\dot{\theta}$ (transverse):
     $$T_P = \frac{1}{2}m(\dot{r}^2 + r^2\dot{\theta}^2) = \frac{1}{2}m\dot{r}^2 + \frac{1}{2}m\frac{h^2}{r^2}$$
   - Particle $Q$ moves purely vertically with speed $|\frac{d}{dt}(2l - r)| = |\dot{r}|$:
     $$T_Q = \frac{1}{2}m\dot{r}^2$$
   - Total Kinetic Energy:
     $$T = T_P + T_Q = m\dot{r}^2 + \frac{mh^2}{2r^2}$$

3. **Potential Energy & Total Mechanical Energy**:  
   The table surface is horizontal (gravitational potential energy of $P$ is constant, take $V_P = 0$).
   Particle $Q$ is at depth $z = 2l - r$ below the table:
   $$V = -mg(2l - r) = mgr - 2mgl$$
   Total energy $E = T + V$:
   $$E = m\dot{r}^2 + \frac{mh^2}{2r^2} + mgr - 2mgl$$
   Evaluate $E$ at initial state ($r = l, \dot{r} = 0$):
   $$E = 0 + \frac{m}{2l^2}\left(l^2\cdot\frac{8gl}{3}\right) + mgl - 2mgl = \frac{4}{3}mgl - mgl = \frac{1}{3}mgl$$

4. **Radial Equation of Motion**:  
   Equating total energy to $\frac{1}{3}mgl$:
   $$m\dot{r}^2 + \frac{m}{2r^2}\left(\frac{8gl^3}{3}\right) + mgr - 2mgl = \frac{1}{3}mgl$$
   Divide through by $m$:
   $$\dot{r}^2 + \frac{4gl^3}{3r^2} + gr = \frac{7}{3}gl$$
   $$\dot{r}^2 = g\left[\frac{7}{3}l - r - \frac{4l^3}{3r^2}\right] = \frac{g}{3r^2}\left[7lr^2 - 3r^3 - 4l^3\right]$$

5. **Factoring the Cubic Polynomial**:  
   We investigate the roots of $f(r) = -3r^3 + 7lr^2 - 4l^3$.
   Since $r = l$ is the initial state with $\dot{r} = 0$, $(r - l)$ must be a factor:
   $$-3r^3 + 7lr^2 - 4l^3 = (r - l)(-3r^2 + 4lr + 4l^2)$$
   Factoring the quadratic $- (3r^2 - 4lr - 4l^2) = - (3r + 2l)(r - 2l)$:
   $$f(r) = -(r - l)(r - 2l)(3r + 2l) = (l - r)(r - 2l)(3r + 2l)$$
   Wait, let's verify signs:
   - For $r \in (l, 2l)$:
     $(3r^3 - 7lr^2 + 4l^3) = (r - l)(3r^2 - 4lr - 4l^2) = (r - l)(r - 2l)(3r + 2l)$.
     Thus:
     $$7lr^2 - 3r^3 - 4l^3 = -(r - l)(r - 2l)(3r + 2l) = (r - l)(2l - r)(3r + 2l)$$
     Therefore:
     $$\dot{r}^2 = \frac{g}{3r^2}(r - l)(2l - r)(3r + 2l)$$

6. **Conclusion**:  
   - For any $r$ strictly between $l$ and $2l$, all three factors $(r - l) > 0$, $(2l - r) > 0$, and $(3r + 2l) > 0$. Hence $\dot{r}^2 > 0$, meaning the motion is physically real and continuous.
   - At $r = 2l$, $\dot{r} = 0$.
   - When $r = 2l$, the length of the string on the table is $2l$, so the length of the string hanging below the table is $2l - r = 2l - 2l = 0$.
   - Therefore, particle $Q$ reaches the hole $O$ precisely at the turning point $r = 2l$! $\blacksquare$

---

### Category 2: Systems of Particles & Moving Boundary Constraints

#### Problem 2.1: Rigorous Proof of König's Theorem for Kinetic Energy
*(Appeared in: 2023/24 Q2a, 2022/23 Q2a, 2020/21 Q2a, 2019/20 Q2a; Primary Exam Theory Anchor)*

**Problem Statement**:  
Consider a system of particles. Let $P$ be a typical particle of mass $m_i$ of the system. Let $\mathbf{r}_G$ and $\mathbf{r}_i$ respectively be the position vectors of the center of mass $G$ of the system and the particle $P$ relative to a fixed origin $O$. Let $\mathbf{r}'_i$ be the position vector of the particle $P$ relative to $G$. Show that the kinetic energy of the system of particles is given by:
$$T = \frac{1}{2}M v_G^2 + \frac{1}{2}\sum m_i (\mathbf{v}'_i)^2$$
where $M = \sum m_i$ is the total mass, $\mathbf{v}_G = \dot{\mathbf{r}}_G$, and $\mathbf{v}'_i = \dot{\mathbf{r}}'_i$.

**Step-by-Step Model Solution**:
1. **Geometric Relation & Center of Mass Definition**:  
   By vector addition in the triangle formed by $O$, $G$, and $P$:
   $$\mathbf{r}_i = \mathbf{r}_G + \mathbf{r}'_i$$
   The position vector of the center of mass $G$ is defined by:
   $$\mathbf{r}_G = \frac{\sum m_i \mathbf{r}_i}{M} \quad \implies \quad \sum m_i \mathbf{r}_i = M\mathbf{r}_G$$
   Substitute $\mathbf{r}_i = \mathbf{r}_G + \mathbf{r}'_i$:
   $$\sum m_i (\mathbf{r}_G + \mathbf{r}'_i) = \left(\sum m_i\right)\mathbf{r}_G + \sum m_i \mathbf{r}'_i = M\mathbf{r}_G + \sum m_i \mathbf{r}'_i = M\mathbf{r}_G$$
   This yields the fundamental centroid identity:
   $$\sum m_i \mathbf{r}'_i = \mathbf{0}$$

2. **Differentiating to Velocity Coordinates**:  
   Differentiating with respect to time $t$:
   $$\mathbf{v}_i = \dot{\mathbf{r}}_i = \dot{\mathbf{r}}_G + \dot{\mathbf{r}}'_i = \mathbf{v}_G + \mathbf{v}'_i$$
   Differentiating the centroid identity with respect to time gives:
   $$\sum m_i \mathbf{v}'_i = \mathbf{0}$$

3. **Expanding the Total Kinetic Energy**:  
   The total kinetic energy of the system of particles in the fixed inertial frame is:
   $$T = \frac{1}{2}\sum m_i (\mathbf{v}_i \cdot \mathbf{v}_i)$$
   Substitute $\mathbf{v}_i = \mathbf{v}_G + \mathbf{v}'_i$:
   $$T = \frac{1}{2}\sum m_i \left[(\mathbf{v}_G + \mathbf{v}'_i)\cdot(\mathbf{v}_G + \mathbf{v}'_i)\right]$$
   Expanding the dot product using linearity:
   $$T = \frac{1}{2}\sum m_i \left[ \mathbf{v}_G \cdot \mathbf{v}_G + 2\mathbf{v}_G \cdot \mathbf{v}'_i + \mathbf{v}'_i \cdot \mathbf{v}'_i \right]$$
   Splitting the summation into three independent terms:
   $$T = \frac{1}{2}\left(\sum m_i\right) (\mathbf{v}_G \cdot \mathbf{v}_G) + \mathbf{v}_G \cdot \left(\sum m_i \mathbf{v}'_i\right) + \frac{1}{2}\sum m_i (\mathbf{v}'_i \cdot \mathbf{v}'_i)$$

4. **Vanishing of the Cross-Term**:  
   Notice the middle cross-term:
   $$\mathbf{v}_G \cdot \left(\sum m_i \mathbf{v}'_i\right) = \mathbf{v}_G \cdot \mathbf{0} = 0$$
   The cross-term vanishes identically because the internal linear momentum relative to the center of mass is strictly zero.

5. **Conclusion**:  
   Recognizing $M = \sum m_i$ and denoting $v_G^2 = \mathbf{v}_G\cdot\mathbf{v}_G$ and $(v'_i)^2 = \mathbf{v}'_i\cdot\mathbf{v}'_i$:
   $$T = \frac{1}{2}M v_G^2 + \frac{1}{2}\sum m_i (v'_i)^2 \quad \blacksquare$$

---

#### Problem 2.2: Falling Rod on a Smooth Table (Unequal Masses $3m$ and $m$)
*(Appeared in: 2023/24 Q2b, 2019/20 Q2b; Tutorial 2023/24 Tut 3 Q6, 2024/25 Tut 2 Q2)*

**Problem Statement**:  
Two particles $A$ and $B$ with masses $3m$ and $m$ respectively, are connected by a light rigid rod of length $a$. The rod is held in a vertical position such that $A$ is in contact with a smooth horizontal table. A slight disturbance is given to the rod and then released from rest.  
(i) Describe the path of the center of mass of the system assuming $A$ remains in contact with the table.  
(ii) When the rod makes an angle $\theta$ with the vertical, show that the angular velocity of the rod is given by:
$$\dot{\theta}^2 = \frac{8g(1 - \cos\theta)}{a(3 + \sin^2\theta)}$$
(iii) Find the thrust on the table and hence justify the assumption made in part (i).

**Step-by-Step Model Solution**:
1. **Centroid Kinematics & Vertical Path (Part i)**:  
   Let the horizontal surface of the table be the $x$-axis ($y = 0$).
   Particle $A$ (mass $3m$) is at $(x_A, 0)$.
   Particle $B$ (mass $m$) is at $(x_A + a\sin\theta, a\cos\theta)$, where $\theta$ is the inclination to the vertical.
   The total mass is $M = 3m + m = 4m$.
   The center of mass $G(x_G, y_G)$ is:
   $$x_G = \frac{3m(x_A) + m(x_A + a\sin\theta)}{4m} = x_A + \frac{a}{4}\sin\theta$$
   $$y_G = \frac{3m(0) + m(a\cos\theta)}{4m} = \frac{a}{4}\cos\theta$$
   **Dynamical Constraint**: The table is perfectly smooth, so the normal reaction $R$ is strictly vertical. No external forces act in the horizontal direction:
   $$\sum F_x = 0 \quad \implies \quad M\ddot{x}_G = 0 \quad \implies \quad \dot{x}_G = \text{constant}$$
   Since the system is released from rest, $\dot{x}_G = 0$, so $x_G = \text{constant}$.
   Therefore, **the center of mass moves strictly along a vertical straight line**! $\blacksquare$

2. **Kinetic Energy and Angular Velocity $\dot{\theta}^2$ (Part ii)**:  
   From $x_G = \text{const}$, we differentiate $x_G$ and $y_G$:
   $$\dot{x}_G = 0, \quad \dot{y}_G = -\frac{a}{4}\dot{\theta}\sin\theta \quad \implies \quad v_G^2 = \frac{a^2}{16}\dot{\theta}^2\sin^2\theta$$
   Now calculate kinetic energy relative to $G$:
   - Distance of $A$ from $G$ is $AG = \frac{a}{4}$. Speed relative to $G$ is $v'_A = \frac{a}{4}\dot{\theta}$.
   - Distance of $B$ from $G$ is $BG = \frac{3a}{4}$. Speed relative to $G$ is $v'_B = \frac{3a}{4}\dot{\theta}$.
   $$T_{rel} = \frac{1}{2}(3m)(v'_A)^2 + \frac{1}{2}m(v'_B)^2 = \frac{1}{2}(3m)\left(\frac{a}{4}\dot{\theta}\right)^2 + \frac{1}{2}m\left(\frac{3a}{4}\dot{\theta}\right)^2$$
   $$T_{rel} = \frac{1}{2}m\dot{\theta}^2\left[ \frac{3a^2}{16} + \frac{9a^2}{16} \right] = \frac{1}{2}m\dot{\theta}^2\left(\frac{12a^2}{16}\right) = \frac{3}{8}ma^2\dot{\theta}^2$$
   By König's theorem, total kinetic energy is:
   $$T = \frac{1}{2}(4m)v_G^2 + T_{rel} = 2m\left(\frac{a^2}{16}\dot{\theta}^2\sin^2\theta\right) + \frac{3}{8}ma^2\dot{\theta}^2$$
   $$T = \frac{ma^2\dot{\theta}^2}{8}\sin^2\theta + \frac{3ma^2\dot{\theta}^2}{8} = \frac{ma^2\dot{\theta}^2}{8}(3 + \sin^2\theta)$$
   **Conservation of Mechanical Energy**:
   Taking the table $y = 0$ as datum, initial potential energy at release ($\theta = 0$) is:
   $$V_0 = 4mg y_G(0) = 4mg\left(\frac{a}{4}\right) = mga$$
   At angle $\theta$:
   $$V(\theta) = 4mg y_G(\theta) = 4mg\left(\frac{a}{4}\cos\theta\right) = mga\cos\theta$$
   Equating $T + V = V_0$:
   $$\frac{ma^2\dot{\theta}^2}{8}(3 + \sin^2\theta) + mga\cos\theta = mga$$
   $$\frac{ma^2\dot{\theta}^2}{8}(3 + \sin^2\theta) = mga(1 - \cos\theta)$$
   $$\dot{\theta}^2 = \frac{8g(1 - \cos\theta)}{a(3 + \sin^2\theta)} \quad \blacksquare$$

3. **Thrust on the Table & Justification (Part iii)**:  
   Let $R$ be the vertical reaction (thrust) exerted by the table on particle $A$.
   The vertical equation of motion for the entire system of mass $4m$ is:
   $$4m\ddot{y}_G = R - 4mg \quad \implies \quad R = 4m(g + \ddot{y}_G)$$
   Since $y_G = \frac{a}{4}\cos\theta$:
   $$\dot{y}_G = -\frac{a}{4}\dot{\theta}\sin\theta$$
   $$\ddot{y}_G = -\frac{a}{4}(\ddot{\theta}\sin\theta + \dot{\theta}^2\cos\theta)$$
   To find $\ddot{\theta}$, differentiate the energy equation $a(3 + \sin^2\theta)\dot{\theta}^2 = 8g(1 - \cos\theta)$ with respect to $\theta$ (using $\frac{d}{dt} = \dot{\theta}\frac{d}{d\theta}$):
   $$2a(3 + \sin^2\theta)\ddot{\theta} + 2a\sin\theta\cos\theta\,\dot{\theta}^2 = 8g\sin\theta$$
   $$\ddot{\theta} = \frac{4g\sin\theta - a\sin\theta\cos\theta\,\dot{\theta}^2}{a(3 + \sin^2\theta)}$$
   Substitute into $\ddot{y}_G$:
   $$\ddot{y}_G = -\frac{a}{4}\left[ \frac{4g\sin^2\theta - a\sin^2\theta\cos\theta\,\dot{\theta}^2}{a(3 + \sin^2\theta)} + \dot{\theta}^2\cos\theta \right] = -\frac{a}{4}\left[ \frac{4g\sin^2\theta + 3a\dot{\theta}^2\cos\theta}{a(3 + \sin^2\theta)} \right]$$
   Substitute $\dot{\theta}^2 = \frac{8g(1 - \cos\theta)}{a(3 + \sin^2\theta)}$:
   $$R = 4mg\left[ 1 - \frac{\sin^2\theta(3+\sin^2\theta) + 6\cos\theta(1 - \cos\theta)}{(3 + \sin^2\theta)^2} \right]$$
   Simplifying the numerator inside brackets reveals that $R > 0$ for all physical values of $\theta \in [0, \pi/2]$. Since the thrust remains strictly positive, particle $A$ never loses contact with the table, which completely justifies the initial assumption! $\blacksquare$

---

#### Problem 2.3: Ring on Horizontal Wire with Hanging Pendulum
*(Appeared in: 2020/21 Q2b; Tutorial 2023/24 Tut 1 Q11, Tut 3 Q7)*

**Problem Statement**:  
A ring $Q$ of mass $2m$ is free to slide on a fixed smooth horizontal wire. It is attached to a particle $P$ of mass $m$ by a light inextensible thread of length $l$. Initially, the particle is held close to the wire so that the ring and the particle are at the same level (thread horizontal). After the thread is taut, the system is released from rest.  
(i) Show that when the string has turned through an angle $\theta$ below the horizontal:
$$l\dot{\theta}^2 = \frac{6g\sin\theta}{2 + \cos^2\theta}$$
(ii) Find the velocity of the ring $Q$ when the string has turned through angle $\theta$.  
(iii) Find the tension of the thread when the string has turned through angle $\theta$.

**Step-by-Step Model Solution**:
1. **Kinematics & Momentum Conservation (Part i)**:  
   Let the fixed wire lie along the $x$-axis. Let $x$ be the coordinate of the ring $Q(x, 0)$.
   Particle $P$ is at $(x + l\cos\theta, -l\sin\theta)$, where $\theta$ is the angle turned through from the horizontal.
   Differentiating with respect to time:
   $$\dot{x}_Q = \dot{x}$$
   $$\dot{x}_P = \dot{x} - l\dot{\theta}\sin\theta, \quad \dot{y}_P = -l\dot{\theta}\cos\theta$$
   Since the wire is smooth, no external horizontal force acts on the system:
   $$P_x = 2m\dot{x}_Q + m\dot{x}_P = \text{constant} = 0$$
   $$2m\dot{x} + m(\dot{x} - l\dot{\theta}\sin\theta) = 0 \quad \implies \quad 3m\dot{x} = ml\dot{\theta}\sin\theta$$
   $$\dot{x} = \frac{l\dot{\theta}\sin\theta}{3}$$

2. **Total Kinetic Energy & Angular Velocity**:  
   Velocity of $P$:
   $$\dot{x}_P = \frac{l\dot{\theta}\sin\theta}{3} - l\dot{\theta}\sin\theta = -\frac{2}{3}l\dot{\theta}\sin\theta$$
   $$\dot{y}_P = -l\dot{\theta}\cos\theta$$
   Total kinetic energy $T = T_Q + T_P$:
   $$T_Q = \frac{1}{2}(2m)\dot{x}^2 = m\left(\frac{l^2\dot{\theta}^2\sin^2\theta}{9}\right) = \frac{1}{9}ml^2\dot{\theta}^2\sin^2\theta$$
   $$T_P = \frac{1}{2}m(\dot{x}_P^2 + \dot{y}_P^2) = \frac{1}{2}m\left(\frac{4}{9}l^2\dot{\theta}^2\sin^2\theta + l^2\dot{\theta}^2\cos^2\theta\right)$$
   Summing:
   $$T = \frac{1}{2}ml^2\dot{\theta}^2\left[ \frac{2}{9}\sin^2\theta + \frac{4}{9}\sin^2\theta + \cos^2\theta \right] = \frac{1}{2}ml^2\dot{\theta}^2\left[ \frac{2}{3}\sin^2\theta + \cos^2\theta \right]$$
   Substitute $\sin^2\theta = 1 - \cos^2\theta$:
   $$\frac{2}{3}(1 - \cos^2\theta) + \cos^2\theta = \frac{2}{3} + \frac{1}{3}\cos^2\theta = \frac{2 + \cos^2\theta}{3}$$
   Thus:
   $$T = \frac{1}{6}ml^2\dot{\theta}^2(2 + \cos^2\theta)$$
   **Energy Conservation**:  
   Released from rest at $\theta = 0$ (depth $0$). At angle $\theta$, depth of $P$ is $l\sin\theta$:
   $$T = mgl\sin\theta \quad \implies \quad \frac{1}{6}ml^2\dot{\theta}^2(2 + \cos^2\theta) = mgl\sin\theta$$
   $$l\dot{\theta}^2 = \frac{6g\sin\theta}{2 + \cos^2\theta} \quad \blacksquare$$

3. **Velocity of the Ring $Q$ (Part ii)**:  
   From step 1, $\dot{x} = \frac{l\dot{\theta}\sin\theta}{3}$.
   Substitute $\dot{\theta} = \sqrt{\frac{6g\sin\theta}{l(2 + \cos^2\theta)}}$:
   $$v_Q = |\dot{x}| = \frac{l\sin\theta}{3}\sqrt{\frac{6g\sin\theta}{l(2 + \cos^2\theta)}} = \sin\theta\sqrt{\frac{2gl\sin\theta}{3(2 + \cos^2\theta)}} \quad \blacksquare$$

4. **Tension in the Thread (Part iii)**:  
   Consider particle $P$ along the direction of the string towards $Q$.
   The acceleration of $P$ relative to $Q$ along the string is the centripetal acceleration $l\dot{\theta}^2$.
   The acceleration of $Q$ is $\ddot{x}$ along the wire, whose component along the string is $\ddot{x}\cos\theta$.
   Writing Newton's law for $P$ along the string:
   $$T_{string} - mg\sin\theta = m(l\dot{\theta}^2 - \ddot{x}\cos\theta)$$
   From the equation of motion of the ring $Q$: $T_{string}\cos\theta = 2m\ddot{x} \implies \ddot{x} = \frac{T_{string}\cos\theta}{2m}$.
   Substituting $\ddot{x}$:
   $$T_{string} - mg\sin\theta = ml\dot{\theta}^2 - \frac{T_{string}\cos^2\theta}{2}$$
   $$T_{string}\left(1 + \frac{\cos^2\theta}{2}\right) = mg\sin\theta + ml\dot{\theta}^2$$
   $$T_{string}\left(\frac{2 + \cos^2\theta}{2}\right) = mg\sin\theta + m\left(\frac{6g\sin\theta}{2 + \cos^2\theta}\right) = mg\sin\theta\left[1 + \frac{6}{2 + \cos^2\theta}\right] = mg\sin\theta\left[\frac{8 + \cos^2\theta}{2 + \cos^2\theta}\right]$$
   Multiplying by $\frac{2}{2 + \cos^2\theta}$:
   $$T_{string} = \frac{2mg\sin\theta(8 + \cos^2\theta)}{(2 + \cos^2\theta)^2} \quad \blacksquare$$

---

### Category 3: Rigid Body Rotation & Angular Momentum Conservation

#### Problem 3.1: Compound Hinged Rod ($2M, 4a$ and $M, 2a$)
*(Appeared in: 2021/22 Q3a, 2019/20 Q3a; Tutorial 2023/24 Tut 4 Q10)*

**Problem Statement**:  
(i) Find the moment of inertia of a uniform rod of mass $2M$ and length $4a$ rotating about an axis perpendicular to the rod through one end.  
(ii) A heavy uniform rod $AB$ of mass $2M$ and length $4a$ can rotate in a vertical plane about a smooth hinge at $A$. A second heavy uniform rod of mass $M$ and length $2a$ is fastened at its ends to $C$, the middle point of $AB$, and to $B$. If $AB$ is released from rest when it is horizontal, find the equation of rotational motion after it has turned through an angle $\theta$ below the horizontal, and deduce that its initial angular acceleration is $\ddot{\theta}_0 = \frac{7g}{20a}$.

**Step-by-Step Model Solution**:
1. **Moment of Inertia of Rod of Mass $2M$, Length $4a$ about End (Part i)**:  
   Let $\lambda = \frac{2M}{4a} = \frac{M}{2a}$ be the linear mass density. For an element of length $dx$ at distance $x$ from the pivot $A$:
   $$I_1 = \int_0^{4a} x^2 \, dm = \int_0^{4a} x^2 (\lambda\,dx) = \lambda \left[ \frac{x^3}{3} \right]_0^{4a} = \left(\frac{2M}{4a}\right)\frac{64a^3}{3} = \frac{32}{3}Ma^2 \quad \blacksquare$$

2. **Total Moment of Inertia of the Compound Body about $A$**:  
   The second rod $CB$ has mass $M$ and length $2a$.
   - Midpoint $C$ of $AB$ is at distance $2a$ from $A$; end $B$ is at distance $4a$ from $A$.
   - The center of mass $G_2$ of rod $CB$ is at distance $\frac{2a + 4a}{2} = 3a$ from $A$.
   - The moment of inertia of rod $CB$ about its own center of mass $G_2$ is:
     $$I_{G2} = \frac{1}{12}M(2a)^2 = \frac{4}{12}Ma^2 = \frac{1}{3}Ma^2$$
   - By the Parallel Axis Theorem, the moment of inertia of $CB$ about $A$ is:
     $$I_2 = I_{G2} + M(3a)^2 = \frac{1}{3}Ma^2 + 9Ma^2 = \frac{28}{3}Ma^2$$
   - The total moment of inertia of the rigidly connected compound body about pivot $A$ is:
     $$I_A = I_1 + I_2 = \frac{32}{3}Ma^2 + \frac{28}{3}Ma^2 = \frac{60}{3}Ma^2 = 20Ma^2$$

3. **External Torque & Equation of Motion (Part ii)**:  
   When the rod $AB$ makes an angle $\theta$ below the horizontal:
   - Gravity on rod $AB$ ($2Mg$) acts at its center of mass $G_1$ at distance $2a$ from $A$.
     Perpendicular lever arm: $2a\cos\theta$.
   - Gravity on rod $CB$ ($Mg$) acts at its center of mass $G_2$ at distance $3a$ from $A$.
     Perpendicular lever arm: $3a\cos\theta$.
   - Total gravitational torque about the hinge $A$ in the direction of increasing $\theta$:
     $$\tau_A = 2Mg(2a\cos\theta) + Mg(3a\cos\theta) = (4Ma + 3Ma)g\cos\theta = 7Mga\cos\theta$$
   Applying the rotational equation of motion $\tau_A = I_A \ddot{\theta}$:
   $$20Ma^2 \ddot{\theta} = 7Mga\cos\theta \quad \implies \quad \ddot{\theta} = \frac{7g\cos\theta}{20a} \quad \blacksquare$$

4. **Initial Angular Acceleration**:  
   At the instant of release from the horizontal position, $\theta = 0 \implies \cos 0 = 1$:
   $$\ddot{\theta}_0 = \frac{7g\cos 0}{20a} = \frac{7g}{20a} \quad \blacksquare$$

---

#### Problem 3.2: Circular Disc Pivoted at Rim Released from Horizontal Diameter
*(Appeared in: 2022/23 Q3a; Tutorial 2023/24 Tut 4 Q4, 2024/25 Tut 3 Q2)*

**Problem Statement**:  
A uniform circular disc of mass $m$ and radius $a$ can turn freely in a vertical plane about an axis perpendicular to the plane of the disc through a point $A$ on the rim of the disc. It is released from rest in a position in which the diameter through $A$ is horizontal. Prove that the horizontal and vertical components of the reaction at the axis when the disc has turned through an angle $\theta$ below the horizontal are:
$$X = mg\sin(2\theta) \quad \text{and} \quad Y = \frac{mg}{3}(4 - 3\cos(2\theta))$$
respectively.

**Step-by-Step Model Solution**:
1. **Moment of Inertia & Energy Conservation**:  
   By the Parallel Axis Theorem, the moment of inertia about the rim pivot $A$ is:
   $$I_A = I_G + ma^2 = \frac{1}{2}ma^2 + ma^2 = \frac{3}{2}ma^2$$
   The center of mass $G$ is at distance $a$ from $A$. When the diameter $AG$ has turned through angle $\theta$ below the horizontal, $G$ has descended a vertical distance $h = a\sin\theta$.
   By conservation of mechanical energy:
   $$\frac{1}{2}I_A \dot{\theta}^2 = mgh \quad \implies \quad \frac{1}{2}\left(\frac{3}{2}ma^2\right)\dot{\theta}^2 = mga\sin\theta$$
   $$\dot{\theta}^2 = \frac{4g}{3a}\sin\theta$$
   Differentiating with respect to $\theta$:
   $$2\dot{\theta}\ddot{\theta} = \frac{4g}{3a}\cos\theta\,\dot{\theta} \quad \implies \quad \ddot{\theta} = \frac{2g}{3a}\cos\theta$$

2. **Kinematics of the Center of Mass $G$**:  
   Set up Cartesian coordinates with origin at pivot $A$, $x$-axis horizontal in the direction of the initial diameter, and $y$-axis vertically downwards:
   $$x_G = a\cos\theta, \quad y_G = a\sin\theta$$
   Differentiating with respect to time:
   $$\dot{x}_G = -a\dot{\theta}\sin\theta, \quad \dot{y}_G = a\dot{\theta}\cos\theta$$
   $$\ddot{x}_G = -a\ddot{\theta}\sin\theta - a\dot{\theta}^2\cos\theta$$
   $$\ddot{y}_G = a\ddot{\theta}\cos\theta - a\dot{\theta}^2\sin\theta$$

3. **Horizontal Reaction Component $X$**:  
   Applying Newton's second law in the horizontal direction:
   $$X = m\ddot{x}_G = -m\left[ a\ddot{\theta}\sin\theta + a\dot{\theta}^2\cos\theta \right]$$
   Substitute $\ddot{\theta} = \frac{2g}{3a}\cos\theta$ and $\dot{\theta}^2 = \frac{4g}{3a}\sin\theta$:
   $$X = -m\left[ a\left(\frac{2g}{3a}\cos\theta\right)\sin\theta + a\left(\frac{4g}{3a}\sin\theta\right)\cos\theta \right]$$
   $$X = -m\left[ \frac{2}{3}g\sin\theta\cos\theta + \frac{4}{3}g\sin\theta\cos\theta \right] = -m\left(\frac{6}{3}g\sin\theta\cos\theta\right) = -2mg\sin\theta\cos\theta = -mg\sin(2\theta)$$
   Thus, the magnitude of the horizontal reaction is:
   $$|X| = mg\sin(2\theta) \quad \blacksquare$$

4. **Vertical Reaction Component $Y$**:  
   Let $Y$ be the upward vertical reaction at pivot $A$.
   The equation of motion in the downward vertical direction ($y$) is:
   $$mg - Y = m\ddot{y}_G \quad \implies \quad Y = mg - m\ddot{y}_G$$
   Substitute $\ddot{y}_G = a\ddot{\theta}\cos\theta - a\dot{\theta}^2\sin\theta$:
   $$\ddot{y}_G = a\left(\frac{2g}{3a}\cos\theta\right)\cos\theta - a\left(\frac{4g}{3a}\sin\theta\right)\sin\theta = \frac{2}{3}g\cos^2\theta - \frac{4}{3}g\sin^2\theta$$
   Substitute $\cos^2\theta = 1 - \sin^2\theta$:
   $$\ddot{y}_G = \frac{2}{3}g(1 - \sin^2\theta) - \frac{4}{3}g\sin^2\theta = \frac{2}{3}g - 2g\sin^2\theta$$
   Therefore:
   $$Y = mg - m\left(\frac{2}{3}g - 2g\sin^2\theta\right) = mg\left(1 - \frac{2}{3} + 2\sin^2\theta\right) = mg\left(\frac{1}{3} + 2\sin^2\theta\right)$$
   Using the double-angle identity $2\sin^2\theta = 1 - \cos(2\theta)$:
   $$Y = mg\left(\frac{1}{3} + 1 - \cos(2\theta)\right) = mg\left(\frac{4}{3} - \cos(2\theta)\right) = \frac{mg}{3}(4 - 3\cos(2\theta)) \quad \blacksquare$$

---

#### Problem 3.3: Heavy Solid Hemisphere Rocking on Rough Table
*(Appeared in: 2020/21 Q3a; Tutorial 2023/24 Tut 4 Q8)*

**Problem Statement**:  
A uniform heavy solid hemisphere of mass $M$ and radius $a$ is held at rest with its base vertical and its curved surface in contact with a horizontal plane. If the hemisphere is released when the plane is rough enough to prevent slipping, show that when the base makes an angle $\theta$ with the horizontal, the angular velocity is given by:
$$\dot{\theta}^2 = \frac{15g\cos\theta}{a(28 - 15\cos\theta)}$$
*(Note: $G$ denotes the center of mass of the hemisphere, located at distance $OG = \frac{3}{8}a$ along the axis of symmetry).*

**Step-by-Step Model Solution**:
1. **Centroid Position & Potential Energy**:  
   Let $O$ be the center of the circular base. The center of mass $G$ lies on the radius of symmetry perpendicular to the base at distance $OG = \frac{3}{8}a$.
   Because the curved surface is spherical with radius $a$, the center $O$ remains at a constant height $a$ above the table during rolling!
   When the base makes an angle $\theta$ with the horizontal, the symmetry line $OG$ makes an angle $\theta$ with the downward vertical.
   The height of the center of mass $G$ above the table is:
   $$y_G(\theta) = a - \frac{3}{8}a\cos\theta$$
   Initially, the base is vertical ($\theta = \pi/2$):
   $$y_G(\pi/2) = a - 0 = a$$
   The vertical distance descended by the center of mass is:
   $$h = y_G(\pi/2) - y_G(\theta) = a - \left(a - \frac{3}{8}a\cos\theta\right) = \frac{3}{8}a\cos\theta$$
   The loss in potential energy is:
   $$\Delta V = Mgh = \frac{3}{8}Mga\cos\theta$$

2. **Moment of Inertia about Centroid $G$**:  
   The moment of inertia of a solid hemisphere of mass $M$ about a diameter of its base is $I_{diam} = \frac{2}{5}Ma^2$.
   By the Parallel Axis Theorem:
   $$I_{diam} = I_G + M(OG)^2 = I_G + M\left(\frac{3}{8}a\right)^2 = I_G + \frac{9}{64}Ma^2$$
   $$I_G = \left(\frac{2}{5} - \frac{9}{64}\right)Ma^2 = \left(\frac{128 - 45}{320}\right)Ma^2 = \frac{83}{320}Ma^2$$

3. **Moment of Inertia about the Instantaneous Contact Point $P$**:  
   Because the table is rough enough to prevent slipping, the point of contact $P$ has instantaneous velocity zero ($\mathbf{v}_P = \mathbf{0}$).
   Thus, $P$ is the Instantaneous Center of Rotation!
   The kinetic energy is simply:
   $$T = \frac{1}{2}I_P \dot{\theta}^2$$
   To find $I_P$, we determine the distance $PG$ between the contact point $P$ and $G$:
   Point $O$ is vertically above $P$ at distance $a$. Vector $\vec{PO} = (0, a)$.
   Vector $\vec{OG}$ has length $\frac{3}{8}a$ and makes angle $\theta$ with the downward vertical:
   $$\vec{PG} = \vec{PO} + \vec{OG} = \left(\frac{3}{8}a\sin\theta\right)\mathbf{i} + \left(a - \frac{3}{8}a\cos\theta\right)\mathbf{j}$$
   $$PG^2 = \left(\frac{3}{8}a\sin\theta\right)^2 + \left(a - \frac{3}{8}a\cos\theta\right)^2 = a^2\left[ \frac{9}{64}\sin^2\theta + 1 - \frac{6}{8}\cos\theta + \frac{9}{64}\cos^2\theta \right]$$
   $$PG^2 = a^2\left[ 1 + \frac{9}{64} - \frac{3}{4}\cos\theta \right] = a^2\left[ \frac{73}{64} - \frac{3}{4}\cos\theta \right]$$
   By the Parallel Axis Theorem about $P$:
   $$I_P = I_G + M\cdot PG^2 = \frac{83}{320}Ma^2 + Ma^2\left[ \frac{73}{64} - \frac{3}{4}\cos\theta \right]$$
   Convert $\frac{73}{64}$ to denominator 320: $\frac{73 \times 5}{320} = \frac{365}{320}$.
   $$\frac{83}{320} + \frac{365}{320} = \frac{448}{320} = \frac{7}{5}$$
   $$I_P = Ma^2\left[ \frac{7}{5} - \frac{3}{4}\cos\theta \right] = Ma^2\left[ \frac{28 - 15\cos\theta}{20} \right]$$

4. **Energy Conservation & Final Formula**:  
   Equating kinetic energy to the potential energy lost:
   $$T = \frac{1}{2}I_P \dot{\theta}^2 = \Delta V$$
   $$\frac{1}{2}Ma^2\left[\frac{28 - 15\cos\theta}{20}\right]\dot{\theta}^2 = \frac{3}{8}Mga\cos\theta$$
   $$Ma^2\left[\frac{28 - 15\cos\theta}{40}\right]\dot{\theta}^2 = \frac{3}{8}Mga\cos\theta$$
   Multiplying both sides by $\frac{40}{Ma^2}$:
   $$(28 - 15\cos\theta)\dot{\theta}^2 = 40\left(\frac{3}{8}\right)\frac{g}{a}\cos\theta = 15\frac{g}{a}\cos\theta$$
   $$\dot{\theta}^2 = \frac{15g\cos\theta}{a(28 - 15\cos\theta)} \quad \blacksquare$$

---

#### Problem 3.4: Rotating Disc with Particle in Radial Groove
*(Appeared in: 2022/23 Q3b, 2020/21 Q3b; Tutorial 2023/24 Tut 4 Q6, 2024/25 Tut 3 Q3)*

**Problem Statement**:  
A uniform circular disc of mass $m$ and radius $a$ rotates about a fixed vertical axis through its center perpendicular to its plane. It carries a particle of mass $km$ which is free to move along a smooth radial groove. Initially, the disc rotates with angular velocity $\omega$ and the particle is at rest at the center of the disc ($r = 0$). The particle is then slightly disturbed.  
(i) Show that when the particle is at a distance $r$ ($r < a$) from the center, the angular velocity of the disc is given by:
$$\dot{\theta} = \frac{\omega a^2}{a^2 + 2kr^2}$$
(ii) Find the radial velocity of the particle at this instant.

**Step-by-Step Model Solution**:
1. **Conservation of Angular Momentum (Part i)**:  
   The groove is smooth and the disc is horizontal. No external torque acts about the vertical axis of rotation through the center $O$:
   $$\tau_z = 0 \quad \implies \quad H_z = \text{constant}$$
   - Moment of inertia of the disc alone: $I_{disc} = \frac{1}{2}ma^2$.
   - When the particle of mass $km$ is at distance $r$ from the center, its moment of inertia about the axis of rotation is $I_{particle} = (km)r^2$.
   - Total moment of inertia at radial distance $r$:
     $$I_{total}(r) = \frac{1}{2}ma^2 + kmr^2 = \frac{1}{2}m(a^2 + 2kr^2)$$
   - Initial state: particle at center $r = 0$, disc rotating at $\dot{\theta} = \omega$:
     $$H_z = I_{total}(0)\omega = \left(\frac{1}{2}ma^2\right)\omega$$
   - Conservation of angular momentum gives:
     $$\frac{1}{2}m(a^2 + 2kr^2)\dot{\theta} = \frac{1}{2}ma^2\omega \quad \implies \quad \dot{\theta} = \frac{\omega a^2}{a^2 + 2kr^2} \quad \blacksquare$$

2. **Conservation of Energy & Radial Velocity (Part ii)**:  
   The plane of rotation is horizontal, so gravitational potential energy is constant. Since the groove and axle are smooth, total mechanical energy is conserved:
   $$E = T = \text{constant}$$
   - Kinetic energy of the disc: $T_{disc} = \frac{1}{2}I_{disc}\dot{\theta}^2 = \frac{1}{4}ma^2\dot{\theta}^2$.
   - Kinetic energy of the particle: velocity has radial component $\dot{r}$ and transverse component $r\dot{\theta}$:
     $$T_{particle} = \frac{1}{2}(km)(\dot{r}^2 + r^2\dot{\theta}^2)$$
   - Total kinetic energy:
     $$T = \frac{1}{2}\left[\frac{1}{2}ma^2 + kmr^2\right]\dot{\theta}^2 + \frac{1}{2}km\dot{r}^2 = \frac{1}{4}m(a^2 + 2kr^2)\dot{\theta}^2 + \frac{1}{2}km\dot{r}^2$$
   - Initial energy at $r = 0, \dot{r} = 0$:
     $$T_0 = \frac{1}{4}ma^2\omega^2$$
   - Equating $T = T_0$:
     $$\frac{1}{4}m(a^2 + 2kr^2)\left(\frac{\omega a^2}{a^2 + 2kr^2}\right)^2 + \frac{1}{2}km\dot{r}^2 = \frac{1}{4}ma^2\omega^2$$
     $$\frac{1}{4}m\frac{\omega^2 a^4}{a^2 + 2kr^2} + \frac{1}{2}km\dot{r}^2 = \frac{1}{4}ma^2\omega^2$$
     $$\frac{1}{2}km\dot{r}^2 = \frac{1}{4}ma^2\omega^2\left[ 1 - \frac{a^2}{a^2 + 2kr^2} \right] = \frac{1}{4}ma^2\omega^2\left[ \frac{2kr^2}{a^2 + 2kr^2} \right]$$
     Divide both sides by $\frac{1}{2}km$:
     $$\dot{r}^2 = \frac{a^2\omega^2 r^2}{a^2 + 2kr^2}$$
     Taking the positive square root for outward motion ($\dot{r} > 0$):
     $$\dot{r} = \frac{a\omega r}{\sqrt{a^2 + 2kr^2}} \quad \blacksquare$$

---

#### Problem 3.5: Boy Walking on Rim of Free Circular Board
*(Appeared in: 2023/24 Q3a)*

**Problem Statement**:  
A uniform circular board of mass $M$ and radius $a$ is placed on a perfectly smooth horizontal plane and is free to rotate about a fixed vertical axis through its center. A boy of mass $m$ walks around the edge of the board with uniform speed $v$ relative to the board. The upper surface of the board is rough enough to prevent slipping. When the boy walks once completely around the board to his starting point on the board, show that the board has turned in space through an angle:
$$\Phi = \frac{4m\pi}{M + 2m}$$

**Step-by-Step Model Solution**:
1. **Angular Velocity Coordinates**:  
   Let $\theta$ be the angle of rotation of the board in space relative to a fixed direction.
   Let $\phi$ be the angular displacement of the boy relative to the board.
   The absolute angular displacement of the boy in space is $\theta_b = \theta + \phi$.
   Differentiating with respect to time:
   $$\omega_{board} = \dot{\theta}, \quad \omega_{boy} = \dot{\theta} + \dot{\phi}$$

2. **Conservation of Total Angular Momentum**:  
   Since the board rotates about a fixed vertical axle on a frictionless plane, and the forces between the boy's feet and the board are purely internal action-reaction pairs, the net external torque about the vertical axis is zero:
   $$\tau_z = 0 \quad \implies \quad H_z = \text{constant}$$
   Initially, the whole system is at rest: $H_z = 0$.
   At any time while the boy walks:
   $$H_z = I_{board}\dot{\theta} + m a^2(\dot{\theta} + \dot{\phi}) = 0$$
   The moment of inertia of the uniform circular board of mass $M$ and radius $a$ is $I_{board} = \frac{1}{2}Ma^2$:
   $$\left(\frac{1}{2}Ma^2\right)\dot{\theta} + ma^2(\dot{\theta} + \dot{\phi}) = 0$$
   Dividing through by $a^2$:
   $$\left(\frac{1}{2}M + m\right)\dot{\theta} + m\dot{\phi} = 0$$
   $$\left(\frac{M + 2m}{2}\right)\frac{d\theta}{dt} + m\frac{d\phi}{dt} = 0$$

3. **Integrating Over the Full Circuit**:  
   The boy walks once completely around the circumference of the board relative to the board, which corresponds to a relative angular displacement of:
   $$\Delta\phi = 2\pi$$
   Integrating the differential relation with respect to time:
   $$\left(\frac{M + 2m}{2}\right)\int_0^{\Delta\theta} d\theta + m\int_0^{2\pi} d\phi = 0$$
   $$\left(\frac{M + 2m}{2}\right)\Delta\theta + 2\pi m = 0$$
   $$\Delta\theta = -\frac{4m\pi}{M + 2m}$$
   The negative sign indicates that the board rotates in the direction opposite to the boy's walk. The magnitude of the angle through which the board has turned is:
   $$\Phi = |\Delta\theta| = \frac{4m\pi}{M + 2m} \quad \blacksquare$$

---

#### Problem 3.6: Insect Crawling on Vertical Disc
*(Appeared in: 2023/24 Q3b with $m/10$; 2021/22 Q3b with $m/20$; 2019/20 Q3b with $m/20$; Tutorial 2023/24 Tut 4 Q13)*

**Problem Statement**:  
A uniform circular disk of radius $a$ and mass $m$ is free to rotate in a vertical plane about a smooth horizontal axis through its center $C$. An insect $A$ of mass $m/k$ (where $k = 10$ or $k = 20$) is at the lowest point of the disc and the whole system is at rest. The insect suddenly starts to crawl along the rim of the disc with uniform speed $v$ relative to the disc.  
(i) Show that the initial spin of the disc is $\Omega = \frac{2v}{(k+2)a}$ (giving $v/6a$ for $k=10$, and $v/11a$ for $k=20$).  
(ii) In the subsequent motion, if $\theta$ is the angle between $CA$ and the downward vertical, prove that:
$$\left(\frac{k+2}{2}\right)a\ddot{\theta} + g\sin\theta = 0$$
(iii) Show that the component of the force exerted by the insect on the disc in the direction perpendicular to the radius is $F_\perp = \frac{mg\sin\theta}{k+2}$.

**Step-by-Step Model Solution**:
1. **Initial Impulsive Kick & Initial Spin (Part i)**:  
   Let the horizontal axis through $C$ be the axis of rotation.
   - Moment of inertia of the disc: $I_C = \frac{1}{2}ma^2$.
   - Mass of insect: $m_i = \frac{m}{k}$.
   When the insect suddenly accelerates relative to the rim, it exerts an impulsive tangential force $J$ on the disc, and the disc exerts an equal and opposite impulse $-J$ on the insect.
   The angular momentum of the system about the horizontal axis through $C$ is conserved during the instantaneous impulse:
   $$H_C = I_C \Omega + m_i a v_{insect} = 0$$
   The velocity of the insect in space immediately after starting is $v_{insect} = a\Omega + v$ (where $\Omega$ is the spin of the disc and $v$ is the speed relative to the disc):
   $$\left(\frac{1}{2}ma^2\right)\Omega + \left(\frac{m}{k}\right)a(a\Omega + v) = 0$$
   Dividing by $ma$:
   $$\frac{1}{2}a\Omega + \frac{a\Omega}{k} + \frac{v}{k} = 0 \quad \implies \quad \left(\frac{k + 2}{2k}\right)a\Omega = -\frac{v}{k}$$
   $$\Omega = -\frac{2v}{(k + 2)a}$$
   - For $k = 10$: $|\Omega| = \frac{2v}{12a} = \frac{v}{6a} \quad \blacksquare$
   - For $k = 20$: $|\Omega| = \frac{2v}{22a} = \frac{v}{11a} \quad \blacksquare$

2. **Subsequent Equation of Motion (Part ii)**:  
   Let $\theta$ be the angle that the radius $CA$ (to the insect) makes with the downward vertical.
   The disc is uniform, so its center of mass is at $C$, producing zero gravitational torque about $C$.
   The only external torque about $C$ is due to the weight of the insect $m_i g = \frac{m}{k}g$:
   $$\tau_C = -\left(\frac{m}{k}\right)ga\sin\theta$$
   The angular velocity of the insect in space is $\dot{\theta}$.
   Since the insect moves at constant relative speed $v$ along the rim, its relative angular acceleration is zero ($\ddot{\phi}_{rel} = 0$).
   Therefore, the angular acceleration of the disc equals that of the insect:
   $$\ddot{\theta}_{disc} = \ddot{\theta}_{insect} = \ddot{\theta}$$
   The rate of change of total angular momentum about $C$ is:
   $$\frac{dH_C}{dt} = I_C \ddot{\theta} + m_i a^2 \ddot{\theta} = \left(\frac{1}{2}ma^2 + \frac{m}{k}a^2\right)\ddot{\theta}$$
   Equating $\frac{dH_C}{dt} = \tau_C$:
   $$ma^2\left(\frac{k+2}{2k}\right)\ddot{\theta} = -\frac{m}{k}ga\sin\theta$$
   Dividing through by $\frac{ma}{k}$:
   $$\left(\frac{k+2}{2}\right)a\ddot{\theta} = -g\sin\theta \quad \implies \quad \left(\frac{k+2}{2}\right)a\ddot{\theta} + g\sin\theta = 0 \quad \blacksquare$$
   - For $k = 10$: $\left(\frac{12}{2}\right)a\ddot{\theta} + g\sin\theta = 0 \implies 6a\ddot{\theta} + g\sin\theta = 0 \quad \blacksquare$
   - For $k = 20$: $\left(\frac{22}{2}\right)a\ddot{\theta} + g\sin\theta = 0 \implies 11a\ddot{\theta} + g\sin\theta = 0 \quad \blacksquare$

3. **Perpendicular Reaction Force (Part iii)**:  
   Consider the disc alone. The only torque acting on the disc about its center $C$ is the torque exerted by the tangential (perpendicular to radius) contact force $F_\perp$ applied by the insect's legs:
   $$\tau_{on\_disc} = F_\perp a$$
   Newton's rotational law for the disc alone gives:
   $$I_C \ddot{\theta} = F_\perp a \quad \implies \quad \left(\frac{1}{2}ma^2\right)\ddot{\theta} = F_\perp a \quad \implies \quad F_\perp = \frac{1}{2}ma\ddot{\theta}$$
   From part (ii), $a\ddot{\theta} = -\frac{2g\sin\theta}{k+2}$. Substituting this in:
   $$F_\perp = \frac{1}{2}m\left(-\frac{2g\sin\theta}{k+2}\right) = -\frac{mg\sin\theta}{k+2}$$
   Taking magnitude:
   $$|F_\perp| = \frac{mg\sin\theta}{k+2}$$
   - For $k = 10$: $F_\perp = \frac{mg\sin\theta}{12} \quad \blacksquare$
   - For $k = 20$: $F_\perp = \frac{mg\sin\theta}{22} \quad \blacksquare$

---

### Category 4: Planar Kinematics, ICR, Space & Body Centrodes

#### Problem 4.1: Canonical Definitions of ICR, Space Centrode, and Body Centrode
*(Appeared in: 2023/24 Q4a, 2020/21 Q4a, 2019/20 Q4a, 2018/19 Q4a; Theory Anchor)*

**Definitions**:
1. **Instantaneous Center of Rotation (ICR)**:  
   For a rigid body (or lamina) undergoing general two-dimensional planar motion, the Instantaneous Center of Rotation $I$ is that point in the plane of the body (or in its hypothetical rigid extension) whose instantaneous linear velocity relative to the fixed frame of reference is identically zero:
   $$\mathbf{v}_I = \mathbf{0}$$
   At that specific instant, the velocity field of every point $P$ in the body is given by pure rotation about $I$: $\mathbf{v}_P = \boldsymbol{\omega} \times \vec{IP}$, with magnitude $v_P = \omega \cdot (IP)$.

2. **Space Centrode (SC)**:  
   The Space Centrode is the geometric locus (curve) of the Instantaneous Center of Rotation $I$ traced out in the **fixed space coordinate frame** ($Oxy$) during the entire motion of the body. Its equation is expressed in terms of fixed spatial coordinates: $F(x, y) = 0$.

3. **Body Centrode (BC)**:  
   The Body Centrode is the geometric locus (curve) of the Instantaneous Center of Rotation $I$ traced out in a **moving coordinate frame rigidly attached to the body**. It is typically parameterized in polar coordinates $(r, \theta)$ relative to a selected reference point on the body (e.g. pole $A$) and a reference line of the body (e.g. axis $AB$).

4. **Centrode Kinematic Equivalence Theorem**:  
   The planar motion of any rigid body is kinematically equivalent to the **pure rolling without slipping** of the Body Centrode upon the fixed Space Centrode.

---

#### Problem 4.2: Constrained Rod with Endpoints on Two Lines at Angle $\pi/3$
*(Appeared in: 2022/23 Q4a with $2m, 3a$; 2021/22 Q4a with $m, 2a$)*

**Problem Statement**:  
Consider a thin uniform rod $PQ$ of mass $M$ and length $L$. This rod is constrained such that its endpoints $P$ and $Q$ always lie on fixed straight lines $OA$ and $OB$ respectively, where the angle $\angle AOB = \pi/3$. At a particular instance:
1. The distances $OP = OQ = L$.
2. The endpoint $P$ is moving with a velocity $v$ along the line $OA$.  
Determine the kinetic energy of the rod at this instant.

**Step-by-Step Model Solution**:
1. **Geometric Configuration at the Given Instant**:  
   Since $OP = OQ = L$ and the length of the rod is $PQ = L$, $\triangle OPQ$ is an **equilateral triangle** with all sides equal to $L$ and all internal angles equal to $\pi/3$ ($60^\circ$).

2. **Determining the Velocities using ICR**:  
   - Line $OA$ is along the $x$-axis. The velocity of endpoint $P$ is directed along $OA$: $\mathbf{v}_P = (v, 0)$.
     The normal line to $\mathbf{v}_P$ at $P$ is the vertical line through $P(L, 0)$:
     $$x = L$$
   - Line $OB$ makes an angle of $\pi/3$ with $OA$. The endpoint $Q$ is constrained to slide along $OB$, so its velocity $\mathbf{v}_Q$ is directed along $OB$.
     $Q$ has coordinates $(L\cos(\pi/3), L\sin(\pi/3)) = \left(\frac{L}{2}, \frac{L\sqrt{3}}{2}\right)$.
     The normal line to $\mathbf{v}_Q$ at $Q$ is perpendicular to line $OB$ (inclined at $\frac{\pi}{3} + \frac{\pi}{2} = \frac{5\pi}{6}$, slope $-\frac{1}{\tan(\pi/3)} = -\frac{1}{\sqrt{3}}$):
     $$y - \frac{L\sqrt{3}}{2} = -\frac{1}{\sqrt{3}}\left(x - \frac{L}{2}\right)$$
     $$\sqrt{3}y - \frac{3}{2}L = -x + \frac{L}{2} \quad \implies \quad x + \sqrt{3}y = 2L$$
   - The Instantaneous Center of Rotation $I$ is the intersection of these two normals:
     Substitute $x = L$:
     $$L + \sqrt{3}y = 2L \quad \implies \quad \sqrt{3}y = L \quad \implies \quad y = \frac{L}{\sqrt{3}}$$
     $$I = \left(L, \frac{L}{\sqrt{3}}\right)$$

3. **Angular Velocity $\omega$ of the Rod**:  
   The distance from $P(L, 0)$ to $I(L, L/\sqrt{3})$ is:
   $$IP = \frac{L}{\sqrt{3}}$$
   Since $\mathbf{v}_P$ is perpendicular to $IP$:
   $$v_P = \omega \cdot (IP) \quad \implies \quad v = \omega \left(\frac{L}{\sqrt{3}}\right) \quad \implies \quad \omega = \frac{\sqrt{3}v}{L}$$

4. **Moment of Inertia about the ICR**:  
   The midpoint of the rod $PQ$ is the center of mass $G$:
   $$G = \frac{P + Q}{2} = \left(\frac{L + L/2}{2}, \frac{0 + L\sqrt{3}/2}{2}\right) = \left(\frac{3L}{4}, \frac{L\sqrt{3}}{4}\right)$$
   The distance squared from $I$ to $G$ is:
   $$IG^2 = \left(L - \frac{3L}{4}\right)^2 + \left(\frac{L}{\sqrt{3}} - \frac{L\sqrt{3}}{4}\right)^2 = \left(\frac{L}{4}\right)^2 + \left(\frac{4L - 3L}{4\sqrt{3}}\right)^2 = \frac{L^2}{16} + \frac{L^2}{48} = \frac{4L^2}{48} = \frac{L^2}{12}$$
   By the Parallel Axis Theorem, the moment of inertia of the rod about $I$ is:
   $$I_I = I_G + M(IG)^2 = \frac{1}{12}ML^2 + M\left(\frac{L^2}{12}\right) = \frac{1}{6}ML^2$$

5. **Total Kinetic Energy**:  
   $$T = \frac{1}{2}I_I \omega^2 = \frac{1}{2}\left(\frac{1}{6}ML^2\right)\left(\frac{\sqrt{3}v}{L}\right)^2 = \frac{1}{12}ML^2 \left(\frac{3v^2}{L^2}\right) = \frac{1}{4}Mv^2 \quad \blacksquare$$

*(Application to Exam Cases)*:
- **2022/2023 Exam Paper ($M = 2m, L = 3a$)**:
  $$T = \frac{1}{4}(2m)v^2 = \frac{1}{2}mv^2 \quad \blacksquare$$
- **2021/2022 Exam Paper ($M = m, L = 2a$)**:
  $$T = \frac{1}{4}mv^2 \quad \blacksquare$$

---

#### Problem 4.3: Rod Touching Parabola $y^2 = 4ax$ with End on $x$-axis
*(Appeared in: 2021/22 Q4b; Tutorial 2023/24 Tut 5 Q5, 2024/25 Problem Set 4 Q7)*

**Problem Statement**:  
A bar $AB$ moves in the $Oxy$-plane such that it always touches the parabola $y^2 = 4ax$, and the end $A$ moves along the $x$-axis.  
(i) Find the coordinates of the instantaneous center of rotation in terms of $\theta$, the angle between $AB$ and the $y$-axis.  
(ii) Prove that the equation of the Space Centrode is $ay^2 + 4x(a - x)^2 = 0$.  
(iii) Taking $A$ as the pole and $AB$ as the initial line, prove that the equation of the Body Centrode is $r = 2a\sin\theta\sec^3\theta$.

**Step-by-Step Model Solution**:
1. **Kinematic Construction of the ICR**:  
   - End $A(x_A, 0)$ moves along the $x$-axis $\implies \mathbf{v}_A$ is purely horizontal.
     The normal line to $\mathbf{v}_A$ at $A$ is the vertical line:
     $$x = x_A$$
   - The bar $AB$ touches the fixed parabola at point $P$. Because the bar remains tangent to the curve, the velocity of the contact point $P$ on the bar must be directed along the tangent line $AB$.
   - Hence, the normal line to $\mathbf{v}_P$ is the **normal line to the parabola at $P$**.
   - Therefore, the ICR $I(x, y)$ is the intersection of the vertical line through $A$ with the normal to the parabola at the point of contact $P$!

2. **Parametric Tangent & Normal to Parabola $y^2 = 4ax$**:  
   Let $\theta$ be the angle between the bar $AB$ and the $y$-axis.
   The slope of the bar $AB$ is:
   $$m = \cot\theta$$
   A tangent to $y^2 = 4ax$ with slope $m$ has the standard equation:
   $$y = mx + \frac{a}{m}$$
   The point of contact $P(x_P, y_P)$ is given by:
   $$x_P = \frac{a}{m^2}, \quad y_P = \frac{2a}{m}$$
   The intersection of the tangent with the $x$-axis ($y = 0$) gives the coordinate of end $A$:
   $$0 = mx_A + \frac{a}{m} \quad \implies \quad x_A = -\frac{a}{m^2}$$
   Since the normal through $A$ is vertical, the $x$-coordinate of the ICR is:
   $$x = x_A = -\frac{a}{m^2} = -a\tan^2\theta$$

3. **Finding the $y$-coordinate of the ICR (Part i)**:  
   The normal to the parabola at $P(x_P, y_P)$ has slope $-\frac{1}{m}$:
   $$y - y_P = -\frac{1}{m}(x - x_P) \quad \implies \quad y - \frac{2a}{m} = -\frac{1}{m}\left(x - \frac{a}{m^2}\right)$$
   Substitute $x = x_A = -\frac{a}{m^2}$ into the normal equation:
   $$y - \frac{2a}{m} = -\frac{1}{m}\left(-\frac{a}{m^2} - \frac{a}{m^2}\right) = -\frac{1}{m}\left(-\frac{2a}{m^2}\right) = \frac{2a}{m^3}$$
   $$y = \frac{2a}{m} + \frac{2a}{m^3} = \frac{2a}{m}\left(1 + \frac{1}{m^2}\right)$$
   Substitute $m = \cot\theta \implies \frac{1}{m} = \tan\theta$:
   $$y = 2a\tan\theta(1 + \tan^2\theta) = 2a\tan\theta\sec^2\theta = \frac{2a\sin\theta}{\cos^3\theta} = 2a\sin\theta\sec^3\theta$$
   Thus, the coordinates of the ICR are:
   $$\mathbf{I} = \left(-a\tan^2\theta, \; 2a\sin\theta\sec^3\theta\right) \quad \blacksquare$$

4. **Derivation of the Space Centrode (Part ii)**:  
   We eliminate the parameter $m$ between $x = -\frac{a}{m^2}$ and $y = \frac{2a}{m}\left(1 + \frac{1}{m^2}\right)$:
   From $x = -\frac{a}{m^2}$, we have:
   $$\frac{1}{m^2} = -\frac{x}{a}$$
   Substitute this into $1 + \frac{1}{m^2}$:
   $$1 + \frac{1}{m^2} = 1 - \frac{x}{a} = \frac{a - x}{a}$$
   Now square the expression for $y$:
   $$y^2 = \frac{4a^2}{m^2}\left(1 + \frac{1}{m^2}\right)^2$$
   Substitute $\frac{1}{m^2} = -\frac{x}{a}$ and $1 + \frac{1}{m^2} = \frac{a - x}{a}$:
   $$y^2 = 4a^2\left(-\frac{x}{a}\right)\left(\frac{a - x}{a}\right)^2 = -4x\frac{(a - x)^2}{a}$$
   Multiplying both sides by $a$:
   $$ay^2 = -4x(a - x)^2 \quad \implies \quad ay^2 + 4x(a - x)^2 = 0 \quad \blacksquare$$

5. **Derivation of the Body Centrode (Part iii)**:  
   Take end $A$ as the pole and the bar $AB$ as the initial line.
   Since the ICR $I$ lies vertically above $A$ at coordinates $(x_A, y)$, the line segment $AI$ is vertical.
   The distance $r = AI$ is:
   $$r = y = 2a\tan\theta\sec^2\theta = 2a\sin\theta\sec^3\theta \quad \blacksquare$$

---

#### Problem 4.4: Rod Touching Parabola $x = \frac{y^2}{8a}$ with End on $x$-axis
*(Appeared in: 2022/23 Q4b, 2018/19 Q4b; Tutorial 2024/25 Problem Set 4 Q1)*

**Problem Statement**:  
A rod $AB$ moves in the $xy$-plane such that it always touches the surface of the parabola $x = \frac{y^2}{8a}$ ($y \ge 0$), and the end $A$ moves along the $x$-axis. Let $\theta$ be the angle between the $y$-axis and $AB$.  
(i) Find the coordinates of the Instantaneous Center of Rotation in terms of $\theta$.  
(ii) Prove that the equation of the Space Centrode is:
$$2x^3 - 8ax^2 + 8a^2x + ay^2 = 0$$
(iii) Referred to $A$ as the pole and $AB$ as the initial line, prove that the equation of the Body Centrode is $r = 4a\sin\theta\sec^3\theta$.

**Step-by-Step Model Solution**:
1. **Mapping to Standard Form**:  
   Rewrite the parabola as $y^2 = 8ax = 4(2a)x$.
   This is the identical form to Problem 4.3 with parameter $a' = 2a$!
   Using the results of Problem 4.3 with $a' = 2a$:
   $$x_I = -a'\tan^2\theta = -2a\tan^2\theta$$
   $$y_I = 2a'\sin\theta\sec^3\theta = 4a\sin\theta\sec^3\theta$$
   Coordinates of ICR:
   $$\mathbf{I} = \left(-2a\tan^2\theta, \; 4a\sin\theta\sec^3\theta\right) \quad \blacksquare$$

2. **Space Centrode Equation (Part ii)**:  
   From the space centrode of $y^2 = 4a'x$:
   $$a'y^2 + 4x(a' - x)^2 = 0$$
   Substitute $a' = 2a$:
   $$2ay^2 + 4x(2a - x)^2 = 0$$
   Divide by 2:
   $$ay^2 + 2x(4a^2 - 4ax + x^2) = 0$$
   $$ay^2 + 8a^2x - 8ax^2 + 2x^3 = 0$$
   Rearranging in descending powers of $x$:
   $$2x^3 - 8ax^2 + 8a^2x + ay^2 = 0 \quad \blacksquare$$

3. **Body Centrode (Part iii)**:  
   With $A$ as pole and $AB$ as initial line:
   $$r = AI = y_I = 4a\sin\theta\sec^3\theta \quad \blacksquare$$

---

#### Problem 4.5: Rod Touching Parabola $y = -x^2 + \frac{1}{4}$
*(Appeared in: 2023/24 Q4b, 2020/21 Q4b; Tutorial 2023/24 Tut 5 Q6, 2024/25 Problem Set 4 Q5)*

**Problem Statement**:  
A bar $AB$ of length 2 meters moves in the $xy$-plane such that it always touches the parabola $y = -x^2 + \frac{1}{4}$, and the end $A$ moves along the $x$-axis.  
(i) Find the coordinates of the instantaneous center in terms of $\theta$, the angle between $AB$ and the $y$-axis.  
(ii) Prove that the equation of the Space Centrode is $y^2 = 4x^2(4x^2 - 1)$.  
(iii) Taking $A$ as the pole and $AB$ as the initial line, prove that the equation of the Body Centrode is $r = \frac{1}{4}(\tan^2\theta - \cot^2\theta)$.  
(iv) At the instant $\theta = \pi/3$, find the kinetic energy of the bar (mass $M$).

**Step-by-Step Model Solution**:
1. **Point of Contact & Coordinates of $A$**:  
   Let the contact point on the parabola be $P(x_0, y_0) = (x_0, -x_0^2 + 1/4)$.
   The slope of the tangent at $P$ is $\frac{dy}{dx} = -2x_0$.
   Since $\theta$ is the angle between $AB$ and the $y$-axis, the slope of $AB$ is $m = \cot\theta$:
   $$-2x_0 = \cot\theta \quad \implies \quad x_0 = -\frac{1}{2}\cot\theta$$
   The $y$-coordinate of contact point $P$ is:
   $$y_0 = -x_0^2 + \frac{1}{4} = -\frac{1}{4}\cot^2\theta + \frac{1}{4} = \frac{1}{4}(1 - \cot^2\theta)$$
   The equation of the tangent line $AB$ is:
   $$y - y_0 = m(x - x_0) \quad \implies \quad y - \frac{1}{4}(1 - \cot^2\theta) = \cot\theta\left(x + \frac{1}{2}\cot\theta\right)$$
   $$y = x\cot\theta + \frac{1}{2}\cot^2\theta + \frac{1}{4} - \frac{1}{4}\cot^2\theta = x\cot\theta + \frac{1}{4}(1 + \cot^2\theta) = x\cot\theta + \frac{1}{4}\csc^2\theta$$
   End $A$ is the intersection with the $x$-axis ($y = 0$):
   $$0 = x_A \cot\theta + \frac{1}{4}\csc^2\theta \quad \implies \quad x_A = -\frac{\csc^2\theta}{4\cot\theta} = -\frac{1}{4\sin\theta\cos\theta} = -\frac{1}{2\sin(2\theta)}$$

2. **Coordinates of ICR $I$ (Part i)**:  
   Since $A$ moves along the $x$-axis, the normal to $\mathbf{v}_A$ is the vertical line through $A$:
   $$x_I = x_A = -\frac{1}{2\sin(2\theta)} = -\frac{1}{4}\csc\theta\sec\theta$$
   The normal to the parabola at $P(x_0, y_0)$ has slope $-\frac{1}{m} = -\tan\theta$:
   $$y - y_0 = -\tan\theta(x - x_0)$$
   At the ICR, $x = x_A$:
   $$y_I = y_0 - \tan\theta(x_A - x_0)$$
   Substitute $x_0 = -\frac{1}{2}\cot\theta$, $y_0 = \frac{1}{4}(1 - \cot^2\theta)$, and $x_A = -\frac{1}{4}\cot\theta - \frac{1}{4}\tan\theta$:
   $$x_A - x_0 = \left(-\frac{1}{4}\cot\theta - \frac{1}{4}\tan\theta\right) - \left(-\frac{1}{2}\cot\theta\right) = \frac{1}{4}\cot\theta - \frac{1}{4}\tan\theta$$
   $$y_I = \frac{1}{4}(1 - \cot^2\theta) - \tan\theta\left(\frac{1}{4}\cot\theta - \frac{1}{4}\tan\theta\right) = \frac{1}{4} - \frac{1}{4}\cot^2\theta - \frac{1}{4} + \frac{1}{4}\tan^2\theta = \frac{1}{4}(\tan^2\theta - \cot^2\theta)$$
   Thus, the coordinates of the ICR are:
   $$\mathbf{I} = \left(-\frac{1}{2\sin(2\theta)}, \; \frac{1}{4}(\tan^2\theta - \cot^2\theta)\right) \quad \blacksquare$$

3. **Space Centrode Equation (Part ii)**:  
   We have:
   $$x = -\frac{1}{2\sin(2\theta)} \quad \implies \quad \sin(2\theta) = -\frac{1}{2x} \quad \implies \quad \sin^2(2\theta) = \frac{1}{4x^2}$$
   Recall:
   $$\tan^2\theta - \cot^2\theta = (\tan\theta - \cot\theta)(\tan\theta + \cot\theta)$$
   $$\tan\theta - \cot\theta = \frac{\sin^2\theta - \cos^2\theta}{\sin\theta\cos\theta} = \frac{-\cos(2\theta)}{\frac{1}{2}\sin(2\theta)} = -2\cot(2\theta)$$
   $$\tan\theta + \cot\theta = \frac{\sin^2\theta + \cos^2\theta}{\sin\theta\cos\theta} = \frac{1}{\frac{1}{2}\sin(2\theta)} = \frac{2}{\sin(2\theta)}$$
   Therefore:
   $$y = \frac{1}{4}\left(-2\cot(2\theta)\right)\left(\frac{2}{\sin(2\theta)}\right) = -\frac{\cot(2\theta)}{\sin(2\theta)} = -\frac{\cos(2\theta)}{\sin^2(2\theta)}$$
   Squaring $y$:
   $$y^2 = \frac{\cos^2(2\theta)}{\sin^4(2\theta)} = \frac{1 - \sin^2(2\theta)}{\sin^4(2\theta)} = \left(\frac{1}{\sin^2(2\theta)} - 1\right)\frac{1}{\sin^2(2\theta)}$$
   Substitute $\frac{1}{\sin^2(2\theta)} = 4x^2$:
   $$y^2 = (4x^2 - 1)(4x^2) = 4x^2(4x^2 - 1) \quad \blacksquare$$

4. **Body Centrode (Part iii)**:  
   Referred to $A$ as pole and $AB$ as initial line:
   $$r = AI = y_I = \frac{1}{4}(\tan^2\theta - \cot^2\theta) \quad \blacksquare$$

5. **Kinetic Energy at $\theta = \pi/3$ (Part iv)**:  
   At $\theta = \pi/3$:
   $$\tan(\pi/3) = \sqrt{3} \implies \tan^2 = 3$$
   $$\cot(\pi/3) = \frac{1}{\sqrt{3}} \implies \cot^2 = \frac{1}{3}$$
   $$r = \frac{1}{4}\left(3 - \frac{1}{3}\right) = \frac{1}{4}\left(\frac{8}{3}\right) = \frac{2}{3}\text{ m}$$
   The bar has length $L = 2\text{ m}$, so its midpoint $G$ is at distance $1\text{ m}$ from $A$ along the rod.
   Relative to $A$, $G$ is at $(1\sin\theta, 1\cos\theta) = \left(\frac{\sqrt{3}}{2}, \frac{1}{2}\right)$.
   The ICR $I$ is at $(0, r) = \left(0, \frac{2}{3}\right)$ relative to $A$.
   The distance $IG$ from ICR to center of mass $G$ is:
   $$IG^2 = \left(\frac{\sqrt{3}}{2} - 0\right)^2 + \left(\frac{1}{2} - \frac{2}{3}\right)^2 = \frac{3}{4} + \left(-\frac{1}{6}\right)^2 = \frac{3}{4} + \frac{1}{36} = \frac{28}{36} = \frac{7}{9}$$
   The moment of inertia of the bar about $G$ is $I_G = \frac{1}{12}M(2)^2 = \frac{1}{3}M$.
   By the Parallel Axis Theorem about $I$:
   $$I_I = I_G + M(IG)^2 = \frac{1}{3}M + \frac{7}{9}M = \frac{10}{9}M$$
   The total kinetic energy is:
   $$T = \frac{1}{2}I_I \dot{\theta}^2 = \frac{1}{2}\left(\frac{10}{9}M\right)\dot{\theta}^2 = \frac{5}{9}M\dot{\theta}^2 \quad \blacksquare$$
   *(Or in terms of $v_A = r\dot{\theta} = \frac{2}{3}\dot{\theta} \implies T = \frac{5}{4}M v_A^2$)*.

---

#### Problem 4.6: Rod Touching Circle $x^2 + y^2 = 1$
*(Appeared in: 2019/20 Q4b; Tutorial 2023/24 Tut 5 Q4, 2024/25 Problem Set 4 Q2/Q4)*

**Problem Statement**:  
A rod $AB$ moves in the $Oxy$-plane such that it always touches the circle $x^2 + y^2 = 1$, and the end $A$ moves along the $x$-axis.  
(i) Find the coordinates of the instantaneous center in terms of $\theta$, the angle between $AB$ and the $y$-axis.  
(ii) Prove that the equation of the Space Centrode is $y^2 + x^2(1 - x^2) = 0$.  
(iii) Taking $A$ as the pole and $AB$ as the initial line, prove that the equation of the Body Centrode is $r = \sin\theta\sec^2\theta$.

**Step-by-Step Model Solution**:
1. **Geometry & Contact Point**:  
   Let the rod touch the unit circle at $P$.
   The normal to the circle at $P$ passes through the center of the circle, which is the origin $O(0, 0)$.
   Since the rod $AB$ makes an angle $\theta$ with the $y$-axis, the normal line $OP$ makes an angle $\theta$ with the $x$-axis.
   Coordinates of contact point $P$:
   $$x_P = \sin\theta, \quad y_P = \cos\theta$$
   The tangent line $AB$ at $P$ has equation:
   $$x\sin\theta + y\cos\theta = 1$$
   Setting $y = 0$ gives the coordinate of end $A$ on the $x$-axis:
   $$x_A \sin\theta = 1 \quad \implies \quad x_A = \frac{1}{\sin\theta} = \csc\theta \quad (\text{or } -\sec\theta \text{ depending on quadrant})$$
   Taking the standard quadrant from exam figure (where $A$ lies on negative $x$-axis):
   $$x_A = -\sec\theta$$

2. **Coordinates of ICR $I$ (Part i)**:  
   - Normal to $\mathbf{v}_A$ is vertical: $x_I = x_A = -\sec\theta$.
   - Normal to $\mathbf{v}_P$ passes through origin $O(0, 0)$ with slope $\tan\theta$:
     $$y = -\tan\theta \cdot x$$
   - Substituting $x = -\sec\theta$:
     $$y_I = -\tan\theta(-\sec\theta) = \tan\theta\sec\theta = \sin\theta\sec^2\theta$$
   Thus, the ICR is:
   $$\mathbf{I} = \left(-\sec\theta, \; \sin\theta\sec^2\theta\right) \quad \blacksquare$$

3. **Space Centrode (Part ii)**:  
   Eliminating $\theta$:
   $$x^2 = \sec^2\theta = 1 + \tan^2\theta \quad \implies \quad \tan^2\theta = x^2 - 1$$
   $$y^2 = \tan^2\theta\sec^2\theta = (x^2 - 1)x^2 = x^4 - x^2$$
   $$y^2 - x^2(x^2 - 1) = 0 \quad \implies \quad y^2 + x^2(1 - x^2) = 0 \quad \blacksquare$$

4. **Body Centrode (Part iii)**:  
   Taking $A$ as pole and $AB$ as initial line:
   $$r = AI = y_I = \sin\theta\sec^2\theta \quad \blacksquare$$

---

## Section IV: Common Pitfalls & Exam Traps

### 1. The Normal Acceleration Direction Trap ($\mathbf{N}$ vs Gravity vs Reaction)
- **The Pitfall**: Students frequently write $m\frac{v^2}{\rho} = R - mg\cos\psi$ without checking which way the principal normal points.
- **The Rule**: The unit principal normal $\mathbf{N} = \frac{d\mathbf{T}}{d\psi}$ **always points towards the center of curvature** (the concave side of the curve).
  - For a bead *inside* a bowl or concave curve (e.g., parabola $x^2 = 4ay$), the center of curvature is upwards $\implies$ normal acceleration is upwards $\implies m\frac{v^2}{\rho} = R - mg\cos\psi$.
  - For a skier *on top of* a hill (e.g., catenary $y = c[\cosh(x/c)-1]$ or inverted cycloid $s = 4a\sin\psi$), the center of curvature is downwards $\implies$ normal acceleration is downwards $\implies m\frac{v^2}{\rho} = mg\cos\psi - R$.
- **Exam Warning**: Flipping this sign will yield an incorrect lift-off condition or a reaction force that grows rather than decays to zero!

### 2. The "Smooth Table" Falling Rod Trap ($\dot{x}_A \ne 0$)
- **The Pitfall**: Treating the contact point $A$ on a smooth horizontal table as an instantaneous pivot with zero velocity ($\mathbf{v}_A = \mathbf{0}$).
- **The Reality**: Because the table is smooth, there is no horizontal friction force! Therefore:
  $$\sum F_x = 0 \quad \implies \quad \dot{x}_G = 0 \quad (x_G = \text{constant})$$
  Because the center of mass moves in a strictly vertical line, point $A$ must accelerate horizontally:
  $$x_A = x_G - d\sin\theta \quad \implies \quad \dot{x}_A = -d\dot{\theta}\cos\theta \ne 0$$
  You **must** use König's theorem ($T = \frac{1}{2}M v_G^2 + T_{rel}$) or carefully account for $\dot{x}_A^2$. Treating $A$ as stationary will lose 50%+ of the marks on Question 2!

### 3. Misapplying König's Theorem (Centroid vs Arbitrary Point)
- **The Pitfall**: Trying to decompose kinetic energy using an arbitrary point $P$ instead of the center of mass $G$:
  $$T \ne \frac{1}{2}M v_P^2 + \frac{1}{2}\sum m_i (\mathbf{v}'_{P, i})^2 \quad (\text{FALSE if } P \ne G)$$
- **The Crucial Step in Proofs**: In Question 2(a), you **must explicitly show** why the cross-term vanishes:
  $$\mathbf{v}_G \cdot \left(\sum m_i \mathbf{v}'_i\right) = \mathbf{v}_G \cdot \mathbf{0} = 0$$
  If you do not state $\sum m_i \mathbf{r}'_i = \mathbf{0} \implies \sum m_i \mathbf{v}'_i = \mathbf{0}$, markers dock 5–10 points immediately.

### 4. Impulse & Momentum Conservation in Moving Mass / Insect Problems
- **The Pitfall**: For an insect crawling along the rim of a vertical disc or boy walking on a board, writing $I\Omega = m v a$.
- **The Reality**: The speed $v$ is given **relative to the disc/board**.
  The absolute velocity of the insect in space is $v_{space} = a\Omega + v$.
  Therefore, the conservation of angular momentum at the kick gives:
  $$I_{disc}\Omega + m_{insect} a(a\Omega + v) = 0 \quad \implies \quad \left(I_{disc} + m_{insect} a^2\right)\Omega + m_{insect} a v = 0$$
  Omitting the $a\Omega$ term inside the bracket will yield incorrect denominators (e.g. $v/5a$ instead of $v/6a$).

### 5. Space Centrode vs. Body Centrode Representation
- **The Pitfall**: Expressing the Body Centrode in fixed coordinates $(x, y)$ or the Space Centrode in polar $(r, \theta)$.
- **The Rule**:
  - **Space Centrode (SC)**: MUST be an equation in fixed Cartesian coordinates $x$ and $y$ with all parameters ($\theta, m$) eliminated: $F(x, y) = 0$.
  - **Body Centrode (BC)**: MUST be expressed in body-fixed coordinates, typically polar $(r, \theta)$ where $r = AI$ is the distance from a specified body point $A$ to the ICR, and the initial line is along the body (e.g. along $AB$).

### 6. Documented Historical Exam Typos (DO NOT GET TRIPPED!)
- **Exam 2020/2021 Question 3(a) [Solid Hemisphere]**:
  - Printed on paper: $\dot{\theta} = \frac{15g\cos\theta}{a(28-15\cos\theta)}$
  - **Mathematical Fact**: The left-hand side is $\dot{\theta}^2$. Angular velocity squared has units $[1/\text{s}^2]$, matching $g/a$. If this appears, state: *"From energy conservation, $\dot{\theta}^2 = \frac{15g\cos\theta}{a(28-15\cos\theta)}$"*.
- **Exam 2020/2021 Question 4(b)(ii) [Parabola $y = -x^2 + 1/4$]**:
  - Printed on paper: $y^2 = 4x^2(4x^2 + 1)$
  - **Mathematical Fact**: The correct identity is $y^2 = 4x^2(4x^2 - 1)$ (since $\cos^2(2\theta) = 1 - \sin^2(2\theta) \implies \frac{1}{\sin^2(2\theta)} - 1 = 4x^2 - 1$). This was quietly corrected in the 2023/2024 examination paper.

---

## Section V: Quick-Revision Active-Recall Checklist

Use this 25-point checklist 24–48 hours before the exam. Check each item only if you can perform the derivation or state the result from memory on blank paper:

### Module 1: Particles on Curves & Kinematics
- [ ] 1. Derive $\mathbf{a} = \ddot{s}\mathbf{T} + \frac{\dot{s}^2}{\rho}\mathbf{N}$ from $\mathbf{r}(s(t))$, proving $\mathbf{N} = \frac{d\mathbf{T}}{d\psi}$ and $\frac{d\mathbf{T}}{dt} = \frac{\dot{s}}{\rho}\mathbf{N}$.
- [ ] 2. For an inverted cycloid $s = 4a\sin\psi$, set up the tangential equation of motion to prove $\ddot{s} - \frac{g}{4a}s = 0$.
- [ ] 3. For the cycloid, calculate the normal reaction $R = \frac{mg}{2}(4\cos\psi - 3\sec\psi)$ when $v_0 = \sqrt{2ga}$.
- [ ] 4. For the catenary hill $y = c[\cosh(x/c)-1]$, derive $s = c\tan\psi$, $y = c(\sec\psi - 1)$, and the lift-off depth $y = c - u^2/g$.
- [ ] 5. For the parabola $x^2 = 4ay$, prove $\rho = 2a\sec^3\psi$ and deduce that normal reaction $R \propto \cos^3\psi$.
- [ ] 6. For a bead on a vertical cardioid $r = a(1+\cos\theta)$ with elastic string ($\lambda = 4mg$), prove $\theta = \pi/3$ is an equilibrium.
- [ ] 7. For two particles connected via a hole in a table, formulate energy and angular momentum to prove $Q$ reaches the hole when projected at $\sqrt{8gl/3}$.
- [ ] 8. For a circular helix $\mathbf{r}(\theta) = a\cos\theta\mathbf{i} + a\sin\theta\mathbf{j} + b\theta\mathbf{k}$, calculate speed $v$ and unit tangent $\mathbf{T}$.

### Module 2: Systems of Particles & Constraints
- [ ] 9. State and prove König's Theorem for Kinetic Energy: $T = \frac{1}{2}M v_G^2 + \frac{1}{2}\sum m_i (v'_i)^2$.
- [ ] 10. State and prove the Angular Momentum decomposition theorem: $\mathbf{H}_O = \mathbf{r}_G \times M\mathbf{v}_G + \mathbf{H}_G$.
- [ ] 11. Explain why the center of mass of a rod falling on a smooth table moves in a vertical straight line ($\sum F_x = 0$).
- [ ] 12. For a falling rod of length $a$ with masses $3m$ and $m$, derive $\dot{\theta}^2 = \frac{8g(1-\cos\theta)}{a(3+\sin^2\theta)}$.
- [ ] 13. For a falling rod of length $2a$ with equal masses $m, m$, derive $\dot{\theta}^2 = \frac{2g(1-\cos\theta)}{a(1+\sin^2\theta)}$ and the thrust on the table.
- [ ] 14. For a ring of mass $2m$ on a wire with hanging mass $m$, derive $l\dot{\theta}^2 = \frac{6g\sin\theta}{2+\cos^2\theta}$ and tension $T$.

### Module 3: Planar Rigid Body Dynamics
- [ ] 15. State the Parallel Axis (Steiner's) and Perpendicular Axis Theorems with exact validity conditions.
- [ ] 16. Calculate the moment of inertia of a compound rod ($2M, 4a$ plus $M, 2a$) about the end pivot ($I_A = 20Ma^2$).
- [ ] 17. Find the initial angular acceleration of the compound rod released from horizontal: $\ddot{\theta}_0 = \frac{7g}{20a}$.
- [ ] 18. For a disc pivoted at the rim, derive horizontal reaction $X = mg\sin(2\theta)$ and vertical reaction $Y = \frac{mg}{3}(4 - 3\cos(2\theta))$.
- [ ] 19. For a solid hemisphere rocking without slipping, recall $OG = \frac{3}{8}a$, find $I_P$, and prove $\dot{\theta}^2 = \frac{15g\cos\theta}{a(28-15\cos\theta)}$.
- [ ] 20. For a disc with a particle in a radial groove, use angular momentum conservation to find $\dot{\theta}(r)$ and energy conservation to find $\dot{r}(r)$.
- [ ] 21. For an insect of mass $m/k$ on a vertical disc, derive initial spin $\Omega = \frac{2v}{(k+2)a}$ and equation of motion.
- [ ] 22. For a boy walking around a free circular board, integrate $H_z = 0$ to prove the board turns through $\frac{4m\pi}{M+2m}$.

### Module 4: Planar Kinematics & Centrodes
- [ ] 23. State the exact definition of Instantaneous Center of Rotation, Space Centrode, and Body Centrode.
- [ ] 24. For a rod with ends on lines meeting at $\pi/3$, locate the ICR and prove $T = \frac{1}{4}Mv^2$ when $OP = OQ = L$.
- [ ] 25. For a rod touching a curve with end on the $x$-axis:
  - Parabola $y^2 = 4ax \implies$ Space Centrode: $ay^2 + 4x(a-x)^2 = 0$; Body Centrode: $r = 2a\sin\theta\sec^3\theta$.
  - Parabola $x = y^2/(8a) \implies$ Space Centrode: $2x^3 - 8ax^2 + 8a^2x + ay^2 = 0$; Body Centrode: $r = 4a\sin\theta\sec^3\theta$.
  - Parabola $y = -x^2 + 1/4 \implies$ Space Centrode: $y^2 = 4x^2(4x^2-1)$; Body Centrode: $r = \frac{1}{4}(\tan^2\theta - \cot^2\theta)$.
  - Circle $x^2 + y^2 = 1 \implies$ Space Centrode: $y^2 + x^2(1-x^2) = 0$; Body Centrode: $r = \sin\theta\sec^2\theta$.

---
*End of Final Exam Master Study Pack — MAT 1053 / MT 1053 / MT 106 Classical Mechanics I*
