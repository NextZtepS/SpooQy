---
Authors:
  - "[[Xiaodong Shi]]"
  - "[[Yue Li]]"
  - "[[Jinyi Du]]"
  - "[[Lin Zhou]]"
  - "[[Ran Yang]]"
  - "[[En Teng Lim]]"
  - "[[Sakthi Sanjeev Mohanraj]]"
  - "[[Mengyao Zhao]]"
  - "[[Xu Chen]]"
  - "[[Xiaojie Wang]]"
  - "[[Guangxing Wu]]"
  - "[[Hao Hao]]"
  - "[[Veerendra Dhyani]]"
  - "[[Sihao Wang]]"
  - "[[Alexander Ling]]"
  - "[[Di Zhu]]"
Publication: "[[Nature]]"
Title: Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks
Year: "2026"
tags:
  - SPDC
  - EntanglementSource
  - QPM
  - IntegratedPhotonics
---
[[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf|Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks]]

## Key Results

The [[Lithium Niobate (LN)]] waveguide for type-0 and type-II are put in series. The TE pump creates a type-0 pairs in TE mode and a type-I pairs in TM mode [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=3&selection=31,2,40,58&color=yellow|p.3]].  The design resembles a dual crystal + single-pass design explained in [[2021 Anwar]].

![[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=14&rect=72,506,283,626&color=red|p.14]]

Combining the pairs in TE ($\ket{H_s H_i}$) and TM ($\ket{V_s V_i}$) modes gives an entangled state $\alpha \ket{H_s H_i} + e^{i\phi} \beta \ket{V_s V_i}$ right out of the end of the waveguide with the need of extra components. The probabilty amplitudes are tuned via section length, and the relative phase is tuned using thermo-optic phase shifter [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=3&selection=58,0,141,72&color=yellow|p.3]].

The imperfections in manufacturing process makes the probability amplitudes (generation rates) hard to control. Changing temperature makes the phase matching condition varies on opposite direction for type-0 and type-I, enabling it as a tuning parameter [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=4&selection=37,0,66,7&color=yellow|p.4]].

The photon pairs are generated uniformly across different chosen Dense Wavelength Division Multiplexing ([[DWDM]]) channels. This is investigated with [[Joint Spectral Intensities]] (JSI) [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=4&selection=227,0,228,86&color=yellow|p.4]] [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=5&selection=0,0,2,86&color=yellow|p.5]].

![[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=15&rect=235,590,537,721&color=red|p.15]]

The polarization entanglement quality is inspected by choosing a corresponding channels, which satisfy energy conservation, to get polarization visibility yielding $99.8\%$ Bell-state fidelities [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=5&selection=10,0,88,1&color=yellow|p.5]].

The visibilties remains $\gt 90\%$ for all basis pairs when deployed in the [[Singapore National Quantum-Safe Network]] [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=5&selection=121,28,198,67&color=yellow|p.5]].

## Key Arguments

> ([[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=2&selection=18,2,29,1&color=note|p.2]])
> In type-II spontaneous parametric down-conversion (SPDC), the orthogonal polarizations of signal and idler photons usually have limited phase-matching bandwidth due to polarization-dependent dispersion. Traditional type-0/I SPDC in bulk nonlinear crystals avoids these drawbacks, but requires rotation of the pump or the photon-pair polarization, or crystal orientation, often implemented with delicate free-space optical setups.

> ([[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=2&selection=60,0,68,70&color=yellow|p.2]])
> In this work, we introduce a dual quasi-phase matched (D-QPM) periodically poled lithium niobate (PPLN) nanophotonic waveguide, that directly generates polarizationentangled photon pairs via sequential type-0 and type-I SPDC in a single device. This design eliminates the need for interferometric or polarization-manipulating circuits, while offering flexible and in situ phase-matching control and phase tuning.

Insertion loss and chp-to-fiber coupling loss remains challenging [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=6&selection=2,32,4,57&color=red|p.6]].

The phase matching temperature tuning is a good tool for mitigating fabrication imperfection [[2026 - Shi et al. - Integrated polarization-entangled photon source for wavelength-multiplexed quantum networks.pdf#page=6&selection=29,2,31,66&color=important|p.6]].

