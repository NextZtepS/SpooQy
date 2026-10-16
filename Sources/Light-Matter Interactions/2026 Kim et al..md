---
Authors:
  - "[[Kyu-Young Kim]]"
  - "[[Heewoo Kim]]"
  - "[[Dong Hyun Park]]"
  - "[[Jinhyuk Bae]]"
  - "[[Gyeongmin Ju]]"
  - "[[Suk In Park]]"
  - "[[Jin Dong Song]]"
  - "[[Je-Hyung Kim]]"
  - "[[Han Seb Moon]]"
Publication: "[[Light: Science & Applications]]"
Title: Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network
Year: "2026"
tags:
  - LightMatter
  - QuantumDots
  - SFWM
  - CW
  - HOM
  - HBT
---
[[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf|Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network]]

## Arguments

Other approaches (including [[Quantum Dots]] and [[SPDC]]) two-photon interference requires spectral modification on the photons to compensate for spectral mismatch. In addition, pulse operation is required for post-selection for different temporal modes. These 2 requirements makes it complex and inefficient for practical usages [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2&selection=139,0,174,58&color=important|p.2]].

[[Warm Atomic Ensembles]] and [[Quantum Dots]] have a compatible bandwidth making them good candiates for hybrid atom-QD interface [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2&selection=175,0,212,1&color=important|p.2]].

**==Gap:==** Previous studys used [[Warm Atomic Ensembles]] as a dispersive media for [[Quantum Dots]]'s photons only. The direct two-photon inteference between these 2 sources had not been done [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2&selection=248,2,269,40&color=important|p.2]].

Division of labour in a hybrid network: [[Quantum Dots]] give bright, on-demand, high-rate photons but suffer spectral randomness and can't store photons; atoms have identical energy levels, so they act as [[Quantum Memory]] and as a global frequency reference for remote QDs [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2|p.2]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=9|p.9]].

Wavelength compatibility: Cs 6P$_{3/2}$–6D$_{5/2}$ (917 nm) matches InAs/GaAs QDs; Rb 780 nm matches GaAs/AlGaAs QDs [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2|p.2]].

**==Suggestion:==** Main limits are detector jitter ≈ photon coherence time and the rate imbalance / multi-photon background of the [[SFWM]] source. Fixes: faster detectors or longer QD coherence via (quasi-)resonant excitation, strain or electric-field tuning instead of temperature tuning, and ∼10× better QD system efficiency → expected visibility > 0.95 [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=9|p.9]].

## Results

![[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=3&rect=58,199,288,444&color=yellow|p.3]]

### Warm Cs ensemble (heralded source)

[[SFWM]] in a ladder system 6S$_{1/2}$–6P$_{3/2}$–6D$_{5/2}$ of a 1 mm thick [[Warm Atomic Ensembles|warm Cs cell]] (105 °C), with counter-propagating CW pump (852 nm) and coupling (917 nm) lasers, gives signal (917.48 nm) + idler (852.35 nm) pairs. The idler is the herald [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=2|p.2]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=10|p.10]].

The thin cell improves pump/emission mode overlap and suppresses reabsorption → heralding efficiency up to 22 % (2 ns window), 18 % (320 ps), > 9 % (80 ps) at signal rates of 0.11–0.88 MHz [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=3|p.3]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=10|p.10]].

Signal–idler cross-correlation $g^{(2)}_{i,s}(0) = 1245$ (CAR ≈ 1244), heralding window 128 ps FWHM. Heralded $g^{(2)}_{i,s,s}(0) = 0.002$ → very high single-photon purity. Oscillations in $g^{(2)}$ come from hyperfine quantum beats / idler reabsorption [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4|p.4]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=5|p.5]].

[[Hong-Ou-Mandel (HOM)|HOM]] between two signal photons from the same cell (phase-matched at ±2°): raw dip 0.10, fitted visibility 1.00 ± 0.11, coherence time 161 ± 28 ps [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=6|p.6]].

### Quantum dot

InAs/GaAs [[Quantum Dots|QD]] in a hole-based [[Circular Bragg Grating]] low-Q cavity (broadband, ∼100× the QD linewidth) → simulated fibre coupling up to 27 %. CW **above-band** excitation at 780 nm, 0.44 MHz count rate [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=3|p.3]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4|p.4]].

Tuning is done on the QD, not the partner: 0.03 nm detuning at 7.5 K → resonance at 12.4 K by raising temperature, at the cost of phonon-induced linewidth broadening [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4|p.4]].

QD at 12.4 K: Lorentzian FWHM 2.17 ± 0.17 GHz, lifetime 1.01 ns, $g^{(2)}(0) = 0.01$. Self-HOM (4 m delay): raw 0.62, deconvolved 1.00 ± 0.10, coherence time 129 ± 18 ps [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4|p.4]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=6|p.6]].

### Two-photon interference Cs ↔ QD

Spectral overlap from scanning Fabry-Perot spectra: $A = 0.88 \pm 0.01$ **without spectral modification** → upper bound on indistinguishability $I_{id}$ [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4|p.4]]. (Note: the QD photons still pass a 50 GHz fibre band-pass filter, but it is ≫ linewidth, so no lossy narrowband filtering [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=10|p.10]].)

Three-fold coincidences (idler herald + both BS outputs), post-selected within 80 ps of the idler, under CW operation. Visibility defined time-resolved as $V(\tau) = (C_\perp - C_\parallel)/C_\perp$ [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=6|p.6]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=7|p.7]].

Detuned (0.03 nm): no difference between parallel and orthogonal (1.64 vs 1.59). Resonant: $C_\perp(0) = 1.28$ vs $C_\parallel(0) = 0.56$ → spectral identity is essential [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=7|p.7]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=8|p.8]].

Raw TPI visibility $V(0) = 0.41$ at a three-fold rate of 1.07 Hz, limited by system resolution (124 ps) ≈ TPI coherence time (119 ps). Deconvolved: 0.65 ± 0.14 [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=7|p.7]].

Visibility drops as the Cs/QD rate ratio $R_{s/QD}$ increases: multi-photon SFWM events add three-fold coincidences that don't interfere, and lost partners of a pair add uncorrelated background. Model ($\eta_s = 0.37$, $\eta_i = 0.57$, $I_{id} = 0.88$, QD system efficiency $\mu = 0.019$) fits the data [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=7|p.7]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=8|p.8]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=9|p.9]].

QD efficiency budget: collection 0.27 × transmission 0.14 × detection 0.50 is the bottleneck [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=9|p.9]].

CW + time-resolved coincidence detection (gating done in post-processing) is compatible with continuous-detection [[Entanglement Swapping]] between remote nodes [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=9|p.9]].

## Comparison with QD–SPDC TPI

| | [[2011 Polyakov et al.]] | [[2017 Huber et al.]] | This work |
|---|---|---|---|
| Partner source | [[SPDC]] | [[SPDC]] (ppKTP, type II) | [[SFWM]] in warm Cs |
| Operation | pulsed | pulsed (82 MHz) | **CW** |
| Who is tuned | partner filtered to QD | SPDC temperature-tuned to QD | **QD** temperature-tuned to atom |
| Partner raw bandwidth | ∼500 GHz | ∼100 GHz | ∼GHz (intrinsically narrow) |
| Partner filtering | 0.9 GHz [[Fabry-Perot Cavity]], active | 7.7 GHz pulse stretcher | none (50 GHz band-pass only) |
| QD excitation | quasi-resonant | two-photon resonant ([[Biexciton]]) | above-band CW (780 nm) |
| QD linewidth | 1.1 GHz | 1.2 GHz | 2.17 GHz (broadened at 12.4 K) |
| Heralding efficiency | — | 9.2 % → 1.5 % after filter | 9–22 % (window-dependent) |
| Timing resolution | — | 240 ps | 124 ps |
| Raw result | 16 % | 39 % | 41 % |
| Improved result | 61–75 % (time post-selection) | 63 % (time post-selection) | 65 % (detector deconvolution) |

> [!warning] Numbers are not directly comparable
> - [[2011 Polyakov et al.]] and [[2017 Huber et al.]] report the coalescence $P_C = (A_\perp - A_\parallel)/A_\perp$ from the **area** of the whole central peak; this work reports the **time-resolved** visibility at $\tau = 0$, which is naturally higher than the area-based value.
> - Huber's 63 % is real data kept after post-selection (12.6 % of events); this work's 65 % is a **deconvolution** of the detector response, i.e. what an ideal detector would show, not something achieved.
> - Fairest comparison: the raw numbers (∼0.4 for both Huber and Kim), keeping the metric difference in mind.

> [!tip] Key contrasts
> - **Filtering cost vs intrinsic match**: SPDC is broadband, so matching the QD costs heralding efficiency (Huber: 9.2 % → 1.5 %). Cs SFWM photons are intrinsically GHz-wide, so no lossy filtering is needed.
> - **Direction of tuning is reversed**: SPDC is tunable and adapts to the QD; the atom is a fixed frequency standard, so the QD must be tuned, and temperature tuning broadens it ([[QD Dephasing]]).
> - **Pulsed vs CW**: Huber defines temporal modes with laser pulses (and uses a pseudo-time axis for the side-peak reference); Kim uses CW + idler heralding and time-resolved detection, with the accidental level at large $\tau$ as the reference.
> - **Shared limit**: both are limited by detector jitter comparable to the coherence time (Huber 240 ps vs $T_2$ = 216 ps; Kim 124 ps vs 119 ps).
> - **Shared multi-photon issue**: both spontaneous pair sources (SPDC, SFWM) emit multi-pair events that dilute interference; Kim quantifies this via $R_{s/QD}$, while Huber kept SPDC rates low.
> - **Open opportunity**: Kim's QD is above-band excited and thermally broadened; Huber's two-photon resonant [[Biexciton]] excitation (less jitter, less dephasing) is exactly the kind of improvement Kim suggests.

