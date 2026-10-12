# Debye Temperature Predictor

A standalone Windows application for rapid prediction of Debye temperature (Θ_D) from crystal structure files.

This application accompanies our study on machine-learning-assisted screening of structurally confined host lattices for high-concentration Eu²⁺-activated luminescent materials.

## Main features

- Import a `.cif` crystal structure file
- Automatically extract structure-related descriptors
- Predict Debye temperature (Θ_D)
- Simple graphical user interface
- No source-code installation required for end users

## Reported model performance

The Debye-temperature model used in the manuscript achieved the following five-fold cross-validation performance:

- R² = 0.968
- MAE = 28.12 K
- RMSE = 43.64 K

## Download

The Windows executable is provided in the **Releases** section of this repository.

Recommended release name:

`Debye Temperature Predictor v1.0.0`

If the executable file is smaller than GitHub's direct upload limit, it may also be placed in:

`app/Debye_Temperature_Predictor.exe`

## How to use

1. Download the latest Windows release.
2. Launch `Debye_Temperature_Predictor.exe`.
3. Click **Import CIF** or the corresponding file-selection button.
4. Select a valid `.cif` structure file.
5. Run the prediction.
6. The predicted Debye temperature will be displayed in kelvin.

An example CIF file is provided in the `examples/` folder.

## Input

Supported input:

- Crystallographic Information File (`.cif`)

The prediction tool is intended for inorganic crystalline materials.

## Output

The application reports the predicted Debye temperature:

`Θ_D (K)`

## Scope and limitations

This software is intended primarily for rapid materials screening.

Predicted values should not be interpreted as replacements for experimental measurements or high-accuracy first-principles elastic/phonon calculations.

Prediction reliability may decrease for compounds that are chemically or structurally far outside the training-data domain.

## Citation

If you use this application in academic work, please cite the associated paper:

R. Wang, Z. Leng, et al., “Machine-Learning-Assisted Multidimensional Screening of Structurally Confined Lattices toward High-Concentration Eu²⁺-Activated Dual-Mode Photoluminescence and Mechanoluminescence,” *Advanced Materials*, publication information to be updated after acceptance.

## Academic use

The application is freely available for academic and non-commercial research use.

## Repository contents

```text
Debye-Temperature-Predictor/
├── README.md
├── LICENSE
├── CITATION.cff
├── app/
│   └── PUT_YOUR_EXE_HERE.txt
├── examples/
│   └── example_BaO.cif
├── docs/
│   ├── USER_GUIDE.md
│   ├── MODEL_INFORMATION.md
│   └── RELEASE_CHECKLIST.md
└── screenshots/
    └── PUT_INTERFACE_SCREENSHOT_HERE.txt
```

## Contact

For questions regarding the application or associated research, please contact the corresponding authors of the paper.
