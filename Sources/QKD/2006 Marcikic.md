---
Authors:
  - "[[Ivan Marcikic]]"
  - "[[Antía Lamas-Linares]]"
  - "[[Christian Kurtsiefer]]"
Publication: "[[Applied Physics Letters]]"
Title: "Free-space quantum key distribution with entangled photons"
Year: "2006"
tags:
  - SPDC
  - EntanglementSource
  - QuantumInternet
---
[[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf|Free-space quantum key distribution with entangled photons]]


## Results

Polarization entanglement [[Quantum Key Distribution (QKD)]] at 630/s key rates over 1.5km distance with no extra classical overhead [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&selection=14,34,17,65&color=yellow|p.1]].

QKD protocol is entanglement based modified BB84 implemted over a free-space link. Synchronization is aided by the time correlation of [[SPDC]]  [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&selection=116,0,128,16&color=yellow|p.1]].

![[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&rect=314,36,565,256&color=yellow|p.1]]

The flying qubit is measured using passive 50/50 H/V and D/A projections [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=2&selection=56,0,117,46&color=yellow|p.2]]

Detection timestamps are recorded on both sides with timing units locked to Rb oscillator to synchronize the sorting process  [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&selection=148,10,149,56&color=yellow|p.1]] [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=2&selection=229,12,247,7&color=yellow|p.2]].

Initially, classical network time protocol locks the controllers to <100ms; then, a cross corelation between raw detection timestamps can narrow down the time resolution down to ~2us then 2ns using FFT [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=2&selection=250,13,276,53&color=yellow|p.2]].

## Arguments

Security is based on quantum mechanics instead of the classical factoring algorithm [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&selection=38,22,41,58&color=yellow|p.1]].

Unlike entanglement based type, Prepare and Send (PaS) type protocol needs overheads of the high bandwidth channel and trusted random number generator [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=1&selection=100,15,103,8&color=important|p.1]].

Classically communicate the timing information takes a lot of bandwidth but essential to efficiently deal with CW-pump source [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=2&selection=277,0,305,14&color=red|p.2]].

Coincidences beyond a accepting time difference but not too high are used to steer againt the clock drift, extending the continuous operating time [[2006 - Marcikic - Free-space quantum key distribution with entangled photons.pdf#page=2&selection=309,32,348,48&color=yellow|p.2]].