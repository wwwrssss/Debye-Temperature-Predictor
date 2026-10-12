Debye Temperature Predictor
A standalone machine-learning application for rapid Debye-temperature prediction from crystallographic information files.
Download the latest Windows release · Example CIF · Documentation
Overview
Debye Temperature Predictor is a standalone Windows application developed for rapid estimation of the Debye temperature, Θ_D, of inorganic crystalline materials directly from crystallographic information files (.cif).
The application was developed as part of a machine-learning-assisted materials-screening workflow in which Debye temperature is used as a descriptor of lattice rigidity. The software is intended to make the trained prediction model easier to use without requiring users to install Python or run source code.
Manuscript status: The associated research article is currently under submission/review. Full bibliographic information will be added after publication.

Download
The latest compiled Windows application is available from the GitHub Releases page:
Download Debye Temperature Predictor v1.0.0
- Version: v1.0.0
- Platform: Windows
- Input: .cif
- Output: predicted Debye temperature, Θ_D (K)
No Python installation is required for the standalone Windows executable.
Software Interface

Model Performance
The Debye-temperature prediction model used in the associated manuscript achieved the following five-fold cross-validation performance:
Metric	Value
R²	0.968
MAE	28.12 K
RMSE	43.64 K


These values correspond to the model version used in the associated study.
Main Features
- Import crystallographic information files (.cif)
- Automatic processing of crystal-structure information for Debye-temperature prediction
- Rapid prediction of Debye temperature
- Graphical user interface for non-programming users
- Standalone Windows executable
- Example CIF file provided for testing
- Free for academic and non-commercial research use
Quick Start
1. Download
Open the latest release:
https://github.com/wwwrssss/Debye-Temperature-Predictor/releases/latest
Download:
Debye.Temperature.Predictor.v1.0.0.exe
2. Launch
Double-click the executable.
Because this is research software distributed as an unsigned executable, Windows may display a security warning. Please verify that the file was downloaded from this official repository before running it.
3. Import a structure
Select a valid .cif file using the file-selection button in the application.
4. Predict
Run the prediction. The application reports the predicted Debye temperature, Θ_D, in kelvin.
An example CIF file is available at:
examples/example_BaO.cif
Intended Use
This application is designed primarily for:
- rapid screening of inorganic crystalline materials;
- comparison of lattice-rigidity-related trends;
- preliminary candidate selection before more computationally intensive calculations;
- materials-discovery workflows requiring fast Debye-temperature estimates.
Important Limitations
The predicted Debye temperatures are machine-learning estimates intended for screening purposes.
They should not be considered replacements for experimental measurements, first-principles elastic calculations, phonon calculations, or other high-accuracy property calculations.
Prediction reliability may decrease for materials that are chemically or structurally far outside the training-data domain.
Citation
The associated research article is currently under submission/review.
Until the article is formally published, please cite the software repository if you use the application in academic work:
Debye Temperature Predictor, version 1.0.0.
https://github.com/wwwrssss/Debye-Temperature-Predictor

The CITATION.cff file will be updated with the final article information after publication.
Availability Statement for the Manuscript
Based on the developed Debye-temperature prediction model (R² = 0.968, MAE = 28.12 K, and RMSE = 43.64 K), a standalone application was further developed to enable rapid Θ_D estimation from crystallographic information files. The application is freely available for academic use at https://github.com/wwwrssss/Debye-Temperature-Predictor.

License and Use
The compiled application is provided free of charge for academic and non-commercial research use.
Please see the LICENSE file for details.
Version
Current release: v1.0.0
For reproducible academic use, please report the software version used in your work.
