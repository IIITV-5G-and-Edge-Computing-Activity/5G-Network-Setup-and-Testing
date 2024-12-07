# 5G Network Simulation and Resource Allocation Optimization Using Machine Learning
---
## Mentor
Bhupendra Kumar

## Team Members
Mamindla Sathvika: 202151084@iiitvadodara.ac.in
Akash Maurya: 202151013@iiitvadodara.ac.in

---
## Table of Contents
1. [Project Overview](#project-overview)
2. [Objectives](#objectives)
3. [System Architecture](#system-architecture)
4. [Features](#features)
5. [Installation](#installation)
6. [Configurations](#configurations)
7. [Machine Learning Approach](#machine-learning-approach)
8. [Results and Analysis](#results-and-analysis)
9. [Troubleshooting and Errors](#troubleshooting-and-errors)
10. [Contributors](#contributors)
11. [Video Drive Link](#Video)

---

## Project Overview
This project involves building a 5G testbed using open-source platforms like *Open5GS, **Free5GC, and **UERANSIM, alongside implementing **Machine Learning (ML)* models to optimize resource allocation. The project aims to simulate real-world 5G network scenarios and apply ML techniques to enhance bandwidth usage, reduce latency, and improve resource efficiency.

---

## Video
https://drive.google.com/drive/folders/1rS93xvHYyijNT6-3-vuyck3b1cC-rKhO?usp=sharing

---

## Objectives
1. To establish a fully functional 5G standalone (SA) core network using *Open5GS* and *Free5GC*.
2. To simulate radio access and user equipment (UE) using *UERANSIM*.
3. To analyze network performance metrics such as latency, signal strength, and bandwidth usage.
4. To implement and compare *Linear Regression, **Polynomial Regression, and **XGBoost* for resource allocation optimization.
5. To address and document troubleshooting and errors encountered during implementation.

---

## System Architecture
The system architecture is composed of:
- *5G Core Network:* Implemented using *Open5GS* and *Free5GC*, including AMF, SMF, NRF, UDM, and AUSF.
- *Radio Access Network:* Simulated using *UERANSIM*, creating virtual gNodeB and UE instances.
- *Database:* MongoDB is used to store subscriber information (IMSI, keys, etc.).
- *Machine Learning Component:* Python-based ML models (Linear Regression, Polynomial Regression, and XGBoost) are used to optimize resource allocation.

---

## Features
- Simulation of real-world 5G core network and radio access using open-source tools.
- UE registration, PDU session management, and network slice configuration.
- Detailed resource allocation optimization using ML models.
- Comprehensive troubleshooting and error documentation.

---

## Installation
### Prerequisites
- *Operating System:* Ubuntu 20.04 or later.
- *Dependencies:* MongoDB, Python 3.8+, GCC, CMake, SCTP libraries.
- *Tools:* Open5GS, Free5GC, UERANSIM.

---

Go through the 2 PDFs uploaded for detailed installation steps for Open5gs and Free5gs.
Download the IPYNB notebook to run the ML complete end to end Resource Allocation in 5G Project

---

## Machine Learning Approach
The project utilized three models to optimize resource allocation within the 5G network:

1. *Linear Regression*: 
   - Used to establish baseline predictions.
   - Performance: R² = 0.19

2. *Polynomial Regression*:
   - Captures non-linear relationships in network parameters.
   - Performance: R² = 0.59

3. *XGBoost*:
   - Final and most effective model.
   - Achieved R² = 0.71

### Dataset Features:
The dataset included the following key metrics:
- *Timestamp*: Time of metric recording.
- *Signal Strength (dBm)*: Measured power level at the receiver.
- *Latency (ms)*: Round-trip time between UE and the server.
- *Bandwidth Usage (Mbps)*: Data transmission rate.
- *Active Users*: Number of concurrent users.

---

## Results and Analysis
1. Successfully set up *Open5GS, **Free5GC, and **UERANSIM* for emulating the 5G core and radio access networks.
2. Achievements in ML-based resource allocation optimization:
   - Linear Regression R²: 0.19
   - Polynomial Regression R²: 0.59
   - XGBoost R²: 0.71
3. Detailed error analysis and troubleshooting of issues in Open5gs and Free5gs such as:
   - NAS registration errors ([SEMANTICALLY_INCORRECT_MESSAGE]).
   - SCTP connection issues.
   - RRC connection drops.

---

## Troubleshooting and Errors
### Common Issues and Fixes:
1. *SCTP Connection Issues*:
   - Resolved by installing libsctp-dev and ensuring proper SCTP endpoint configuration.
2. *NAS Registration Failures*:
   - Corrected IMSI and key values in MongoDB subscriber entries.
3. *RRC Connection Drops*:
   - Fixed inconsistencies in tac and gnbSearchList settings in ueransim-gnb.yaml.

For a comprehensive list of troubleshooting steps and solutions, refer to the 2 pdf's uploaded.

---

## Acknowledgments
We extend our gratitude to the open-source communities behind *Open5GS, **Free5GC, and **UERANSIM* for their excellent tools and documentation, which made this project possible. And also this project would have not been possible without the guidance of our professor.

---
