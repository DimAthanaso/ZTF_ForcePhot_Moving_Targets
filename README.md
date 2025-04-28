# ZTF Force Photometry for Moving Targets (Asteroids)

This repository contains the code used in the study:  
**"Spin states of X-complex asteroids in the inner main belt-I. Investigating Athor and Zita collisional families"**
Athanasopoulos, D., et al. (2024) Astronomy & Astrophysics 690 : A215.
[https://doi.org/10.1051/0004-6361/202451363]

## 📜 License
This code is distributed under the **MIT License**. See [LICENSE](LICENSE) for details.

## 📚 Citation
If you use this code in your research, please cite our work:

```bibtex
@ARTICLE{2024A&A...690A.215A,
       author = {{Athanasopoulos}, D. and {Hanu{\v{s}}}, J. and {Avdellidou}, C. and {van Belle}, G. and {Ferrero}, A. and {Bonamico}, R. and {Gazeas}, K. and {Delbo}, M. and {Rivet}, J.~P. and {Apostolovska}, G. and {Todorovi{\'c}}, N. and {Novakovic}, B. and {Bebekovska}, E.~V. and {Romanyuk}, Y. and {Bolin}, B.~T. and {Zhou}, W. and {Agrusa}, H.},
        title = "{Spin states of X-complex asteroids in the inner main belt: I. Investigating Athor and Zita collisional families}",
      journal = {\aap},
     keywords = {astronomical databases: miscellaneous, minor planets, asteroids: general, Astrophysics - Earth and Planetary Astrophysics},
         year = 2024,
        month = oct,
       volume = {690},
          eid = {A215},
        pages = {A215},
          doi = {10.1051/0004-6361/202451363},
archivePrefix = {arXiv},
       eprint = {2409.03419},
 primaryClass = {astro-ph.EP},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2024A&A...690A.215A},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```

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
