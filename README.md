# Digital Signal Processing (KI/PZS) – Seminar Projects

This repository contains two seminar assignments completed within the course **Digital Signal Processing (KI/PZS)**.

The work focuses on biomedical and acoustic signal processing, feature extraction, correlation analysis, and machine learning classification.

---

# 📘 Seminar Assignment I

## 1️⃣ Heart Rate Estimation from ECG Signal

### Objective
To detect R-peaks in ECG signals and compute heart rate (BPM).

### Methods
- ECG signal loading using **WFDB**
- Z-score normalization
- R-peak detection using `scipy.signal.find_peaks`
- RR interval computation
- BPM calculation
- Evaluation against MIT-BIH reference annotations
- Accuracy analysis across multiple patients

### Results
- Average detection accuracy: **~86%**
- Accuracy range: **72% – 99%**
- Performance depends strongly on signal quality
- The algorithm is not fully stable for precise medical-grade HR estimation

---

## 2️⃣ Correlation of Physiological Signals (ECG, ABP, ICP)

### Objective
To analyze relationships between:
- ECG (Electrocardiogram)
- ABP (Arterial Blood Pressure)
- ICP (Intracranial Pressure)

### Methods
- Preprocessing:
  - NaN interpolation
  - Detrending
  - Mean centering
  - Optional resampling
- Pearson correlation
- Lagged cross-correlation
- Detection of maximum correlation and time lag
- Multi-patient correlation analysis
- Heatmap visualization of ABP cross-patient similarity

### Clinical Context
In patients with traumatic brain injury (TBI), the relationship between ABP and ICP provides diagnostic insight into:
- Cerebral autoregulation
- Intracranial compliance
- Hemodynamic response delays

Detected time lags provide insight into delayed physiological responses.

---

# 📙 Seminar Assignment II

## 🎤 Voice Signal Classification

### Objective
To classify voice recordings into:
- Healthy
- Pathological

And further distinguish between:
- Hyperkinetic dysphonia
- Hypokinetic dysphonia
- Reflux laryngitis

---

## 🔎 Feature Extraction

### Acoustic Features
- Jitter (%)
- Shimmer (%)
- Cepstral Peak Prominence (CPP)

### Spectral Features
- Energy distribution in frequency bands:
  - Low (≤800 Hz)
  - Mid (800–2500 Hz)
  - High (>2500 Hz)

---

## 🤖 Machine Learning Models

### Binary Classification (Healthy vs Pathological)
- Random Forest classifier
- Accuracy achieved: **93%**

### Multi-Class Pathology Classification
- k-Nearest Neighbors (k-NN)
- 10-fold cross-validation
- Mean accuracy: **~49%**
- Random baseline: 33%

The results indicate:
- Reliable pathological detection
- Limited performance for specific pathology differentiation
- Need for more advanced models for higher accuracy

---

# 🛠 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- WFDB
- Scikit-learn
- Random Forest
- k-NN
- FFT / Cepstral analysis

---

# 📊 Key Concepts Applied

- Signal preprocessing
- Peak detection
- Time-series correlation
- Cross-correlation and lag analysis
- Spectral analysis (FFT)
- Cepstrum analysis
- Feature engineering
- Supervised machine learning
- Cross-validation

---

# 📂 Project Structure

