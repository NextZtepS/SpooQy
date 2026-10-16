## Definition

> [!note] Definition
> SPDC stands for Spontaneous Parametric Down Conversion which is also commonly known as three wave-mixing process including pump, signal, and idler. It is a popular technique used to create a [[ bipartite entanglement]] for various quantum applications. SPDC is also known by another name called [[parametric fluorescence]].

![[2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals.pdf#page=3&rect=300,94,557,236|2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals, p.3]]

---
## Types of SPDC

There are 3 types of SPDC in total which is categorized by the relationship between the polarization of the pump, signal and idler photons. The possibilty of each type depends on the [[Phase Matching]] conditions.

- **Type-0**  $\ket{H} \rightarrow \ket{HH}$
  In Type-0 SPDC, the pump, signal, and idler photons share the same polarization ($z_p z_s z_i$ in KTP). This process has the **largest nonlinear coefficient** of all three types — for ppKTP, $d_{zzz} \approx 18.5\ \text{pm/V}$ — making it the brightest in terms of raw pair-generation rate [[2014 Steinlechner et al.]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=2|page 2]]. Experimentally, the spectral brightness of Type-0 was measured to be approximately **20× higher** than Type-II in the same optical setup.

  However, these advantages come with trade-offs. The FWHM bandwidth of the Type-0 process is **significantly wider** than Type-II (e.g., ~2.3 nm vs. ~0.3 nm at nondegenerate operation), and the bandwidth grows dramatically near wavelength degeneracy ($\lambda_s = \lambda_i = 2\lambda_p$). The center wavelengths of Type-0 emission are also strongly sensitive to crystal temperature, shifting considerably over a range of 20°C–50°C [[2014 Steinlechner et al.]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=3|page 3]].

- **Type-I**  $\ket{H} \rightarrow \ket{VV}$
  In Type-I SPDC, the signal and idler photons are orthogonally polarized with respect to the pump, but co-polarized with each other ($z_p y_s y_i$ in KTP). The nonlinear coefficients of Type-I and Type-II are of similar magnitude due to Kleinman symmetry ($d_{zyy} \approx 4.7\ \text{pm/V}$). The spectral characteristics of Type-I (bandwidth and temperature dependence) are comparable to those of Type-0, since both involve co-polarized signal and idler photons. Because Type-I offers spectral behavior similar to Type-0 but with significantly **lower efficiency**, it is generally not preferred for entanglement sources in ppKTP and is omitted from direct comparison [[2014 Steinlechner et al.]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=2|page 2]].

- **Type-II**  $\ket{H} \rightarrow \ket{HV}$
  In Type-II SPDC, the signal and idler photons are **orthogonally polarized** ($y_p y_s z_i$ in KTP), with a nonlinear coefficient $d_{yyz} \approx 3.9\ \text{pm/V}$. Because the two generated photons experience different group velocities in the crystal, the Type-II process has a **much narrower bandwidth** than Type-0 (e.g., ~0.3 nm FWHM vs. ~2.3 nm at nondegenerate Type-0 operation), and the center wavelengths are **far less sensitive to temperature** changes [[2014 Steinlechner et al.]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=3|page 3]].

  The narrow bandwidth and spectral stability make type-II the preferred configuration for most quantum communication and entanglement applications where spectral control is important. Heralding efficiencies for type-II in a Sagnac configuration have been demonstrated at $\eta_s \approx 0.45$, $\eta_i \approx 0.39$ without correction for detector inefficiency [[2014 Steinlechner et al.]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=4|page 4]].

---
## [[Phase Matching]]

Phase matching determines the actual wavelengths and type of the SPDC possible in a specific crystal.

---

## Spectral Bandwidth

Photons generated from SPDC are spatio-spectral correlated, meaning its spectrum varies with spatial mode/collection. The correlation comes from the energy and momentum conservations ([[Phase Matching]]) between the generated pairs [[2026 Barcons Planas]] [[2026 - Barcons Planas - Pure narrowband photon-pair generation in a monolithic cavity.pdf#page=1&selection=100,19,104,80&color=yellow|p.1]]. 

In general, SPDC photons distinguishable when using for interference with other photons as measuring the heraled partner would tell the spectral characteristic of its pair; a narrow spectral filtering in needed to let it interfere with other indendently created photons [[2017 Huber et al.]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=5&selection=97,0,97,74&color=red|p.5]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=6&selection=3,0,18,12&color=red|p.6]]. 

There are methods to go about this [[2026 Barcons Planas]]:
- Spatial/Spectral filter - trade off with brightness
- Engineering - use waveguide to confine the spatial mode, group velocity matching, counter/back propagating signal and idler, crystal domain engineer
- [[Optical Cavities]] - use resonant frequency mode of the cavity to enhance certain spatial/spectral modes.

---
## [[Entanglement Sources]]

SPDC is the most widely used physical process for generating polarization-entangled photon pairs. Various optical configurations have been developed around it to prepare photon pairs in maximally entangled [[Bell state|Bell states]], as reviewed in [[2021 Anwar]].

SPDC-based source works well at room temperature for entanglement generation but still faces statistical fluctuation which makes it act less like on-demand single photon source without complex heralding [[2023 Heindel]] [[2023 - Heindel - Quantum dots for photonic quantum information technology.pdf#page=4&selection=145,39,163,53&color=yellow|p.4]]. 

For a detailed treatment of source architectures — including the **linear beam displacement interferometer** used by the SpooQy group — see [[Entanglement Sources]].

[[SPDC]] source doesn't scale well with increasing brightness requirement. The quanlity of the generated photons degrate quickly as the pump power increases [[2017 Senellart]] [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=4&selection=39,0,92,1&color=red|p.1029]].

---

## Interaction Hamiltonian

This summarized from  [[2021 Anwar]] and [[2021 Zhang]].

### The General 3D Interaction Hamiltonian
$$\mathcal{H}_I = \epsilon_0 \int d^3r \chi^{(2)} E_p^{(+)}(\mathbf{r},t) \hat{E}_s^{(-)}(\mathbf{r},t) \hat{E}_i^{(-)}(\mathbf{r},t) + \text{H.c.}$$
We apply the following assumption to tackle the Hamiltonian:
- The non-depleted classical pump field is defined using its **transverse momentum spatial mode** $A_p(\mathbf{k}_p^\perp)$ and **spectral function** $S(\omega_p)$.
- The signal and idler fields are quantized using creation operators $\hat{a}^\dagger_{\mathbf{k}_{s,i}}$.
- Recall the time evolution of the state is given by $\vert{}\Psi(t)\rangle = e^{- \frac{i}{\hbar} \int_0^t \mathcal{H}_I(t') dt'} \vert{}0\rangle_s \vert{}0\rangle_i$. In the weak-pump regime, the probability of single pair emission is isolated by truncating the Taylor series expansion of the state evolution to the first order: $\vert{}\Psi(t)\rangle \propto \int_0^t \mathcal{H}_I(t') dt' \vert{}0\rangle_s \vert{}0\rangle_i$.

The integral can be expressed as
$$\vert{}\Psi(t)\rangle \propto \frac{\epsilon_0 e_p \chi^{(2)} e_s e_i}{(2\pi)^3} \int d\omega_s d\omega_i dk_s^\perp dk_i^\perp \times \left[ A_p(k_p^\perp) S(\omega_p) N_p N_s N_i \int_0^t dt e^{i(\omega_p - \omega_s - \omega_i)t} \times \int_{-\infty}^{\infty} dx e^{i(k_{px} - k_{sx} - k_{ix})x} \int_{-\infty}^{\infty} dy e^{i(k_{py} - k_{sy} - k_{iy})y} \times \int_{-L/2}^{L/2} dz e^{i(k_{pz} - k_{sz} - k_{iz})z} \right] \vert{}k_s^\perp, \omega_s\rangle \vert{}k_i^\perp, \omega_i\rangle$$

**Time Integral:** $\int_0^t dt e^{i(\omega_p - \omega_s - \omega_i)t} = \delta(\omega_p - \omega_s - \omega_i)$ represents the time evolution over the interaction period $t$, which ultimately evaluates to energy conservation.

**Transverse Spatial Integrals:** $\int_{-\infty}^{\infty} dx e^{i(k_{px} - k_{sx} - k_{ix})x}$ and $\int_{-\infty}^{\infty} dy e^{i(k_{py} - k_{sy} - k_{iy})y}$ represent the integration over the effectively infinite transverse cross-section of the pump beam, establishing transverse momentum conservation. The collapse to  $\delta(k_{\perp p} - k_{\perp s} - k_{\perp i})$.

**Longitudinal Spatial Integral:** $\int_{-L/2}^{L/2} dz e^{i(k_{pz} - k_{sz} - k_{iz})z} = \text{sinc}\left(\frac{\Delta k_z L}{2}\right)$ integrates the phase mismatch strictly over the finite thickness ($L$) of the nonlinear crystal.

**Frequency and Momentum Integrals:** $\int d\omega_s d\omega_i dk_s^\perp dk_i^\perp$ sum over all possible frequencies and transverse momenta to build the final continuous state vector.

The full 3D bi-photon state evaluates to 
$$\vert{}\Psi(t)\rangle \propto \int d\omega_s d\omega_i d\mathbf{k}_s^\perp d\mathbf{k}_i^\perp \Phi(\mathbf{k}_s^\perp, \mathbf{k}_i^\perp, \omega_s, \omega_i) \vert{}\mathbf{k}_s^\perp, \omega_s\rangle_s \vert{}\mathbf{k}_i^\perp, \omega_i\rangle_i$$
The governing 3D mode function is 
$$\Phi(\mathbf{k}_s^\perp, \mathbf{k}_i^\perp, \omega_s, \omega_i) = L \sigma A_p(\mathbf{k}_s^\perp + \mathbf{k}_i^\perp) S(\omega_s + \omega_i) \text{sinc}\left(\frac{\Delta k_z L}{2}\right)$$

### Simplification to Z-Propagation (Plane Wave)

A standard simplifying condition assumes the pump and SPDC transverse modes are much smaller than the nonlinear material's cross-section, reducing the susceptibility tensor to a single coefficient $d$.

By restricting all field propagation to the collinear longitudinal $z$-axis, the transverse momentum components become zero ($k_s^\perp = k_i^\perp = 0$).

The integrals over transverse momentum collapse, reducing the quantum state to a 1D frequency-dependent integral to 
$$\vert{}\Psi(t)\rangle \propto \int d\omega_s d\omega_i \Phi(\omega_s, \omega_i) \vert{}\omega_s\rangle_s \vert{}\omega_i\rangle_i$$

The spatial pump mode $A_p(\mathbf{k}_s^\perp + \mathbf{k}_i^\perp)$ simplifies to a constant on-axis amplitude $A_p(0)$.

The longitudinal wave-vector mismatch $\Delta k_z$ becomes the total collinear phase mismatch $\Delta k = k_p - k_s - k_i$.

In the end, we have
$$\Phi(\omega_s, \omega_i) = L \sigma A_p(0) S(\omega_s + \omega_i) \text{sinc}\left(\frac{\Delta k L}{2}\right)$$
where  $\sigma$ is the effective nonlinear coefficient
$$\sigma = d \sqrt{\frac{\hbar^3 \omega_p \omega_s \omega_i}{32 \pi^4 \epsilon_0 c^3 n_p(\omega_p) n_s(\omega_s) n_i(\omega_i)}}$$

### Joint Spectral Amplitude and Intensity

The Joint Spectral Intensity (JSI) represents the physically measurable probability distribution of generating a specific photon pair.

The JSI is calculated by taking the absolute square of the mode function
$$\text{JSI} = \vert{}L \sigma A_p(0) S(\omega_s + \omega_i) \text{sinc}\left(\frac{\Delta k L}{2}\right)\vert{}^2$$