Copyright (c) 2025 Sidhharth Balakrishnan
# Visual-distraction-in-Cyclists
Analysing Visual distraction cues in Cyclists using OpenEarables
Non-Commercial License
This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/


# IMU Labeled Dataset

This directory contains labeled IMU (Inertial Measurement Unit) data collected from 20 participants across 5 sessions each. The dataset is organized for easy access and usage in time-series modeling and machine learning experiments.


---

## File Naming Convention

- Each **participant folder** is renamed using the format: `pxXX`, where `XX` is the participant number (01 to 20).
- Each **CSV file** inside represents a session and is named using the format: `pxXX_sYY.csv`, where:
  - `XX` is the participant ID
  - `YY` is the session number (01 to 05)

Example:
- `px07_s03.csv` → Data from Participant 07, Session 3

---

##  Data Format (Inside Each CSV)

Each CSV file contains time-series IMU data with the following typical columns:
- `seconds` – time in seconds sampled at 30 Hz
- `acc_x`, `acc_y`, `acc_z` – Accelerometer readings
- `gyro_x`, `gyro_y`, `gyro_z` – Gyroscope readings
- `label` – Distraction label

##  Labels

The dataset labels were generated using **video recordings** as ground truth. Each session for every participant was thoroughly reviewed and annotated based on visual cues from the recordings to ensure high labeling accuracy.

A total of **seven distinct labels** were used to classify head orientation and distraction states:

- `ST`  – Looking Straight  
- `LD`  – Looking Down  
- `NLL` – Non-distracted Looking Left  
- `NLR` – Non-distracted Looking Right  
- `DLL` – Distracted Looking Left  
- `DLR` – Distracted Looking Right  
- `TR`  – Turning Right  

