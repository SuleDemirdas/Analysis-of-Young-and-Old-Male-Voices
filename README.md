# Analysis-of-Young-and-Old-Male-Voices

This project aims to classify male voices into young and old categories using digital signal processing techniques. The primary methods employed include spectrum analysis, pitch calculation, IIR filter design, power calculation, and Fourier transform.

## Abstract

This project utilizes digital signal processing techniques to classify male voices as young or old. Key techniques include spectrum analysis, fundamental frequency calculation, IIR filter design, power calculation, and Fourier transform.

### Key Methods and Steps:

1. **Loading and Normalizing Audio Files:** Audio files from different age groups are collected, converted into a suitable format for digital processing, and normalized.
2. **Frequency Domain Analysis:** Using Fast Fourier Transform (FFT) to obtain the frequency spectrum of the audio signals.
3. **Filtering:** Applying digital filters (e.g., low-pass, high-pass, band-pass) to reduce noise and emphasize certain frequency bands.
4. **Power Analysis:** Calculating the power spectrum of the audio signals to determine energy distribution across frequency components.
5. **Pitch Calculation:** Determining the fundamental frequency (pitch) by identifying the frequency component with the highest magnitude in the frequency spectrum.

## Repository Contents

- **/audio_samples/**: Contains the audio files used in the project for analysis.
- **/filter/**: Contains the designed IIR Butterworth filter in `.mat` format.
- **/codes/**: Contains a Jupyter notebook that integrates all steps of the analysis and a filter file for butterworth IIR filter.
  - `voice_analysis.ipynb`: Main notebook that includes loading and normalizing audio files, FFT and frequency spectrum calculation, filtering, power calculation, and pitch analysis.
  - `bandpassX2.mat`: Butterworth IIR filter designed by using pydfa library for filtering desired frequencies.
- **report/**: Contains the full project report in PDF format, detailing the methodology, analysis, results, and conclusions.
