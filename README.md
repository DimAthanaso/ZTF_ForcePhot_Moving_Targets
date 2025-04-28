# ZTF Force Photometry for Moving Targets (Asteroids)

This repository contains the code used in the study:  
**"Spin states of X-complex asteroids in the inner main belt-I. Investigating Athor and Zita collisional families"**  
[https://doi.org/10.1051/0004-6361/202451363]

## 📜 License
This code is distributed under the **MIT License**. See [LICENSE](LICENSE) for details.

## 📚 Citation
If you use this code in your research, please cite our work:

```bibtex
@article{YourPublicationRef,
  title = {Spin states of X-complex asteroids in the inner main belt-I. Investigating Athor and Zita collisional families},
  author = {Your Name and Co-authors},
  journal = {Journal Name},
  year = {Year},
  doi = {DOI/URL}
}


##🚀 Usage
### 1. Prerequisites
ZTF Forced Photometry Account:
Register here.
GUI login: ztffps / dontgocrazy! (not your personal credentials).

MOST Tool:
Search for asteroid images at MOST.
Save output as MOST/<asteroid_id>_ZTF.tbl.

### 2. Workflow
▶️ Step 1: Request Data
Run Asteroid_ZTF_FP_Request.ipynb:

Input: RA/Dec, time range, your email/password.

Status checks: FP Requests Portal (updates hourly).

💾 Step 2: Save Results
After email confirmation, save submission history as ForcedPhot/<asteroid_id>_ZTF_FP.txt.

Wait 1 hour for full status.

🔧 Step 3: Process Data
Run ZTF_photometry.ipynb to:

Parse photometry data.

Handle procstatus codes (see below).

📊 Step 4: Lightcurves
Calibrate fluxes (forcediffimflux).

Use thresholds: SNT=3 (non-detections), SNU=5 (upper limits).

## 📧 Contact
For questions, contact: dimathanaso@phys.uoa.gr
