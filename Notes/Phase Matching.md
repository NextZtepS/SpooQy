
Phase matching refers to the requirement to conserve energy and monentum at in the nonlinear interaction. We mostly discuss about three-wave (second-order nonlinearity) mixing process here but the concept applies to four-wave (third-order nonlinearity) mixing as well. The energy conservation is quite straightforward since it could be computed directly from a frequency of the photons involved.
$$ f_p = f_s + f_i $$
The momentum conservation is a bit more tricky as it involes propagation direction.
$$ \vec{k_p} = \vec{k_s} + \vec{k_i}$$
If the all the $\vec{k}$'s are pointing in the same direction, it is said to be **collinear** and generally preferred as it simplifies the collection of signal and idler photons.

There are 2 types of phase matching techniques possible

## Critial Phase Matching (CPM + [[QPM]])

In this case, we cut the crystal such that the the angle between the beam propagation and crystal's optical axis is not $0^\circ$ or $90^\circ$. Therefore, the extraordinary beam experinces some $n_{eff}$ while the ordinary beam experience $n_0$. In many cases, the engineer can use electric field to flip the domain of the crystal to create a *periodic polling*. This periodic polling addes another [[grating vector]] term in the momentum covservation condition where $\Lambda$ is the pooling period.
  ![[2007 - Fedrizzi - A wavelength-tunable fiber-coupled source of narrowband entangled photons.pdf#page=4&rect=172,574,438,609|p.4]]
The technique is called **Quasi-phasematching** (QPM) offers a flexibility in choosing almost any phasematching angles and wavelengths with *no spatial walkoff* with careful engineering and enably **type-0 SPDC** [[Fedrizzi 2007]] [[2007 - Fedrizzi - A wavelength-tunable fiber-coupled source of narrowband entangled photons.pdf#page=4&selection=144,2,168,52&color=yellow|p.4]]  [[Kim 2024]] [[2024 - Kim - Robust and bright polarization-entangled photon sources exploiting non-critical phase matching without periodic poling.pdf#page=2&selection=420,6,430,1&color=yellow|p.2]].
  
Although QPM offers great flexibility, it does have limit as the nonlinear optical coefficient $d(l)$ which has spatial dependence. This spatial dependence makes the effective coefficient $d_{eff}$ to be significantly lower [[Kim 2024]] [[2024 - Kim - Robust and bright polarization-entangled photon sources exploiting non-critical phase matching without periodic poling.pdf#page=3&selection=5,2,135,1&color=yellow|p.3]].

---
## Noncritical Phase Matching ([[NCPM]])

In this case, the phase matching conditions are simpler as we let the beams propagate along the at $0^\circ$ or $90^\circ$ to the optical axis. NCPM does not exhibit spatial walkoff thanks to its alignment with axis. The wavelength choices then are more limited and often produce photon pairs that are highly nondegenerate (very different $\lambda$). The highly non-degenerate pairs (VIS+NIR) is suitable for interacting with atomic systems (VIS) and sending in fiber (NIR). NCPM in [[KTP crystal]] offers higher temperature stability, but at higher temperature, compared to QPM because the changes in refractive indexes of the pump and signal dominates the idler [[Chin 2025]] [[2025 - Chin - Highly nondegenerate polarization-entangled photon pairs produced through noncritical phasematching in single-domain KTiOPO4.pdf#page=4&selection=1,40,65,21&color=yellow|p.4]].
  ![[2025 - Chin - Highly nondegenerate polarization-entangled photon pairs produced through noncritical phasematching in single-domain KTiOPO4.pdf#page=3&rect=314,279,575,478|2025 - Chin - Highly nondegenerate polarization-entangled photon pairs produced through noncritical phasematching in single-domain KTiOPO4, p.3]]
NCPM's idler also has a small linewidth that minimize chromatic dispersion in optical fiber. NCPM crystal is often cheaper to buy compared to QPM. However, it might be hard to find a pump laser that works with the NCPM crystal as NCPM only works at specific wavelength [[Chin 2025]] [[2025 - Chin - Highly nondegenerate polarization-entangled photon pairs produced through noncritical phasematching in single-domain KTiOPO4.pdf#page=6&selection=145,0,153,50&color=important|p.6]].

NCPM in [[LN crystal]] was shown to be tunable with temperature (150-230 C) to produce VIS 700-900 nm + NIR 1400-1700 nm pairs [[Han et al. 2026]].

![[2026 - Han et al. - Broadband tunable photon-pair generation and spectrum measurement based on noncritical lithium niobate crystals.pdf#page=4&rect=126,589,291,739&color=red|p.4]]