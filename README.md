# mic-pba1

This repository contains the experimental data and processed outputs associated with the study **"Investigation of Microbially Influenced Corrosion Mechanism by Acid Producing Bacteria in Marine Environments"**.

The dataset supports the analysis of **microbially influenced corrosion (MIC)** of AH36 carbon steel exposed to the acid-producing bacterium **Photobacterium A1 (PBA1)** under anaerobic artificial seawater conditions. The repository includes biofilm imaging, surface topography, electrochemical measurements, mass-loss data, nuclear magnetic resonance spectroscopy, and scanning electron microscopy with elemental analysis.

## Experimental overview

The repository compares three experimental conditions:

| Condition | Description |
|---|---|
| **Sterile static control** | Anaerobic artificial seawater without PBA1 |
| **Biotic static** | Anaerobic artificial seawater inoculated with PBA1, without nutrient replenishment |
| **Biotic flow** | Anaerobic artificial seawater inoculated with PBA1, with continuous nutrient replenishment |

The flow condition used a testing-cell volume of 75 mL continuously replenished from an external deoxygenated artificial seawater reservoir at 0.35 mL/min.

## Repository structure

```text
mic-pba1-main/
├── CFLM Analysis/
├── CLM Analysis/
│   ├── Abiotic/
│   ├── Biotic Static/
│   └── Biotic Flow/
├── EIS-PDP-LPR Analysis/
│   ├── Sample-Abiotic-Static/
│   └── Sample-Static-Biotic/
├── Mass Loss Analysis/
├── NMR Analysis/
└── SEM-EDS Analysis/
    ├── EDS Analysis/
    └── SEM Analysis/
```

## Folder descriptions

| Folder | Contents | Purpose |
|---|---|---|
| **CFLM Analysis** | Fluorescence confocal laser microscopy images, segmentation workbooks, and bacterial feature plots | Supports the analysis of PBA1 biofilm morphology and surface coverage |
| **CLM Analysis** | Confocal laser microscopy optical images, laser topography maps, 3D maps, line profiles, and localized corrosion summaries | Supports the analysis of localized corrosion depth and average localized penetration-rate estimates |
| **EIS-PDP-LPR Analysis** | Raw and processed electrochemical files for electrochemical impedance spectroscopy, potentiodynamic polarization, and linear polarization resistance | Supports time-resolved electrochemical characterization of sterile and PBA1-inoculated static systems |
| **Mass Loss Analysis** | Mass-loss corrosion-rate plots and statistical summary workbooks | Supports average uniform corrosion-rate calculations from coupon mass loss |
| **NMR Analysis** | Nuclear magnetic resonance spectrum and supporting document | Supports identification of organic acids produced by PBA1 during anaerobic fermentation |
| **SEM-EDS Analysis** | Scanning electron microscopy images, metadata text files, energy dispersive X-ray spectroscopy reports, and summary image | Supports biofilm, corrosion-product, surface morphology, and elemental characterization |

## Key processed outputs

### Biofilm morphology and fluorescence imaging

- `CFLM Analysis/CFLM-BACTERIAL-ANALYSIS.xlsx`
- `CFLM Analysis/CFLM-INFECTION-ANALYSIS.xlsx`
- `CFLM Analysis/CFLM_BACTERIA_PROPERTIES.png`
- `CFLM Analysis/CFLM_BACTERIA_AREA.png`
- `CFLM Analysis/CFLM_BACTERIA_CIRCULARITY.png`
- `CFLM Analysis/CFLM_BACTERIA_ROUNDNESS.png`

### Localized corrosion analysis

- `CLM Analysis/CLM_LOC_CORR_DEPTH.xlsx`
- `CLM Analysis/CLM_LOC_CORR_CR.xlsx`
- `CLM Analysis/CLM_LOC_CORR_DEPTH.png`
- `CLM Analysis/CLM_LOC_CORR_CR.png`
- `CLM Analysis/CLM_LOC_CORR_PROFILE.png`

Condition-specific confocal laser microscopy images and profiles are stored in:

- `CLM Analysis/Abiotic/`
- `CLM Analysis/Biotic Static/`
- `CLM Analysis/Biotic Flow/`

### Electrochemical analysis

- `EIS-PDP-LPR Analysis/EIS FITTING SUMMARY.xlsx`
- `EIS-PDP-LPR Analysis/PDP FITTING SUMMARY.xlsx`
- `EIS-PDP-LPR Analysis/EIS SPECTRA.png`
- `EIS-PDP-LPR Analysis/PDP-LPR ANALYSIS.png`

Raw and processed electrochemical files are organized by condition:

- `EIS-PDP-LPR Analysis/Sample-Abiotic-Static/`
- `EIS-PDP-LPR Analysis/Sample-Static-Biotic/`

Each condition contains files for:

- **Electrochemical impedance spectroscopy (EIS)**
- **Linear polarization resistance (LPR)**
- **Potentiodynamic polarization (PDP)**

Raw Bio-Logic `.mpr` files are provided together with extracted `.txt` files and fitting reports when available.

### Mass-loss analysis

- `Mass Loss Analysis/MLT_CR_STATS.xlsx`
- `Mass Loss Analysis/MLT_CR_STATS_OVERALL.xlsx`
- `Mass Loss Analysis/MLT_CR_A_F.png`
- `Mass Loss Analysis/MLT_CR_A_S.png`
- `Mass Loss Analysis/MLT_CR_B_F.png`
- `Mass Loss Analysis/MLT_CR_B_S.png`

### Nuclear magnetic resonance spectroscopy

- `NMR Analysis/NMR.png`
- `NMR Analysis/NMR.docx`

### Scanning electron microscopy and elemental analysis

- `SEM-EDS Analysis/SEM-EDS-Summary.png`
- `SEM-EDS Analysis/SEM Analysis/`
- `SEM-EDS Analysis/EDS Analysis/`

## File formats

| Extension | Description |
|---|---|
| `.xlsx` | Processed datasets, summary statistics, and analysis workbooks |
| `.png`, `.jpg`, `.tif` | Image outputs from microscopy, topography, and plotted analyses |
| `.txt` | Extracted electrochemical data and microscopy metadata |
| `.mpr` | Raw Bio-Logic electrochemical acquisition files |
| `.pdf` | Electrochemical fitting reports |
| `.docx` | Supporting analysis notes and reports |

## Interpretation notes

- Mass-loss data report **area-averaged uniform corrosion rates** calculated from coupon mass loss and should not be interpreted as localized penetration severity.
- Confocal laser microscopy depth measurements report **localized pit-depth metrics** and average localized penetration-rate estimates obtained by normalizing end-point pit depths by the exposure time.
- Electrochemical measurements under static conditions provide **time-resolved interfacial information**, including changes in open-circuit potential, polarization resistance, corrosion-rate estimates, and impedance response during biofilm development.
- Flow-through experiments were used for mass-loss and surface-characterization endpoints to evaluate the effect of nutrient replenishment on biofilm-associated corrosion.

## Reuse and reproducibility

The repository is intended to support transparency and reuse of the experimental dataset. Processed summary workbooks and figure outputs can be used directly to verify the reported trends. Raw electrochemical files are included for users who wish to reprocess the electrochemical measurements using Bio-Logic EC-Lab or compatible software.

## Citation

If you use this repository, please cite the associated manuscript once published:

> Messinese, E., Brenna, A., Tan Jie Hao, N. J., Ivanovich, N., Ormellese, M., and Lauro, F. M. **Investigation of Microbially Influenced Corrosion Mechanism by Acid Producing Bacteria in Marine Environments**. Manuscript under preparation.

## Contact

For questions about the dataset, please contact the corresponding author:

**Elena Messinese**  
Department of Chemistry, Materials and Chemical Engineering "Giulio Natta"  
Politecnico di Milano  
Email: elena.messinese@polimi.it
