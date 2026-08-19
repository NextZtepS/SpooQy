#Source

# Overview

An entanglement source is a device that prepares a pair of photons in a [[bipartite entanglement|maximally entangled state]], most commonly a [[Bell state]]. The two dominant physical processes used to generate photon pairs are:

- **[[SPDC]]** (Spontaneous Parametric Down Conversion) — the most mature and widely deployed technique, based on a second-order nonlinear ($\chi^{(2)}$) process in birefringent crystals such as [[ppKTP crystal|ppKTP]], BBO, and lithium niobate. See [[Anwar 2021]] for a comprehensive review of SPDC-based source designs.
- **[[SFWM]]** (Spontaneous Four-Wave Mixing) — based on a third-order ($\chi^{(3)}$) process, commonly implemented in optical fibers or silicon waveguides. *To be studied later.*
- **[[Quantum Dots]]** — based on the [[biexcitons]] cascade radiative decays. See [[Heindel 2023]] for detailed description.

---

# [[SPDC]]
## Common Source Designs

Many entanglement source geometries have been developed around the SPDC process, differing in how they create the two coherent paths needed to produce a superposition state. The most widely used designs include:

- **Sagnac interferometer** — pump travels clockwise and counter-clockwise in a loop through a single crystal, creating both $\ket{HH}$ and $\ket{VV}$ contributions. High stability due to common-path geometry.
- **Double-pass / back-reflection** — pump passes through the crystal twice. Requires careful alignment for phase stability.
- **Two-crystal crossed configuration** — two crystals with orthogonal optical axes placed in series; each generates one polarization component.
- **Linear beam-displacement interferometer** — pump is split into two spatially separated beams by a birefringent walk-off crystal; both beams pass through a single crystal along two distinct paths, then recombine. Used by the SpooQy group — see below [[Lohrmann 2019]].

---

## Linear Beam Displacement Interferometer

![[2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals.pdf#page=13&rect=46,128,284,187|2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals, p.13]]

### Design Principle

The source is built around a **single [[ppKTP crystal|PPKTP crystal]]** (10 mm long, poling period 3.425 µm) operated in **Type-0 SPDC** ($\ket{V} \rightarrow \ket{VV}$). A diagonally polarized 405 nm pump beam enters a birefringent **BBO crystal** (13 mm, cut-angle 45°), which spatially separates the $\ket{H}$ and $\ket{V}$ polarization components via walk-off, creating two parallel pump beams displaced by ~1 mm.

The $\ket{H}$ component is rotated to $\ket{V}$ by a **half-wave plate (HWP)**, so both beams enter the PPKTP crystal as $\ket{V}$-polarized pump photons. Each path independently undergoes Type-0 SPDC, generating $\ket{VV}$ photon pairs. After the crystal, one beam's polarization is rotated from $\ket{VV}$ to $\ket{HH}$ by a second HWP. A second BBO crystal (13.76 mm) then recombines the two beams, producing the entangled state:

$$\ket{\Phi^+} = \frac{1}{\sqrt{2}}\left(\ket{HH} + e^{i\phi}\ket{VV}\right)$$
[[Lohrmann 2019]] [[2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf#page=1|page 1]].


> [!tip] Key advantage
> The entire interferometer is spanned by the walk-off crystals — the two paths are defined by the birefringent displacement, not by mirror alignment. This makes the interferometer **self-stable** and **alignment-free**, lending itself naturally to compact and robust deployments (e.g., space applications).

### Phase Compensation

Because the broadband pump introduces wavelength-dependent phase shifts in the birefringent components, **pre- and post-compensation crystals** (YVO₄, ~0.97 mm) are inserted in the beam path to cancel phase errors across the broad SPDC emission spectrum. This is the key step that allows high-quality entanglement to be maintained without narrow-band spectral filtering [[Lohrmann 2019]] [[2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf#page=2|page 2]].

### Pump

The source was demonstrated with two pump configurations:

| Pump | Linewidth | Pair rate | Visibility (H/V) | Visibility (D/A) |
|---|---|---|---|---|
| Narrowband laser diode | < 160 MHz | 1.2 Mpairs/s/mW | 99.2 ± 0.2% | 98.4 ± 0.2% |
| Free-running (broadband) laser diode | ~0.5 nm (~THz) | 0.56 Mpairs/s/mW | 99.0 ± 0.2% | 96.4 ± 0.4% |

The free-running configuration achieves an **average intrinsic visibility of 97.7%** across a 100 nm spectral emission range (750–870 nm) [[Lohrmann 2019]] [[2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf#page=3|page 3]].

---

## Quality of Entanglement

> [!note] Key Results (Lohrmann 2019)
> - **Narrowband pump**: H/V visibility = **99.2 ± 0.2%**, D/A visibility = **98.4 ± 0.2%**, achieved across the full SPDC spectral range from 780 nm to 842 nm.
> - **Broadband pump**: average visibility = **97.7%** over ~100 nm bandwidth, corresponding to an intrinsic quantum bit error rate (QBER) of ~1% — suitable for quantum key distribution.
> - **Pair-to-singles ratio**: 21–22% (an estimate of collection efficiency into single-mode fiber) [[2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf#page=3|page 3]].

The slight reduction in D/A visibility for the broadband pump is attributed to non-ideal compensation crystal lengths (manufacturing tolerance), not a fundamental limitation of the design.

### Pathway to High Rates

A primary motivation of the design is to exploit the high output power available from free-running laser diodes (up to 1 W at 405 nm). The authors project that combining this source with **wavelength-multiplexed, high-speed single-photon detectors** could enable observation of **~10 billion entangled pairs per second** in a single spatial mode [[Lohrmann 2019]] [[2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf#page=4|page 4]].

---
# [[SFWM]]

---

# [[Quantum Dots]]

---
# See Also

- [[SPDC]] — the underlying photon-pair generation process
- [[ppKTP crystal]] — the nonlinear crystal used in this source
- [[bipartite entanglement]] — the target quantum state
- [[Bell state]] — the specific maximally entangled states prepared
