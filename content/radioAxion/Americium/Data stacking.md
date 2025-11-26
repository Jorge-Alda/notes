---
title: Data stacking
tags:
  - ALP
  - RadioAxion
  - DataAnalysis
---
Original dataset:
- Observation time $T$
- Number of samples $N$
- Sampling time $\Delta t =\frac{T}{N}$
- Sampling frequency $\Delta f = \frac{1}{N\Delta t}=\frac{1}{T}$
- DFT frequencies $f_k = \frac{k}{N\Delta t} = k \Delta f$, $k \in [-N/2, N/2]$ (for real signals, it is enough with $k \in [0, N/2]$)
- PSD $S_k = \frac{(\Delta t)^2}{T} \left|\sum_{n=0}^{N-1}a_n \exp(-2\pi i k n/N)\right|^2$


Data stacked:
- Data divided in $N_T$ subintervals, and each subinterval contains $N_S = N/N_T$ samples
- Each subinterval has duration $T_N = T/N_T$
- New sampling frequency $\Delta f_T = \frac{1}{T_N}$
- DFT frequencies $f_k = k \Delta f_T$, $k \in [0, N_S/2]$
- PSD $S_{k,l} = \frac{(\Delta t)^2}{T_N} \left|\sum_{n=0}^{N_S-1}a_{n,l} \exp(-2\pi i k n/N)\right|^2$ where $l$ is an index for the subinterval
- Stacked PSD $\bar{S}_k = \frac{1}{N_T} \sum_l S_{k,l}$

Some numbers:
$\Delta f_T = 1\,\mathrm{Hz}$, $T_N = 1\,\mathrm{s}$
$T \sim 280\,\mathrm{days}$
$N_T = T/T_N = 2.42\times 10^7$
$N_S = \frac{N}{N_T} = \frac{N T_N}{T} =\frac{T_N}{\Delta t} = 10^6$
$f_k = [0, 1\,\mathrm{Hz}, \ldots, 500\,\mathrm{kHz}]$