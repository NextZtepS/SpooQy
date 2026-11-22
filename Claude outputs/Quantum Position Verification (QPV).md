#QPV

## Definition

> [!note] Definition
> **Quantum position verification (QPV)**: trusted verifiers $V_0, V_1$ certify that an untrusted prover $P$ sits at a claimed position by sending challenges at light speed and checking both the **answers** and the **round-trip timing**. Security combines [[No-cloning theorem|no-cloning]] with the relativistic **no-signalling** bound. QPV is the building block of position-based quantum cryptography (authentication, key exchange, "spacetime seals").

## Core ideas

- **Classical PV is impossible.** Colluding attackers copy the classical challenges and answer from both sides (Chandran et al. 2009). Quantum challenges cannot be copied, which blocks this attack.
- **Quantum PV is breakable in general.** Attackers who pre-share enough entanglement can break any protocol using [[Instantaneous non-local computation]] (Buhrman et al. 2014; Beigi & König 2011). In practice security means **"secure unless attackers share ≥ N qubits of entanglement"**, so good protocols make N large.
- **Making N large with classical bits.** In **f-BB84 / f-routing**, the verifiers send one qubit plus $n$-bit classical strings $x, y$, and the basis is $f(x,y)$. The entanglement an attack needs grows with $n$, so the honest prover needs only a single qubit while the attackers need many [[2022 Bluhm]].
- **Loss is the main barrier.** If verifiers simply discard rounds where the prover reports "no photon", attackers can guess, discard their bad rounds and pass. A protocol is **fully loss-tolerant** only if this strategy gives no advantage [[2022 Allerstorfer]], [[2026 Allerstorfer]].
- **Slow quantum, fast classical.** Light in fiber travels at ≈ 2c/3, slower than radio or hollow-core fiber. Protocols stay secure if the qubit arrives early (or slowly) and the fast classical bits trigger the measurement [[2023 Escolà-Farràs]].

## Major protocols

| Protocol / idea                                  | Key point                                                                                                                                                               | Source                                       |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| QPV-BB84 (quantum tagging)                       | One BB84 qubit from $V_0$, basis bit from $V_1$. Broken by attackers sharing a single EPR pair; the reference point for later protocols                                 | Kent, Munro & Spiller 2011                   |
| Single-qubit-state protocols, practical security | Analysis of protocols where the verifiers prepare and send single-qubit states                                                                                          | [[2021 Das]]                                 |
| Error-robust QPV / loss in attacks               | Error thresholds, and why naive loss handling fails                                                                                                                     | [[2022 Allerstorfer]], [[2026 Allerstorfer]] |
| **f-BB84 / f-routing**                           | Classical input size sets the attackers' entanglement cost                                                                                                              | [[2022 Bluhm]]                               |
| Single-qubit loss-tolerant                       | Secure against entangled attackers under moderate loss; qubit may travel arbitrarily slowly                                                                             | [[2023 Escolà-Farràs]]                       |
| Secret-tag QPV                                   | Tag holds a classical key replenished by [[QKD]]; the verification step needs no quantum communication; tolerates loss and errors                                       | [[2023 Cowperthwaite]]                       |
| **Commitment (c-QPV-BB84)**                      | Photon-presence detection, then a small delay and a commitment. Only the **prover-lab loss** matters, not channel loss                                                  | [[2025 Allerstorfer et al.]]                 |
| Multi-basis, loss-independent prep               | Verifier state preparation independent of channel loss; tighter SDP bounds; exposes hidden assumptions in earlier proofs. Theory for the [[2026 Kon et al.]] experiment | [[2026 Kon]]                                 |
| Bell-test QPV (device-independent)               | Security from a loophole-free Bell test only, with no trust in the hardware                                                                                             | [[2026 Kavuri et al.]]                       |

> [!tip] Other branches (not yet in vault)
> - **Weak coherent pulses and decoy states**: Qi & Siopsis 2015; Lim et al., PRA 94, 032315 (2016).
> - **Continuous-variable QPV**: Allerstorfer et al. 2023 (arXiv:2308.04166); Escolà-Farràs et al., PRA 110, 062605 (2024).
> - **Classical-verifier PV**, where the prover has a quantum computer and the verifiers are classical: Liu, Liu & Qian 2022; Kaleoglu et al. 2026; Kon, Kaleoglu & Chakraborty 2026 (arXiv:2609.38441).

## Experiments

| Work                                          | Platform                                                                                                                                                                                                                   | Headline result                                                                                                                     | Security model                                                                                                                            |
| --------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| [[2025 Kanneworff et al.]] (Leiden)           | [[Quantum Dots\|QD]]–micropillar [[Optical Cavities\|cavity]] single photons, demultiplexed by a fast optical switch; prover does [[Hong-Ou-Mandel (HOM)\|HOM]] at a BS plus 2 BS and 4 detectors (loss-resilient readout) | First lab steps toward QPV with true single photons; "towards", not a full secure run                                               | Lab proof of principle                                                                                                                    |
| [[2026 Kavuri et al.]] (NIST, *Nature*)       | Polarization-entangled photons; one photon delayed in a local fiber loop, the other sent to the prover; fast random challenge bits; [[SNSPD]]s                                                                             | **First complete device-independent QPV.** 1D localization **2.47(2)×** smaller than the best (non-remote) classical protocol       | Loophole-free Bell test; adversaries weakly entangled before each trial                                                                   |
| [[2026 Fan-Yuan et al.]] (USTC, *Nat. Phys.*) | Phase-randomized **weak coherent states**; ultra-low-loss fiber for the quantum channel; classical bits by DWDM on–off keying over **hollow-core fiber**; hardware lookup table for $f(x,y)$                               | Verifiers **2 km** apart, position verified to **< 75 m**                                                                           | Information-theoretic, f-type protocol with finite-size bounds; bounded attacker entanglement                                             |
| [[2026 Kon et al.]] (JPMorganChase + Qunnect) | ⁸⁵Rb four-wave-mixing [[Entanglement Sources\|entanglement source]]; commercial off-the-shelf components; only one verifier needs quantum hardware                                                                         | **Loss-tolerant QPV, security independent of channel loss**; certification in 22 min net data; projected to > 100 km with ULL fiber | Finite-size security vs. quantum-polynomial-time entangled adversaries in the quantum random-oracle model, against a restricted adversary |

## Practical challenges (experiment ⇄ theory)

- **Loss**: channel loss versus prover-lab loss; see the commitment and loss-independent schemes above.
- **Timing / safety radius**: the prover's processing time (switches, Pockels cells, detector jitter) enlarges the region that can be certified. This is often neglected in theory [[2026 Kanneworff]].
- **Classical channel speed**: protocols only benefit from large $n$ if those bits travel at near-$c$ (hollow-core fiber, free space) [[2026 Fan-Yuan et al.]].
- **Source and detector imperfections**: multiphoton components (weak coherent states lead to decoy states), photon [[Indistinguishability|indistinguishability]] for HOM-based readout, and polarization drift in fiber [[2026 Kanneworff]].
- **Trust in devices**: device-independent QPV removes it, at the cost of loophole-free Bell-test efficiency requirements [[2026 Kavuri et al.]].

## Further reading

- [[2026 Kanneworff]]: PhD thesis. Ch. 2 gives an overview of protocols and attacks; later chapters cover polarization stability and QD photon indistinguishability.
