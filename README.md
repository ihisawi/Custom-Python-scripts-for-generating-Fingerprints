# Molecular Fingerprint Generator

This repository contains a Python-based pipeline for generating molecular fingerprints, developed as part of the study: **"Computational Studies Towards the Identification of CB2R-M1R Dual Modulators"**

The tool automates the generation of five distinct fingerprint types using **OpenBabel** and the **Chemistry Development Kit (CDK)**, facilitating reproducibility in cheminformatics workflows. [As those fingerprints are not freely available in Knime]

## Features
Generates the following molecular fingerprints from SMILES strings:
1.  **FP2** (OpenBabel)
2.  **Klekota-Roth** (CDK)
3.  **Graph Only** (CDK)
4.  **Substructure** (CDK)
5.  **Hybridization** (CDK)

## Prerequisites
To run this tool, you need:
1.  **Python 3.7+**
2.  **Java JDK 11+** (Required for CDK interaction)
    * *Linux:* `sudo apt install openjdk-11-jdk`
    * *Windows/Mac:* Install from [Adoptium](https://adoptium.net/)

## Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```

2.  Install Python dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Place your data:** Put your CSV file(s) in the same folder as the script.
    * Ensure your CSV has a column containing SMILES strings (e.g., "Canonical SMILES").

2.  **Run the script:**
    ```bash
    python fingerprint_generator.py
    ```

3.  **Results:**
    The script will automatically detect your input file and save the fingerprints in the `output/` directory, organized by fingerprint types.

Note: Sample input and output files are included in this repository (Input: MK.csv) (Output: MK-FP2.csv). You can use these files to verify that the code is running correctly and producing the expected results.

## Citation
If you utilize this resource, please cite our article:
> [Computational Studies Towards the Identification of CB2R-M1R Dual Modulators]

## License
This project is licensed under the MIT License - see the [LICENSE] file for details.
