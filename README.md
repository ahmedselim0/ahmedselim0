<div align="center">

<img src="assets/header.svg" width="100%" alt="Ahmed Selim - Biomedical Engineer"/>

<a href="https://github.com/ahmedselim0">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=21&pause=1100&color=00E5C3&center=true&vCenter=true&width=720&height=48&lines=Engineering+the+future+of+medicine+%F0%9F%A9%BA;Turning+biosignals+into+insights+%F0%9F%AB%80;Where+engineering+meets+medicine+%F0%9F%A7%A0;Building+Python+apps+for+healthcare+%F0%9F%90%8D" alt="typing"/>
</a>

<img src="https://komarev.com/ghpvc/?username=ahmedselim0&label=Patients+seen&color=ef4444&style=flat-square" alt="views"/>
<img src="https://img.shields.io/github/followers/ahmedselim0?label=Followers&style=flat-square&color=3b82f6" alt="followers"/>

</div>

---

## 📋 Patient File

<table>
<tr><td><b>🧑‍⚕️ Name</b></td><td>Ahmed Selim</td></tr>
<tr><td><b>🏥 Department</b></td><td>Biomedical Engineering (student)</td></tr>
<tr><td><b>🩺 Chief complaint</b></td><td>Can't stop thinking about biosignals, medical devices and Python</td></tr>
<tr><td><b>🔬 Diagnosis</b></td><td>Chronic curiosity. Prognosis: excellent</td></tr>
<tr><td><b>💊 Current treatment</b></td><td>Building, learning, shipping</td></tr>
<tr><td><b>⚠️ Allergies</b></td><td>Bugs without stack traces</td></tr>
</table>

I bridge **healthcare technology** and **software engineering**, working on biomedical problems from physiological signals to medical data and turning the results into usable Python apps.

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
| 3 | **Medical imaging** | ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) |
| 4 | **Apps & backend** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |
| 5 | **Workflow** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) |

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
| 🫀 **ECG Analyzer** | R-peak detection and heart-rate variability from ECG | SciPy · NumPy | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |
| 🧠 **EEG Signal Explorer** | Filter, visualise and extract band-power features from EEG | MNE · Streamlit | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |
| 🩻 **Chest X-ray Viewer** | Image enhancement and measurement tools | OpenCV · Streamlit | ![](https://img.shields.io/badge/Phase-Planning-yellow?style=flat-square) |

---
