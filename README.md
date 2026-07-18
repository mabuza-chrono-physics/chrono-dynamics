# Chrono Dynamics: Data Verification Pipelines

Welcome to the official open-source code verification repository for **Chrono Dynamics**—a phenomenological framework for history-dependent gravitational anomalies authored by **Mduduzi Mishack Mabuza** (University of South Africa).

This repository hosts the live data validation and statistical calculation pipelines referenced in the core manuscript. These pipelines allow independent researchers to verify the empirical consistency of the model.

## 📊 Available Validation Scripts

1. **Precision Solar System Constraints (`solar_system.py`)**
   * *Purpose:* Verifies the suppression of History Depth ($D \ll 10^{-6}$) in high-velocity local environments to recover standard General Relativity.
   * *Data Metric:* Compares calculated parameters against NASA Cassini Spacecraft radio tracking telemetry bounds.

2. **Null Gravitational Wave Dipole Radiation (`gwosc_strain.py`)**
   * *Purpose:* Confirms isotropic field symmetric metric modulations suppress asymmetric radiative leakage at the 1PN order ($E_{\text{dipole}} < 10^{-15}$).
   * *Data Metric:* Bound checks parameters against the LIGO-Virgo-KAGRA Gravitational Wave Open Science Center strain series (Event GW170817).

3. **Strong Lensing Mass Profiles (`slacs_lensing.py`)**
   * *Purpose:* Fits early-type elliptical galaxy mass profiles to constrain and lock the global history parameter space ($\gamma T$).
   * *Data Metric:* Optimization models utilizing the Sloan Lens ACS (SLACS) Survey baseline.

4. **Cluster Age Relaxation Mapping (`cluster_age.py`)**
   * *Purpose:* Executes the Pearson linear correlation test mapping cluster mass discrepancies against X-ray structural relaxation proxies ($r = 0.41, p = 0.001$).
   * *Data Metric:* Evaluation pipeline tracking the $D^{1/2}$ scaling law across the 62-cluster core sample extracted from Chandra X-ray and Hubble CLASH archives.

## ⚙️ Execution Requirements

To run these pipelines locally, clone this repository and install the standard scientific Python stack:

```bash
git clone https://github.com
cd chrono-dynamics
pip install numpy scipy
python solar_system.py
```

## 📄 Contact & Citation
If you utilize this framework or its data verification pipelines in your independent research, please cite the core manuscript. For mathematical inquiries or project collaboration, contact **14689561@mylife.unisa.ac.za**.
