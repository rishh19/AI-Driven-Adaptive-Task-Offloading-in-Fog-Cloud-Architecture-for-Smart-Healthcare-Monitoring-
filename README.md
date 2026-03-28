#  AI-Driven Adaptive Task Offloading in Fog-Cloud Architecture for Smart Healthcare Monitoring

---

##  Overview

This project presents an **AI-driven adaptive task offloading framework** for smart healthcare systems using a **fog-cloud architecture**.

Modern healthcare IoMT (Internet of Medical Things) devices generate large volumes of **latency-sensitive data**, which must be processed efficiently and in real time. Traditional cloud-based approaches introduce:

* High latency
* Increased energy consumption
* Network congestion

To overcome these challenges, this project implements an intelligent scheduling system that dynamically distributes tasks between **fog nodes and cloud servers**.

---

##  Objectives

* Minimize **task response time (latency)**
* Reduce **energy consumption**
* Decrease **SLA (Service Level Agreement) violations**
* Enable efficient **real-time healthcare monitoring**

---

##  System Architecture

The system follows a **three-layer architecture**:

### 1. IoMT Layer

* Wearable medical devices (ECG, heart rate sensors, BP monitors)
* Generates healthcare monitoring tasks

### 2. Fog Layer

* Processes latency-sensitive tasks near the data source
* Reduces communication delay and network congestion

### 3. Cloud Layer

* Handles computation-intensive tasks
* Provides high processing power and storage

---

##  Methodology (Q-Learning Based Scheduling)

The task scheduling problem is modeled using **Reinforcement Learning (Q-Learning)**.

### 🔹 State (S)

* Network latency
* Node energy availability
* CPU requirement
* Task deadline

### 🔹 Action (A)

* Execute task at **Fog node**
* Offload task to **Cloud server**

### 🔹 Reward Function

R = -(Latency + Energy Consumption)

* Lower latency and energy → Higher reward
* SLA violations are penalized

The model learns optimal scheduling decisions dynamically through interaction with the environment.

---

##  Performance Metrics

The system is evaluated based on:

*  **Task Response Time (Latency)**
*  **Energy Consumption**
*  **SLA Violation Rate**

---

##  Results

| Metric             | Improvement |
| ------------------ | ----------- |
| Latency            | ↓ 15–20%    |
| Energy Consumption | ↓ 10–15%    |
| SLA Violations     | Reduced     |

---

##  Project Structure

```
.
├── adaptive_task_offloading.ipynb
├── healthcare_iomt_offloading_dataset.csv
├── latency_comparison.png
├── energy_fixed.png
├── sla_violation.png
└── README.md
```

---

##  Installation

Clone the repository:

```bash
git clone https://github.com/rishh19/AI-Driven-Adaptive-Task-Offloading-Fog-Cloud-Healthcare.git
cd AI-Driven-Adaptive-Task-Offloading-Fog-Cloud-Healthcare
```

Install dependencies:

```bash
pip install pandas numpy matplotlib
```

---

##  Usage

1. Open the Jupyter Notebook:

```bash
jupyter notebook
```

2. Run all cells in:

```
adaptive_task_offloading.ipynb
```

---

##  Future Work

* Extend to **Deep Reinforcement Learning (DRL)**
* Deploy in real-time healthcare environments
* Use larger and more diverse IoMT datasets
* Integrate real-time monitoring systems

---

##  Team Members

* **Rishav Kumar Shrivastava**
* **Priyanshu Sekhar Bhuyan**
* **Vridhi Patnala**

---

##  License

This project is developed for **academic and research purposes**.
