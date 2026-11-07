---
Authors:
  - "[[Haifei Wang]]"
  - "[[Rui Qu]]"
  - "[[Zhengning Yang]]"
  - "[[Xiaodan Lyu]]"
  - "[[Haotao Zhu]]"
  - "[[Zitong Xu]]"
  - "[[Lianzhen Cao]]"
  - "[[Joel Yang]]"
  - "[[Otfried Gühne]]"
  - "[[Weibo Gao]]"
Publication: "[[arXiv]]"
Title: Experimental High-Dimensional Quantum Overlapping Tomography
Year: "2026"
tags:
  - Tomography
---
[[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf|Experimental High-Dimensional Quantum Overlapping Tomography]]


[[Quantum Overlapping Tomopography (QOT)]] is an efficient method to extract reduced density matrices (marginals) of the system rather than the entire system [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=1&selection=137,0,161,30&color=note|p.1]]. 

## Arguments

> ([[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=1&selection=197,0,206,34&color=important|p.1]])
> In particular, recent work demonstrated that the optimal scheme of QOT can be formulated using graph-theoretic constructions and covering arrays [44–46], yielding a further reduction in the number of measurements [47], and allowing for a generalization to fermionic systems [48]. However, a general high-dimensional formulation of QOT and its experimental realization remain unexplored.


## Results

> ([[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=1&selection=75,0,95,83&color=yellow|p.1]])
> We experimentally realize it on a photonic four-party entangled state in a 4 × 4 × 2 × 2 system. Using measurements in mutually unbiased bases, we reconstruct all six two-body marginals with only 25 projective measurement settings, compared with 94 and 225 settings for independent tomography of all two-body reduced states and full state tomography, respectively. 

## Summary

### Theory: QOT as a graph-covering problem

Each party of dimension $d_i$ gets $d_i+1$ vertices, one per [[Mutually Unbiased Bases (MUB)]] setting. Edges connect every pair of vertices from different parties, giving the complete multipartite graph $K_{d_1+1,\dots,d_n+1}$. A global measurement setting (one basis per party) is a clique. Reconstructing all two-body marginals means covering every edge with the fewest cliques [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=2|p.2]].

- Example: 3 qutrits ($K_{4,4,4}$) need 16 settings instead of $3 \times 16 = 48$ for separate tomography of each pair.
- For $k$-body marginals this generalizes to a covering array with alphabet $v = d+1$. It is the same framework as optimal Pauli QOT, with only the alphabet changed (Pauli: $v=3$) [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=9|p.9]].
- Scaling: $(d+1)^k\, O(\log n)$ settings, versus $(d+1)^k \binom{n}{k}$ for measuring each marginal separately. The cost in party number drops from polynomial to logarithmic [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=9|p.9]].
- Assumes prime-power $d$ so that complete MUB sets exist.

### Experimental setup

Target state with local dimensions $(4,4,2,2)$ (two ququarts, two qubits) [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=2|p.2]]:
$$\ket{\Lambda} = \tfrac{1}{2}\left(\ket{0011} + \ket{1100} + \ket{2211} + \ket{3300}\right)$$

- Pump: 390 nm fs pulses (80 MHz, 230 mW) on two sandwich BBO–HWP–BBO crystals, giving two polarization Bell pairs $\ket{\Psi^+}$ at 780 nm via [[SPDC]]. YVO$_4$ crystals compensate spatial and temporal walk-off, and 3 nm filters remove frequency correlations [[2026 - Wang et al. - Experimental High-Dimensional Quantum Overlapping Tomography.pdf#page=3|p.3]].
- The two pairs interfere on a PBS. Beam displacers (1.3 mm offset) add a path DOF, so each ququart is a hybrid path–polarization encoding: $\ket{H_u}, \ket{H_l}, \ket{V_u}, \ket{V_l} \to \ket{0}, \ket{1}, \ket{2}, \ket{3}$. The state is post-selected on four-fold coincidences.
- Detection: BD + waveplate + PBS modules project onto MUB settings, with SPADs and a TCSPC module.
- Performance: 0.8 Hz four-fold rate, visibility 0.893, global fidelity 0.809.
- QOT: 25 settings from clique-covering $K_{5,5,3,3}$, 600 s each. These reconstruct all six two-body marginals (MLE) with average fidelity 0.876. For comparison, separate tomography of each marginal needs 94 settings and full tomography needs 225.


