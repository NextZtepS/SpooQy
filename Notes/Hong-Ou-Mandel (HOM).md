
Hong-Ou-Mandel (HOM) interference is the **coalescence** of two indistinguishable photons at a 50:50 beamsplitter. The amplitudes for *both transmitted* and *both reflected* cancel ($t^2 + r^2 = 0$ with $r = i/\sqrt{2}$), so the photons always exit through the same port and the coincidence rate between the two outputs vanishes. This requires the photons to be identical in every degree of freedom (spatial mode, time-frequency, polarization). Fully distinguishable photons behave classically and give coincidences half the time [[2017 Huber et al.]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=10&selection=22,0,41,12&color=note|p.10]].

![[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2&rect=314,191,519,342|2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources, p.1027]]

For normalization, the photons are made distinguishable on purpose, usually by rotating one polarization ($\perp$) or delaying one photon by more than its coherence time. Comparing the parallel coincidences $C_\parallel$ with this reference $C_\perp$ gives the visibility [[2017 Senellart]] [[2017 - Senellart - High-performance semiconductor quantum-dot single-photon sources.pdf#page=2|p.2]]:
$$ V_{HOM} = \frac{C_\perp - C_\parallel}{C_\perp} $$
$V_{HOM}$ equals the indistinguishability $M$ for a 50:50 beamsplitter. It runs from 0 (distinguishable) to 1 (identical).

---
## Pulsed HOM

Both sources are triggered by the same mode-locked laser, so in each repetition period $T_L$ one photon from each source reaches the beamsplitter at the same time. Coincidences are histogrammed against the detection time difference, which gives a comb of peaks at multiples of $T_L$ [[2017 Huber et al.]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=10|p.10]]:
- **Side peaks** ($nT_L$, $n \neq 0$): the photons come from different pulses, so they cannot interfere. These peaks are the same for $\parallel$ and $\perp$.
- **Central peak, $\perp$:** half the height of the side peaks, because distinguishable photons exit through the same port half the time.
- **Central peak, $\parallel$:** suppressed by coalescence. The "dip" is the **missing area of this peak**.

For a quantum dot, each peak is a two-sided exponential set by the lifetime $T_1$. Only the coherent part ($T_2$) interferes, so it cuts a sharp dip into the centre that detector jitter smears into a flattened peak [[2010 Flagg et al.]] [[2010 - Flagg et al. - Interference of Single Photons from Two Separate Semiconductor Quantum Dots.pdf#page=4&selection=11,1,42,3&color=important|p.4]] . Keeping only early detection bins removes late, incoherent photons. In [[2017 Huber et al.]] [[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=12&selection=14,14,21,61&color=yellow|p.12]] this raised the coalescence from 0.39 to 0.63, at the cost of count rate.

![[2017 - Huber et al. - Interfacing a quantum dot with a spontaneous parametric down-conversion source.pdf#page=11&rect=68,389,529,707&color=yellow|p.11]]

---
## Continuous-Wave (CW) HOM

With no clock, photons arrive at random times, so the histogram against detection time difference $\tau$ is continuous:
- **Large $|\tau|$:** the photons are separated in time, so the rate sits at the uncorrelated background for both polarizations.
- **$\tau \to 0$, $\perp$:** each source is antibunched, so a coincidence needs one photon from each source. The rate dips to **half** the background.
- **$\tau \to 0$, $\parallel$:** photons within about one coherence time of each other coalesce, and the rate falls towards **zero** over a width of order $T_2$.

Here the detection time itself post-selects the pairs that overlapped. The visibility at $\tau = 0$ therefore depends on the **timing resolution relative to the coherence time**. For example, poorly indistinguishable photons gave a post-selected visibility of 0.97 (200 ps resolution, 150 ps coherence time) but only 0.18 without post-selection. Spectral diffusion lowers it further [[2023 Heindel]] [[2023 - Heindel - Quantum dots for photonic quantum information technology.pdf#page=54|p.54]].

![[2026 - Kim et al. - Two-photon interference between independent atomic and quantum dot single-photon sources for hybrid quantum network.pdf#page=5&rect=298,264,464,479&color=yellow|p.5]]
