---
Authors:
  - "[[Tobias Huber]]"
  - "[[Maximilian Prilmüller]]"
  - "[[Michael Sehner]]"
  - "[[Glenn S. Solomon]]"
  - "[[Ana Predojević]]"
  - "[[Gregor Weihs]]"
Publication: "[[Quantum Science and Technology]]"
Title: Interfacing a quantum dot with a spontaneous parametric down-conversion source
Year: "2017"
tags:
  - LightMatter
  - QuantumDots
  - SPDC
  - Pulsed
  - HOM
---
[[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf|Interfacing a quantum dot with a spontaneous parametric down-conversion source]]

## Arguments

[[Quantum Dots]] excels at producing high purity single photons with low decoherence if cooled down the few Kelvins range [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=1&selection=93,0,98,84&color=important|p.1]].

[[SPDC]] is favorable for producing entangled photon pairs with tunable frequencies but can't be operated at high repitition rate due to random generation of photon pairs [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=1&selection=102,0,102,59&color=important|p.1]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=2&selection=3,0,9,67&color=important|p.2]].

Adjusting the SPDC photons to match the quantum dot photons is inspired by [[2011 Polyakov et al.]]

[[Hong-Ou-Mandel (HOM)]] looks at the coalescence between two photons which requires them to indistinguisable in time and polarization [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=2&selection=35,0,46,30&color=note|p.2]].

The bandwith of the common photon sources go like this: [[SPDC]] > [[Quantum Dots]] > [[Atomic Spectral Lines]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=2&selection=51,0,56,55&color=yellow|p.2]].

It is straightforward to get transform-limited wavepacket by filtering **mode-locked** pumped [[SPDC]] but **dephasing** in [[Quantum Dots]] is much more tricky to deal with [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=2&selection=63,0,67,82&color=red|p.2]].

==**Gap:**== Reducing the problem of dephasing in [[2011 Polyakov et al.]] by resonantly excite to [[Biexciton]] which has shorter lifetime compared to [[Exciton]]. Thus, this requires simpler **pulse strecher filter** and stabilization compared to **active tunable [[Fabry-Perot Cavity]] spectral filters** [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=3&selection=5,0,8,54&color=important|p.3]].

==**Sugguestion:**== Shorter-lifetime [[Quantum Dots]] (e.g. GaAs/AlGaAs by [[Droplet Epitaxy]]) are preferred over narrower SPDC filtering, since filtering costs heralding efficiency (see [[#Outlook]]) [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=13|p.13]]. 

## Results

[[Biexciton]] yield higher indisguishabilty compared to [[Exciton]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=3&selection=57,0,84,32&color=yellow|p.3]].

[[QD Dephasing]] (coherence) time $T_2$ is longer in [[Hong-Ou-Mandel (HOM)|HOM]] compared to [[Micheson Interferomenter]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=4&selection=114,0,121,85&color=yellow|p.4]].

Temperature tuning of [[SPDC]] enables the signal to match the [[Biexciton]] ($\ket{XX} \rightarrow \ket{X}$) wavelength at 919.6 nm [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=5&selection=70,0,77,4&color=yellow|p.5]].

Fiber Bragg grating is applied to spectrally filter (30 GHz) SPDC photons to improve its indisguishabilty from 39.94% to 96.3% [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=6&selection=22,51,33,20&color=yellow|p.6]].

The time/frequency shape of the [[SPDC]] is sinc function while that of the [[Quantum Dots]] is exponential decay [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=7&selection=38,0,61,6&color=red|p.7]].

The bandwidth of SPDC photons (100 GHz) and QD photons (1 GHz) are different as well. After the ==**pulse strecher filter**==, the heralding efficiency of the SPDC photons goes down together with the brightness [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=7&selection=65,0,81,25&color=red|p.7]].  

![[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=8&rect=132,546,460,709&color=note|p.8]]

![[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=11&rect=68,389,529,707&color=yellow|p.11]]

 The side peaks were obtained via shifting/delaying the heralded events by a repitition period of the pulse. The side peaks show delayed conicidence of events from a different pulse serving as a reference value of [[Hong-Ou-Mandel (HOM)]] measurement [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=9&selection=216,0,226,36&color=yellow|p.9]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=10&selection=3,0,4,30&color=yellow|p.10]].

The center peak (real HOM phenomena) was obtained by aggregating true coincident events (same pulse "triple" events) for 5.5 hrs combined from several blocks of time [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=10&selection=4,31,21,47&color=yellow|p.10]].

Limited by the timing jitter of the detector and coherence time of the [[Quantum Dots]], the coalescence probability achieved is 0.39 [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=11&selection=94,82,155,1&color=yellow|p.11]]. Filtering the time of the photon to only keep the photons detected closed to zeroth time yields coalescence probability of 0.63 [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=12&selection=14,14,21,61&color=important|p.12]].

## Discussion

Comparison with an earlier run using only the fiber Bragg grating and with [[2011 Polyakov et al.]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=13|p.13]]:

|                             | Fiber Bragg grating                 | Pulse stretcher                     | [[2011 Polyakov et al.]]                     |
| --------------------------- | ----------------------------------- | ----------------------------------- | -------------------------------------------- |
| SPDC filter $\Delta\nu$     | 30 GHz                              | 7.7 GHz                             | 0.9 GHz ([[Fabry-Perot Cavity]], stabilized) |
| QD excitation               | two-photon resonant ([[Biexciton]]) | two-photon resonant ([[Biexciton]]) | quasi-resonant (higher shell)                |
| $2T_1/T_2$                  | 3.0                                 | 3.0                                 | 5.7                                          |
| Max theoretical coalescence | 17 %                                | 36 %                                | 67 %                                         |
| Measured raw coalescence    | 18(4) %                             | 39(4) %                             | 16(3) %                                      |
| Time-selected coalescence   | 35(9) %                             | 63(5) %                             | 61 / 75 %                                    |
| Time selection efficiency   | 13.3 %                              | 12.6 %                              | 25 / 10 %                                    |

- **QD coherence beats filter narrowness**: Polyakov had a ~10× narrower filter (higher ceiling) but lower raw coalescence, because quasi-resonant excitation adds jitter and dephasing.
- Measured values reach or exceed the "max theoretical" because the Michelson $T_2$ underestimates the coherence relevant for [[Hong-Ou-Mandel (HOM)|HOM]] (spectral diffusion is quasi-static over ns).
- Time-selected result comparable to Polyakov **without active stabilization**.
- Still far below unity; post-selection discards ~87 % of events.
- Projection: this QD + bandwidth-matched [[Fabry-Perot Cavity]] filtering → ~86 % coalescence even with dephasing (model estimate, efficiency cost not quantified) [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=12|p.12]].

## Outlook

- Priority: [[Quantum Dots]] emitting highly indistinguishable (pure) photons, already shown for InAs/GaAs in cavities [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=12|p.12]].
- Filtering [[SPDC]] down to ≲ 1 GHz is possible but costly: 7.7 GHz filtering already cut heralding efficiency from 9.2 % to 1.5 % [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=6|p.6]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=7|p.7]].
- Alternative: intracavity (narrowband) [[SPDC]], see [[Optical Cavities]].
- Authors' preference: shorter-lifetime QDs (GaAs/AlGaAs, [[Droplet Epitaxy]], $T_1$ < 250 ps) → broader natural linewidth meets SPDC halfway, less filtering needed [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=13|p.13]].
- Long-term goal: QD spins as stationary qubits in [[Quantum Repeater]] nodes, entangling remote QDs via SPDC entanglement and [[Entanglement Swapping]] → [[Quantum Internet]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=13|p.13]].