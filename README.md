# tess-variable-star-clustering

## Project Overview

This project investigates whether unsupervised machine learning can identify meaningful variability structure in stellar light curves obtained from the Transiting Exoplanet Survey Satellite (TESS).

Using real observational photometric data from NASA’s TESS mission, the pipeline:

* retrieves stellar light curves,
* extracts variability features,
* applies dimensionality reduction,
* and performs unsupervised clustering analysis.

The goal of the project is not direct astrophysical classification, but rather the discovery of statistical structure within stellar variability behavior using feature-based machine learning techniques.

---

## Scientific Motivation

Modern astronomical surveys generate massive volumes of time-series data that are difficult to analyze manually. Computational methods such as machine learning provide scalable approaches for identifying patterns and relationships within these datasets.

This project explores whether stars exhibiting similar variability behavior naturally cluster together in feature space without requiring labeled training data.

---

## Pipeline Structure

The computational workflow consists of:

1. Real TESS target acquisition
2. Light curve retrieval using Lightkurve
3. Data cleaning and normalization
4. Variability feature extraction
5. Lomb–Scargle periodicity analysis
6. Feature scaling
7. Principal Component Analysis (PCA)
8. KMeans clustering
9. Visualization and results export

---

## Features Extracted

The pipeline extracts several statistical and astrophysical descriptors from each light curve, including:

* Mean Flux
* Standard Deviation
* Amplitude
* RMS Variability
* Median Absolute Deviation (MAD)
* Lomb–Scargle Period
* Lomb–Scargle Power
* Slope
* Variability Index

---

## Technologies Used

* Python
* Lightkurve
* Astropy
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

---

## Example Output

The project produces:

* PCA cluster visualizations
* variability feature matrices
* clustered stellar datasets
* publication-style plots

---

## Research Context

This project was developed as an independent astroinformatics and machine learning research investigation using real TESS observational data.

---

## Running the Pipeline

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook or Python pipeline:

```bash
jupyter notebook
```

or

```bash
python pipeline.py
```

---

## License

This repository is intended for educational and research purposes.
