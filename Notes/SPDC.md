#SPDC

## Definition

> [!note] Definition
> SPDC stands for Spontaneous Parametric Down Conversion which is also commonly known as three wave-mixing process including pump, signal, and idler. It is a popular technique used to create a [[ bipartite entanglement]] for various quantum applications. SPDC is also known by another name called [[parametric fluorescence]].

![[2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals.pdf#page=3&rect=300,94,557,236|2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals, p.3]]
## Types of SPDC

There are 3 types of SPDC in total which is categorized by the relationship between the polarization of the pump, signal and idler photons.

- **Type-0**  $\ket{H} \rightarrow \ket{HH}$
  In Type-0 SPDC, the pump, signal, and idler photons share the same polarization ($z_p z_s z_i$ in KTP). This process has the **largest nonlinear coefficient** of all three types — for ppKTP, $d_{zzz} \approx 18.5\ \text{pm/V}$ — making it the brightest in terms of raw pair-generation rate [[Steinlechner et al. 2014]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=2|page 2]]. Experimentally, the spectral brightness of Type-0 was measured to be approximately **20× higher** than Type-II in the same optical setup.

  However, these advantages come with trade-offs. The FWHM bandwidth of the Type-0 process is **significantly wider** than Type-II (e.g., ~2.3 nm vs. ~0.3 nm at nondegenerate operation), and the bandwidth grows dramatically near wavelength degeneracy ($\lambda_s = \lambda_i = 2\lambda_p$). The center wavelengths of Type-0 emission are also strongly sensitive to crystal temperature, shifting considerably over a range of 20°C–50°C [[Steinlechner et al. 2014]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=3|page 3]].

- **Type-I**  $\ket{H} \rightarrow \ket{VV}$
  In Type-I SPDC, the signal and idler photons are orthogonally polarized with respect to the pump, but co-polarized with each other ($z_p y_s y_i$ in KTP). The nonlinear coefficients of Type-I and Type-II are of similar magnitude due to Kleinman symmetry ($d_{zyy} \approx 4.7\ \text{pm/V}$). The spectral characteristics of Type-I (bandwidth and temperature dependence) are comparable to those of Type-0, since both involve co-polarized signal and idler photons. Because Type-I offers spectral behavior similar to Type-0 but with significantly **lower efficiency**, it is generally not preferred for entanglement sources in ppKTP and is omitted from direct comparison [[Steinlechner et al. 2014]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=2|page 2]].

- **Type-II**  $\ket{H} \rightarrow \ket{HV}$
  In Type-II SPDC, the signal and idler photons are **orthogonally polarized** ($y_p y_s z_i$ in KTP), with a nonlinear coefficient $d_{yyz} \approx 3.9\ \text{pm/V}$. Because the two generated photons experience different group velocities in the crystal, the Type-II process has a **much narrower bandwidth** than Type-0 (e.g., ~0.3 nm FWHM vs. ~2.3 nm at nondegenerate Type-0 operation), and the center wavelengths are **far less sensitive to temperature** changes [[Steinlechner et al. 2014]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=3|page 3]].

  The narrow bandwidth and spectral stability make Type-II the preferred configuration for most quantum communication and entanglement applications where spectral control is important. Heralding efficiencies for Type-II in a Sagnac configuration have been demonstrated at $\eta_s \approx 0.45$, $\eta_i \approx 0.39$ without correction for detector inefficiency [[Steinlechner et al. 2014]] [[2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf#page=4|page 4]].


## [[Entanglement Sources]]

SPDC is the most widely used physical process for generating polarization-entangled photon pairs. Various optical configurations have been developed around it to prepare photon pairs in maximally entangled [[Bell state|Bell states]], as reviewed in [[Anwar 2021]].

SPDC-based source works well at room temperature for entanglement generation but still faces statistical fluctuation which makes it act less like on-demand single photon source without complex heralding [[Heindel 2023]] [[2023 - Heindel - Quantum dots for photonic quantum information technology.pdf#page=4&selection=145,39,163,53&color=yellow|p.4]]. 

For a detailed treatment of source architectures — including the **linear beam displacement interferometer** used by the SpooQy group — see [[Entanglement Sources]].

[[SPDC]] source doesn't scale well with increasing brightness requirement. The quanlity of the generated photons degrate quickly as the pump power increases [[Senellart 2017]] [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=4&selection=39,0,92,1&color=red|p.1029]].