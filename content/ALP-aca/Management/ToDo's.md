---
title: ToDo's
draft: false
tags:
---
 [Google Doc](https://docs.google.com/document/d/1k1V7VydBTKMHMgXEMlUlx0Te4GMagtz96uPc3YhpepM/edit?usp=sharing)
[GitHub Project](https://github.com/orgs/alp-aca/projects/2)

## Theory

- [ ] Understanding of ChiPT above 1 GeV
     - [ ] Systematic computation of $a\to 3\phi$ amplitudes for any combination of 3 pseudoscalar mesons (i.e. replacing the current expressions, which are taken from Ovchninnikov’s notebook for each individual process, by more compact expressions that are generic).
    - [ ] Check that $a \to \gamma \gamma$ is correct, using WZW.
    - [ ] Processes involving vector mesons (background fields vs HLS?)
		- [ ] 4-body decays? Check the implementation in Ovchninnikov’s notebook.
    - [ ] Baryonic processes? $a \to p \bar p \pi$ and $a \to n \bar n \pi$ are borderline in the validity range.
- [ ] Transition to pQCD regime
    - At the moment, in pQCD we only consider $a \to gg$, $a \to c \bar c$, $a -> b \bar b$. Should we also include decays to lighter quarks? And flavour violation?
	    - For example, let us imagine that, at low energy scales, the ALP couples only/mostly to down quarks. In our current implementation, the ALP would only decay in the non-perturbative regime, but it would be stable in pQCD, which doesn’t make much sense to me.
    - Including more ChiPT processes, especially those with s quarks (e.g. $a \to K K \pi$), could improve the agreement between non-pert and pQCD.
	- If we include axial-vectors via background fields, then there are some processes that are mediated by flavour-conserving vector couplings. However, in the pQCD these couplings do not enter the phenomenology. What is happening there?
- [ ] Extensions: Non-shift-symmetric, CP-violating…
- [ ] Theoretical bounds (unitarity, positivity), see [https://arxiv.org/abs/2510.13953](https://arxiv.org/abs/2510.13953)
- [ ] Stability of EW vacuum
    - Check [https://arxiv.org/abs/2506.06426](https://arxiv.org/abs/2506.06426), however note that there is a mistake in the computations, and according to several people I have talked with, this flips completely the stability criterion. Better wait till it’s solved…
- [ ] Connections to string-theory axions ???
## Pheno

- [X] Projections for bounds on long-lived ALPs in LHCb using the new reconstruction algorithm (see [https://arxiv.org/abs/2503.13092](https://arxiv.org/abs/2503.13092) and [https://arxiv.org/abs/2312.14016](https://arxiv.org/abs/2312.14016)) 
- [X] Implementing the “BC benchmarks” (BC9, BC10 and BC11) used frequently by experimentalists [https://arxiv.org/abs/1901.09966](https://arxiv.org/abs/1901.09966) 
- [ ] Beam dump experiments (do we need to run a MonteCarlo each time, or is it possible to run once and then recast?)
- [ ] Indirect probes: magnetic dipole moments [and edm’s], chromomagnetic dipole moment of the top quark.
- [ ] High-mass processes: light-by-light scattering, production in W, Z, higgs decays.
- [ ] Low-mass processes: supernovae and neutron star mergers.
- [X] Analysis of B-> K nu nu considering either new measurement of Belle (when it appears) or extend recasting done by Altmannshofer et al to account for lower values of ma (until ma=0).
- [ ] Check if all Robert’s comments are implemented or if some of them are missing.
## Program optimizations and new features

- [ ] Phase space integration routines
	- At the moment, we use a completely general integration for 3-body decays, integrating over one energy and two angular variables. However, in our case (decays of a scalar into scalars and/or summing over polarisation of vectors), it is possible to use instead integration over two Mandelstam variables (see for example the Kinematics section of PDG).
- [X] Interactive plots
- [ ] Generate citation reports: 
	- For each bibliographical reference, add a category (e.g. “Measurement”, “Running”) and a short description, and generate a TeX file.
- [ ] Matching of generic UV theories with ALP-EFT using Matchete and/or MatchmakerEFT
- [ ] Exporting ALP-EFT Lagrangians to FeynRules and UFO [I have a basic implementation that is still not uploaded, but more work would be needed]
- [ ] Connection with Pythia for decays into hadrons
	- We would need to contact someone that knows Pythia. Before summer, I did a little experiment, generating a UFO model for a light ALP (0.5 GeV) and only coupling to gluons, and running it with MadGraph using Pythia as a plug-in in the default settings. From ChiPT, I was expecting that the ALP would decay into 3 pions, but in all the events that I generated it decayed into 2 pions, which is forbidden. Clearly, there was something wrong/missing.