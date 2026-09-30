<div align="center">

<img src="assets/header.svg" width="100%" alt="Ahmed Selim - Biomedical Engineer"/>

<a href="https://github.com/ahmedselim0">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=21&pause=1100&color=00E5C3&center=true&vCenter=true&width=720&height=48&lines=Engineering+the+future+of+medicine+%F0%9F%A9%BA;Turning+biosignals+into+insights+with+ML+%F0%9F%AB%80;From+neurons+to+neural+networks+%F0%9F%A7%A0;Building+Python+apps+for+healthcare+%F0%9F%90%8D" alt="typing"/>
</a>

<img src="https://komarev.com/ghpvc/?username=ahmedselim0&label=Patients+seen&color=ef4444&style=flat-square" alt="views"/>
<img src="https://img.shields.io/github/followers/ahmedselim0?label=Followers&style=flat-square&color=3b82f6" alt="followers"/>

</div>

---

## 📋 Patient File

<table>
<tr><td><b>🧑‍⚕️ Name</b></td><td>Ahmed Selim</td></tr>
<tr><td><b>🏥 Department</b></td><td>Biomedical Engineering (student)</td></tr>
<tr><td><b>🩺 Chief complaint</b></td><td>Can't stop thinking about machine learning, biosignals and Python</td></tr>
<tr><td><b>🔬 Diagnosis</b></td><td>Chronic curiosity. Prognosis: excellent</td></tr>
<tr><td><b>💊 Current treatment</b></td><td>Building, learning, shipping</td></tr>
<tr><td><b>⚠️ Allergies</b></td><td>Bugs without stack traces</td></tr>
</table>

I bridge **healthcare technology** and **artificial intelligence**, using machine learning and software to solve biomedical problems, from physiological signals to medical data, and turning the results into usable Python apps.

---

## 🫀 Anatomy of My Interests

<div align="center">
<img src="assets/body.svg" width="100%" alt="Anatomy of my interests"/>
</div>

---

## 📟 Vital Signs

<div align="center">
<img src="assets/monitor.svg" width="100%" alt="Patient monitor"/>
</div>

Here is the kind of thing I'm learning to build: an R-peak detector that estimates heart rate from a raw ECG *(illustrative snippet)*.

```python
import numpy as np
from scipy.signal import butter, filtfilt, find_peaks

def detect_r_peaks(ecg, fs=360):
    b, a = butter(3, [0.5, 40], btype="bandpass", fs=fs)      # remove drift & noise
    clean = filtfilt(b, a, ecg)
    peaks, _ = find_peaks(clean, distance=int(0.25 * fs),      # refractory period
                          height=1.5 * np.std(clean))
    heart_rate = 60 * fs / np.diff(peaks).mean()                # bpm
    return peaks, heart_rate
```

<img src="assets/dna.svg" width="100%" alt="DNA"/>

---

## 💊 Prescription (Tech Stack)

| ℞ | Category | Tools |
|:-:|---|---|
| 1 | **Core languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| 2 | **Signal processing** | ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat-square) |
| 3 | **Machine learning** | ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) |
| 4 | **Medical imaging** | ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) |
| 5 | **Apps & backend** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |
| 6 | **Workflow** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) |

<sub>*Dosage: daily. Side effects may include excessive coding.*</sub>

---

## 🧪 Case Studies

### ✅ Completed: [SelimTours](https://github.com/ahmedselim0/selim_tours)
Full-stack travel booking platform.
**Frontend:** HTML · CSS · JavaScript &nbsp;|&nbsp; **Backend:** Node.js · Express · SQLite · JWT auth · rate limiting · email notifications
**Features:** trip catalogue, bookings, reviews, wishlist, user dashboard and admin panel

### 🧫 Upcoming Clinical Trials

| Trial | Objective | Stack | Phase |
|---|---|---|---|
| 🫀 **ECG Arrhythmia Classifier** | Detect abnormal heartbeats from ECG | SciPy · scikit-learn | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |
| 🧠 **EEG Signal Explorer** | Filter, visualise and extract features from EEG | MNE · Streamlit | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |
| 🩻 **Chest X-ray Classifier** | CNN for pneumonia detection | PyTorch · OpenCV | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |

---

## 🧠 From Neurons to Neural Networks

<div align="center">
<img src="assets/neural.svg" width="100%" alt="Neural network"/>
</div>

## 🗺 Treatment Plan

```mermaid
flowchart LR
    A["🩺 Diagnosis<br/>Python & C++"] --> B["🫀 Signals<br/>ECG · EEG filtering"]
    B --> C["🧪 Lab work<br/>Machine Learning"]
    C --> D["🧠 Therapy<br/>Deep Learning"]
    D --> E["🩻 Imaging<br/>X-ray · MRI · CT"]
    E --> F["🏥 Discharge<br/>Clinical AI apps"]
    style A fill:#3776AB,color:#fff
    style B fill:#ef4444,color:#fff
    style C fill:#F7931E,color:#fff
    style D fill:#be185d,color:#fff
    style E fill:#3b82f6,color:#fff
    style F fill:#10b981,color:#fff
```

---

## 🔬 Lab Results

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=ahmedselim0&show_icons=true&theme=tokyonight&hide_border=true&bg_color=06121c&title_color=00e5c3&icon_color=ef4444" alt="stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ahmedselim0&layout=compact&theme=tokyonight&hide_border=true&bg_color=06121c&title_color=00e5c3" alt="top languages"/>

<img src="https://streak-stats.demolab.com?user=ahmedselim0&theme=tokyonight&hide_border=true&background=06121c&ring=ef4444&fire=ef4444&currStreakLabel=00e5c3" alt="streak"/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ahmedselim0/ahmedselim0/output/snake-dark.svg"/>
  <img alt="contribution snake" src="https://raw.githubusercontent.com/ahmedselim0/ahmedselim0/output/snake.svg"/>
</picture>

</div>

---

## 📞 Book an Appointment

<div align="center">

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL_HERE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ahmedselim0)

*"The best way to predict the future of medicine is to engineer it."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ef4444,50:3b82f6,100:00e5c3&height=110&section=footer" width="100%" alt="footer"/>

</div>
