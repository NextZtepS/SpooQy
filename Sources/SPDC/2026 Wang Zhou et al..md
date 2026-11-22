---
Authors:
  - "[[Xiaojie Wang]]"
  - "[[Lin Zhou]]"
  - "[[Yue Li]]"
  - "[[Sakthi Sanjeev Mohanraj]]"
  - "[[Xiaodong Shi]]"
  - "[[Zhuoyang Yu]]"
  - "[[Ran Yang]]"
  - "[[Xu Chen]]"
  - "[[Guangxing Wu]]"
  - "[[Hao Hao]]"
  - "[[Sihao Wang]]"
  - "[[Veerendra Dhyani]]"
  - "[[Di Zhu]]"
Publication: "[[Physical Review Letters]]"
Title: On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs
Year: "2026"
tags:
  - SPDC
  - IntegratedPhotonics
  - QPM
  - Pulsed
  - Bandwidth
  - SpectralPurity
  - PhotonSource
---
[[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf|On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs]]

## Arguments

Group velocity matching using higher-order TE mode and gaussian-apodized pooling helps achieve high [[Spectral Purity]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&annotation=343R|p.1]].

[[SPDC]] generally exhibits spectral correlation that reduces the [[Spectral Purity]] of the heralded photon. The reduced [[Spectral Purity]] is undesirable as it reduces interference visibility [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&selection=145,34,162,37&color=red|p.1]].

### Existing Approaches for high [[Spectral Purity]]

- [[SPDC]] [[Optical Cavities]] -> limited bandwidth and resonance fluctuation [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&selection=184,5,188,6&color=yellow|p.1]].
- Type-II [[SPDC]] that matches the group velocity using polarization dependent dispersion management e.g. like beam displacement source in [[2025 Chin]] -> many rotators and combiners which are lossy in integrated system [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&selection=201,0,223,32&color=important|p.1]].
- Backward-wave [[SPDC]] in [[2023 Kuo et al.]] can make a very narrow band photons but requires sub-um pooling -> hard to manufacture [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&selection=223,34,230,37&color=important|p.1]].

[[Thin-Film Lithium Niobate (TFLN)]] offers great electro-optic tunability and model engineering through waveguide geometry [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=2&selection=6,0,25,5&color=important|p.2]].

[[Spectral Purity]] is achieved when [[Phase Matching Function]] is orthogonal the [[Pump Envelope Function]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&annotation=370R|p.3]]. The [[Pump Envelope Function]] is always antidiagonal because it must fulfill the energy conservation; however, the [[Phase Matching Function]] can be rotated by carefully matching the group velocities of interacting fields (first-order expansion of the wavevector $k$) [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&annotation=378R|p.3]].

[[Phase Matching Function]] contains normalized nonlinearity profile that can be tuned by aperiodic pooling to suppress the side lobes. A guassian width of $\sigma = L/5$ seems to be a common choice for many experiments [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&selection=295,0,348,18&color=yellow|p.3]].

> ([[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&selection=348,19,369,14&color=important|p.3]])
> For the modal configuration in Fig. 1(a) with a matched pump bandwidth, periodic poling yields a sinc-shaped JSA with strong spectral correlations [Fig. 1(d)]. In contrast, Gaussian-apodized poling on the same waveguide produces a smooth and highly factorable JSA [Fig. 1(e)], improving the theoretical spectral purity from 84% to 99%. The complete poling configuration is shown in Fig. S9 [34]. 

![[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=2&rect=102,466,511,749&color=important|p.2]]

Unheralded $g^{(2)}$ Measurement also covers the phase-dependent correlation unlike the [[Joint Spectral Intensity (JSI)]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=5&annotation=411R|p.5]].

## Results

> ([[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=1&annotation=346R|p.1]])
> The resulting heralded photons exhibit spectral purities up to 94% inferred from joint-spectral intensity and 89% from unheralded $g^{(2)}$  measurement.

[[Second Harmonic Generation (SHG)]] was used to confirm that aperiodic pooling could shape the [[Phase Matching Function]] as expected [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&annotation=386R|p.3]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=4&selection=9,15,16,25&color=yellow|p.4]].

![[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=3&rect=307,435,571,748&color=note|p.3]]

Two methods were used to verify the [[Spectral Purity]]: 1) [[Joint Spectral Intensity (JSI)]] and 2) Unheralded $g^{(2)}$ Measurement [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=4&annotation=400R|p.4]]. 

Femtosecond pump laser was used and shaped to match the [[Phase Matching Function]] and a long SMF-28 fiber was used the measure the frequency by mapping from time dispersion (0.15nm resolution) [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=4&annotation=403R|p.4]].

The recovered [[Joint Spectral Intensity (JSI)]] was used to perform Schmidt decomposition and obtained Schmidt number of 1.06 (~94% purity) compared to a perfect 1 [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=4&selection=117,16,158,1&color=yellow|p.4]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=5&selection=0,0,76,1&color=yellow|p.5]].

![[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=4&rect=308,520,520,748&color=yellow|p.4]]

The unheralded  $g^{(2)}$ for the signal and idler 82% and 89% respectively because the phase-dependent correlation is now included unlike [[Joint Spectral Intensity (JSI)]] [[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=5&selection=144,0,222,56&color=yellow|p.5]].

![[2026 - Wang et al. - On-Chip Generation of Copolarized and Spectrally Separable Photon Pairs.pdf#page=5&rect=128,647,483,747&color=yellow|p.5]]