<!---
{
  "id": "077e7849-3a02-4e7d-bdc9-c7ad443784fd",
  "depends_on": [],
  "author": "Stephan Bökelmann",
  "first_used": "2025-04-11",
  "keywords": ["quantum mechanics", "de-Broglie wavelength", "ionization energy", "relativistic physics", "wave-particle duality"]
}
-->

# de Broglie Wavelength and Ionizing Radiation

> In this exercise you will learn how to compute key properties of electromagnetic radiation that is capable of ionizing a hydrogen atom. Furthermore we will explore how the de Broglie wavelength of particles depends on their kinetic energy, in classical, relativistic, and ultrarelativistic regimes.

### Introduction

In quantum mechanics, the concept of wave-particle duality is a cornerstone principle that extends across both electromagnetic waves and material particles. Photons, which constitute electromagnetic radiation, exhibit both wave-like and particle-like properties. This duality allows us to associate a frequency, wavelength, and wavenumber to photons with a given energy. For example, the ionization energy of a hydrogen atom defines the minimum photon energy required to remove an electron from its ground state.

The de Broglie hypothesis further extends wave-particle duality to massive particles. According to de Broglie, every particle with momentum \( p \) can be associated with a wavelength \( \lambda = h/p \), where \( h \) is Planck’s constant. Depending on the kinetic energy of the particle and its mass, we must use different models to calculate its momentum: classical mechanics when the particle's speed is much less than the speed of light, and relativistic or ultrarelativistic models when velocities approach or exceed relativistic thresholds.

This exercise guides you through calculating ionizing radiation properties and deriving the de Broglie wavelength for a variety of physical systems — from electrons to Higgs bosons, and even dust particles — each illustrating a different physical regime.

### Further Readings and Other Sources

- [HyperPhysics: de Broglie Wavelength](http://hyperphysics.phy-astr.gsu.edu/hbase/quantum/debrog.html)
- [DOI:10.1016/j.physletb.2012.08.020](https://doi.org/10.1016/j.physletb.2012.08.020) — Higgs boson discovery
- [YouTube: de Broglie Wavelength Explained](https://www.youtube.com/watch?v=TItdkDdldvU)

---

### Tasks

#### Part (a): Ionizing Radiation of Hydrogen

Given the ionization energy of hydrogen in its ground state is:

```
E_ion = 13.6 eV
```

Compute the frequency \( \nu \), wavelength \( \lambda \), and wavenumber \( k \) of the photon required for ionization.

**Step-by-step solution:**

1. Use \( E = h \nu \) with \( h = 4.14 \times 10^{-15} \text{ eV·s} \):

   \[
   \nu = \frac{E_{\text{ion}}}{h} = \frac{13.6}{4.14 \times 10^{-15}} \approx 3.29 \times 10^{15} \, \text{Hz}
   \]

2. Calculate the wavelength using \( \lambda = \frac{c}{\nu} \) with \( c = 3.00 \times 10^8 \, \text{m/s} \):

   \[
   \lambda = \frac{3.00 \times 10^8}{3.29 \times 10^{15}} \approx 9.11 \times 10^{-8} \, \text{m} \quad (91 \, \text{nm})
   \]

3. Compute the wavenumber \( k = \frac{2\pi}{\lambda} \):

   \[
   k = \frac{2\pi}{9.11 \times 10^{-8}} \approx 6.89 \times 10^7 \, \text{m}^{-1}
   \]

#### Part (b): de Broglie Wavelengths for Various Particles

Derive expressions and compute the de Broglie wavelength \( \lambda = \frac{h}{p} \) for different kinetic energies and physical cases.

---

##### Relativistic Case:

\[
E^2 = (pc)^2 + (m_0 c^2)^2 \Rightarrow p = \frac{\sqrt{E_{\text{kin}}^2 + 2 m_0 c^2 E_{\text{kin}}}}{c}
\Rightarrow \lambda = \frac{h c}{\sqrt{E_{\text{kin}}^2 + 2 m_0 c^2 E_{\text{kin}}}}
\]

##### Classical (non-relativistic) Case:

\[
E_{\text{kin}} = \frac{p^2}{2m_0} \Rightarrow p = \sqrt{2 m_0 E_{\text{kin}}} \Rightarrow \lambda = \frac{h}{\sqrt{2 m_0 E_{\text{kin}}}}
\]

##### Ultrarelativistic Case:

\[
p \approx \frac{E_{\text{kin}}}{c} \Rightarrow \lambda = \frac{h c}{E_{\text{kin}}}
\]

---

**Now compute the following:**

1. **Electron, \( E_{\text{kin}} = 10 \text{ eV} \):**

   Use classical model:

   \[
   m_e = 511 \times 10^3 \text{ eV}/c^2 \Rightarrow p = \sqrt{2 \cdot 511000 \cdot 10} = 3195 \text{ eV}/c
   \Rightarrow \lambda \approx \frac{1.242 \times 10^{-6}}{3195} \approx 3.89 \times 10^{-10} \text{ m}
   \]

2. **Electron, \( E_{\text{kin}} = 1 \text{ GeV} \):**

   Use ultrarelativistic model:

   \[
   \lambda = \frac{1.242 \times 10^{-6}}{1 \times 10^9} = 1.24 \times 10^{-15} \text{ m}
   \]

3. **Higgs boson, \( m = 125 \text{ GeV}/c^2, E_{\text{kin}} = 1 \text{ GeV} \):**

   Use classical model:

   \[
   p = \sqrt{2 \cdot 125 \cdot 10^9 \cdot 10^9} = 1.58 \times 10^{10} \text{ eV}/c
   \Rightarrow \lambda = \frac{1.242 \times 10^{-6}}{1.58 \times 10^{10}} \approx 7.86 \times 10^{-17} \text{ m}
   \]

4. **Dust particle, \( m = 10^{-12} \text{ kg}, v = 1 \text{ m/s} \):**

   Use classical expression:

   \[
   \lambda = \frac{6.626 \times 10^{-34}}{10^{-12} \cdot 1} = 6.63 \times 10^{-22} \text{ m}
   \]

---

### Questions

1. Why can different models (classical, relativistic, ultrarelativistic) be used for the same formula depending on the regime?
2. How does the de Broglie wavelength scale with particle mass and velocity? Provide examples from your calculations.
3. Would it be feasible to detect the de Broglie wavelength of a dust particle? Why or why not?

---

### Advice

This exercise is an excellent opportunity to integrate fundamental quantum mechanics with relativistic physics. Don’t rush through the derivations — understanding how the assumptions lead to different forms of momentum is key. When working with de Broglie wavelengths, always check the energy scale: electrons often allow classical approximations, but particles like Higgs bosons require careful relativistic treatment. For even more practice, try extending these calculations to protons or muons using similar steps as outlined here. Confidence builds with repetition — revisit this sheet when tackling problems involving particle-wave duality in other contexts.