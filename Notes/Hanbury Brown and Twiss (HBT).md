
The Hanbury Brown and Twiss (HBT) experiment tests whether a light field contains **no more than one photon**, which is the [[single-photon purity]] of a source. The light is sent to a 50:50 beamsplitter with a single-photon detector on each output, and a correlation card records the time delay between clicks on the two detectors [[2017 Senellart]] [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2&selection=92,0,98,1&color=note|p.1027]].

![[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2&rect=82,191,306,344&color=yellow|2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources, p.1027]]

A single photon cannot split, so it triggers only one detector. A coincidence at zero delay therefore requires at least two photons. This is measured by the second-order correlation function [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2|p.1027]]:
$$ g^{(2)}(0) = \frac{\langle n_1(t)\,n_2(t)\rangle_t}{\langle n_1(t)\rangle_t\,\langle n_2(t)\rangle_t} \approx \frac{2p(2)}{p(1)^2} $$
Here $p(n)$ is the probability of $n$ photons. $g^{(2)}(0) = 0$ for an ideal single-photon source and $1$ for a laser ([[Quantum Dots#Requirement Parameters as a quantum emitter|QD parameters]]). HBT only sees detection events, so it says nothing about the vacuum component $p(0)$. That is measured separately as the brightness $\mathcal{B}$ [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2|p.1027]].

## Pulsed vs. CW

- **Pulsed:** coincidences appear as peaks at multiples of the repetition period, from photons emitted in different pulses. The **area of the zero-delay peak** relative to the side peaks gives $g^{(2)}(0)$ [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2|p.1027]].

![[2011 - Polyakov et al. - Coalescence of Single Photons Emitted by Disparate Single-Photon Sources The Example of InAs Quantum Dots and Parametric Down-Conversion Sources.pdf#page=2&rect=310,576,565,748|2011 - Polyakov et al. - Coalescence of Single Photons Emitted by Disparate Single-Photon Sources The Example of InAs Quantum Dots and Parametric Down-Conversion Sources, p.2]]

- **CW:** the histogram is continuous and shows an **antibunching dip** at $\tau = 0$, the same effect behind the $\perp$ reference in CW [[Hong-Ou-Mandel (HOM)]].

![[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=5&rect=136,264,294,480&color=note|2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network, p.5]]

## Heralded HBT (SPDC / SFWM)

For pair sources, the HBT is conditioned on detecting the herald (idler), which gives $g^{(2)}_{i,s,s}(0)$. Multi-photon emission grows with pump power, so purity sets an upper limit on brightness. In [[2019 Paudel et al.]], the [[SPDC]] stayed single-photon up to 65 mW of pump [[2019 - Paudel et al. - Direct excitation of a single quantum dot with cavity-SPDC photons.pdf#page=6&selection=84,19,117,49&color=yellow|p.6]].

## Link to HOM

Multi-photon terms add coincidences to both $C_\parallel$ and $C_\perp$, so $g^{(2)}(0) > 0$ lowers $V_{HOM}$ even for identical wavepackets. Many papers therefore report a purity-corrected indistinguishability $M^* = M + g^{(2)}(0)$, but $M$ remains the figure of merit for applications [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2|p.1027]].

## Examples

| Source                                                | $g^{(2)}(0)$                  | Ref.                                                                                                                                                                                                                                  |
| ----------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Two separate InGaAs [[Quantum Dots\|QDs]]             | > 90 % purity                 | [[2010 Flagg et al.]] [[2010 - Flagg et al. - Interference of Single Photons from Two Separate Semiconductor Quantum Dots.pdf#page=2&selection=254,0,277,43&color=yellow\|p.2]]                                                        |
| InAs QD in CBG, CW above-band                         | 0.01                          | [[2026 Kim et al.]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=4\|p.4]]                                                        |
| Warm Cs [[SFWM]], heralded                            | 0.002                         | [[2026 Kim et al.]] [[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=5\|p.5]]                                                        |
| State-of-the-art QD sources                           | < 0.02                        | [[2017 Senellart]] [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=11&selection=163,0,178,1&color=yellow\|p.1036]]                                                                       |
