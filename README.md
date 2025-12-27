# Molecular Fingerprint Generator

This repository contains a Python-based pipeline for generating molecular fingerprints, developed as part of the study: **"Development of a Machine Learning Model for Virtual Screening to Identify New HPK1 Inhibitors with Anticancer Activity."**

The tool automates the generation of five distinct fingerprint types using **OpenBabel** and the **Chemistry Development Kit (CDK)**, facilitating reproducibility in cheminformatics workflows.

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
    The script will automatically detect your input file and save the fingerprints in the `output/` directory, organized by fingerprint type.

## Citation
If you utilize this resource, please cite our manuscript:
> [Insert your manuscript citation here once published]
