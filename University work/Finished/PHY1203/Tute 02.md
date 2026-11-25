###   
Modern Physics Tute 02 Submission

by [Dr P W S K Bandaranayake](https://scilms.pdn.ac.lk/user/view.php?id=604&course=1524) - Monday, 31 August 2026, 11:34 AM

Number of replies: 0

Dear students,

Please submit PHY1203-Modern Physics: Tute 02, on or before 11th September 2026.

Questions are: (6), (11), (12) and (13).

Lecturer in-charge


![[Pasted image 20260911072236.png]]

---

## Solutions

### Constants Used
* Planck's constant: $h = 6.626 \times 10^{-34} \text{ J}\cdot\text{s}$ (or $4.136 \times 10^{-15} \text{ eV}\cdot\text{s}$)
* Speed of light: $c = 3.00 \times 10^8 \text{ m/s}$
* Elementary charge: $e = 1.602 \times 10^{-19} \text{ C}$
* Rest mass of electron: $m_e = 9.109 \times 10^{-31} \text{ kg}$
* Compton wavelength of electron: $\lambda_c = \frac{h}{m_e c} \approx 2.426 \times 10^{-12} \text{ m} = 2.426 \text{ pm}$

---

### Question (06)

**Problem:**
Light with wavelength $600\text{ nm}$ falls on a metal surface and photoelectrons with the maximum kinetic energy of $0.17\text{ eV}$ are emitted.
(i) Determine the work function and
(ii) Find the threshold frequency for the metal.
(iii) What is the stopping potential (in V) when the surface is illuminated with light of wavelength $400\text{ nm}$?

**Solution:**

Einstein's photoelectric equation:
$$K_{\max} = E - \Phi = \frac{hc}{\lambda} - \Phi$$

#### (i) Work Function ($\Phi$)
For $\lambda_1 = 600\text{ nm} = 600 \times 10^{-9}\text{ m}$:
$$E_1 = \frac{hc}{\lambda_1} = \frac{(6.626 \times 10^{-34} \text{ J}\cdot\text{s})(3.00 \times 10^8 \text{ m/s})}{600 \times 10^{-9} \text{ m}} = 3.313 \times 10^{-19} \text{ J}$$

Converting to electron-volts ($\text{eV}$):
$$E_1 = \frac{3.313 \times 10^{-19} \text{ J}}{1.602 \times 10^{-19} \text{ J/eV}} \approx 2.068 \text{ eV}$$

Now finding $\Phi$:
$$\Phi = E_1 - K_{\max} = 2.068 \text{ eV} - 0.17 \text{ eV} = \mathbf{1.90 \text{ eV}} \quad (\approx 3.04 \times 10^{-19} \text{ J})$$

#### (ii) Threshold Frequency ($f_0$)
$$\Phi = h f_0 \implies f_0 = \frac{\Phi}{h}$$
$$f_0 = \frac{3.044 \times 10^{-19} \text{ J}}{6.626 \times 10^{-34} \text{ J}\cdot\text{s}} \approx \mathbf{4.59 \times 10^{14} \text{ Hz}}$$

#### (iii) Stopping Potential for $\lambda_2 = 400\text{ nm}$
For $\lambda_2 = 400 \times 10^{-9}\text{ m}$:
$$E_2 = \frac{hc}{\lambda_2} = \frac{(6.626 \times 10^{-34} \text{ J}\cdot\text{s})(3.00 \times 10^8 \text{ m/s})}{(400 \times 10^{-9} \text{ m})(1.602 \times 10^{-19} \text{ J/eV})} \approx 3.102 \text{ eV}$$

Maximum kinetic energy:
$$K_{\max, 2} = E_2 - \Phi = 3.102 \text{ eV} - 1.898 \text{ eV} = 1.204 \text{ eV}$$

Since $e V_s = K_{\max}$:
$$V_s = \mathbf{1.20 \text{ V}}$$

---

### Question (11)

**Problem:**
A clean magnesium surface is supported in a vacuum as the cathode of a photocell. A wire-mesh electrode surrounds the cathode and is used as the anode. When the cathode is illuminated with ultraviolet radiation of wavelength $254\text{ nm}$ the anode current can be reduced to zero by making it negative with respect to the cathode using a PD of $1.2\text{ V}$ or greater. Obtain a value for the work function of magnesium in eV.

**Solution:**

* Given:
  * Wavelength $\lambda = 254\text{ nm} = 254 \times 10^{-9}\text{ m}$
  * Stopping potential $V_s = 1.2\text{ V} \implies K_{\max} = e V_s = 1.2\text{ eV}$

1. Energy of incident photon:
   $$E = \frac{hc}{\lambda} = \frac{(6.626 \times 10^{-34} \text{ J}\cdot\text{s})(3.00 \times 10^8 \text{ m/s})}{254 \times 10^{-9} \text{ m}} = 7.826 \times 10^{-19} \text{ J}$$
   $$E = \frac{7.826 \times 10^{-19} \text{ J}}{1.602 \times 10^{-19} \text{ J/eV}} \approx 4.885 \text{ eV}$$

2. Work function $\Phi$:
   $$e V_s = E - \Phi \implies \Phi = E - e V_s$$
   $$\Phi = 4.885 \text{ eV} - 1.20 \text{ eV} = \mathbf{3.69 \text{ eV}}$$

---

### Question (12)

**Problem:**
(a) What is Compton Effect?
(b) Write down the formula for the Compton shift identifying all the symbols and stating all the assumptions made.
(c) Explain why there is no wavelength shift in some of the scattered photons.
(d) X-rays of wavelength $0.2\text{ nm}$ are scattered from a block of material. The scattered X-rays are observed at an angle of $45.0^\circ$ to the incident beam.
  (i) Calculate the wavelength of the scattered X-rays at this angle.
  (ii) Compute the fractional change in the energy of a photon in this scattering.

**Solution:**

#### (a) Definition
The **Compton Effect** is the increase in wavelength (decrease in frequency and photon energy) observed when high-frequency electromagnetic radiation (such as X-rays or $\gamma$-rays) is scattered by electrons in matter. It demonstrates the particle nature of light.

#### (b) Formula, Symbols, and Assumptions
$$\Delta \lambda = \lambda' - \lambda = \frac{h}{m_e c} (1 - \cos\theta)$$

* **Symbols:**
  * $\lambda$: Wavelength of incident photon
  * $\lambda'$: Wavelength of scattered photon
  * $\Delta \lambda$: Compton wavelength shift
  * $h$: Planck's constant ($6.626 \times 10^{-34} \text{ J}\cdot\text{s}$)
  * $m_e$: Rest mass of the electron ($9.109 \times 10^{-31} \text{ kg}$)
  * $c$: Speed of light in vacuum ($3.00 \times 10^8 \text{ m/s}$)
  * $\lambda_c = \frac{h}{m_e c} \approx 2.426 \times 10^{-12} \text{ m}$: Compton wavelength of electron
  * $\theta$: Photon scattering angle relative to initial incident direction

* **Assumptions:**
  1. Radiation behaves as corpuscular photons with energy $E = h\nu$ and momentum $p = \frac{h}{\lambda} = \frac{E}{c}$.
  2. The target electron is loosely bound (nearly free) and initially stationary ($E_{\text{binding}} \ll E_{\text{photon}}$).
  3. The photon-electron interaction is an elastic collision where relativistic energy and momentum are conserved.

#### (c) Why there is no shift in some photons
Some incident photons collide with tightly bound inner-shell electrons. In this case, the electron cannot be ejected alone, and the photon scatters elastically off the **entire atom** as a single unit. In the Compton formula:
$$\Delta \lambda = \frac{h}{M_{\text{atom}} c}(1 - \cos\theta)$$
Since $M_{\text{atom}} \approx 10^4 - 10^5 \times m_e$, the shift $\Delta \lambda \approx 0$. These photons emerge with essentially no change in wavelength (known as the unmodified line or Thomson scattering).

#### (d) Calculations for $\lambda = 0.2\text{ nm}$ and $\theta = 45.0^\circ$

**(i) Scattered wavelength ($\lambda'$):**
$$\Delta \lambda = \lambda_c (1 - \cos 45.0^\circ) = (2.426 \times 10^{-12} \text{ m})(1 - 0.7071) \approx 7.10 \times 10^{-13} \text{ m} = 0.000710 \text{ nm}$$
$$\lambda' = \lambda + \Delta \lambda = 0.2 \text{ nm} + 0.000710 \text{ nm} = \mathbf{0.20071 \text{ nm}} \quad (= 2.0071 \times 10^{-10} \text{ m})$$

**(ii) Fractional change in photon energy:**
$$\frac{|\Delta E|}{E} = \frac{E - E'}{E} = \frac{\frac{hc}{\lambda} - \frac{hc}{\lambda'}}{\frac{hc}{\lambda}} = \frac{\lambda' - \lambda}{\lambda'} = \frac{\Delta \lambda}{\lambda'}$$
$$\frac{|\Delta E|}{E} = \frac{0.000710 \text{ nm}}{0.200710 \text{ nm}} \approx \mathbf{3.54 \times 10^{-3}} \quad (\text{or } \mathbf{0.354\%})$$

---

### Question (13)

**Problem:**
X-rays with wavelength $7.0 \times 10^{-11}\text{ m}$ is incident on a calcite target.
(i) Find the wavelength of the X-ray scattered at an angle of $30^\circ$.
(ii) What is the largest shift that can be expected in this experiment?

**Solution:**

#### (i) Wavelength at $\theta = 30^\circ$
$$\Delta \lambda = \lambda_c (1 - \cos 30^\circ) = (2.426 \times 10^{-12} \text{ m})\left(1 - \frac{\sqrt{3}}{2}\right)$$
$$\Delta \lambda = 2.426 \times 10^{-12} \times (1 - 0.8660) \approx 3.25 \times 10^{-13} \text{ m} = 0.0325 \times 10^{-11} \text{ m}$$

$$\lambda' = \lambda + \Delta \lambda = 7.0 \times 10^{-11} \text{ m} + 0.0325 \times 10^{-11} \text{ m} = \mathbf{7.0325 \times 10^{-11} \text{ m}} \quad (\approx 7.03 \times 10^{-11} \text{ m})$$

#### (ii) Largest Shift Expected
The Compton shift $\Delta \lambda = \lambda_c (1 - \cos\theta)$ is maximized when $\cos\theta = -1$ (i.e. $\theta = 180^\circ$, direct backscattering):
$$\Delta \lambda_{\max} = 2\lambda_c = 2 \times 2.426 \times 10^{-12} \text{ m} = \mathbf{4.85 \times 10^{-12} \text{ m}} \quad (= 4.85 \text{ pm})$$