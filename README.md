# 🫀 ECG Signal Conditioning Circuit

##  Project Overview
This project demonstrates the design and simulation of an **ECG Signal Conditioning Circuit** using **Multisim**.  
The goal is to amplify extremely weak ECG signals (in microvolts), remove noise and unwanted frequencies, and produce a **clean, stable output signal** suitable for display and digital processing.

---

##  Objectives
- Amplify microvolt-level ECG signals into millivolt-level signals  
- Remove common noise and interference  
- Filter out unwanted low and high frequencies  
- Produce a smooth, readable ECG output

---

##  Circuit Description

The circuit consists of the following stages:

### 1️⃣ Input Amplification  
Two op-amp stages (U1 and U2) provide initial amplification and signal stabilization.

### 2️⃣ Differential Amplifier  
Op-amp U3 amplifies only the **difference** between the two input signals and rejects common-mode noise such as 50/60 Hz interference.

### 3️⃣ Filtering Stage  
- **C1 & R8** remove DC offset and very low-frequency noise (baseline drift).  
- **C2 & R9** remove high-frequency noise and smooth the signal.

### 4️⃣ Final Amplification  
Op-amp U4 amplifies the filtered signal to a usable level for output.

---

##  Signal Behavior

| Stage | Signal Level |
|------|--------------|
| Input ECG | 10–100 µV |
| After amplification | ~30–50 mV |
| Output | Clean, stable ECG signal |

**Frequency Handling:**
- Preserves ECG band (0.5–100 Hz)
- Removes baseline drift (<0.5 Hz)
- Suppresses high-frequency noise (>100 Hz)

---

## 🛠 Tools Used
- **NI Multisim** – Circuit design and simulation
- **Operational Amplifiers**
- **Resistors, Capacitors**
- **Virtual Oscilloscope & Signal Sources**

---

## 📂 Repository Contents
- `ECG_Circuit.ms14` – Multisim project file  
- `Presentation.pdf` – Project presentation  
- `Report.pdf` – Detailed project report  
- `README.md` – Project documentation  

---

##  Results
The circuit successfully amplifies weak ECG signals and significantly reduces noise, producing a stable and clean waveform suitable for biomedical analysis.

---

## 👤 Author
**Dua Kashif**

---

##  License
This project is for academic and educational purposes.
