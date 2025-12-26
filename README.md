# Automated-Assembly-Line-PLC
Control logic for a rotary table and pneumatic sorting system using Siemens TIA Portal V15.1

This repository contains the control logic for an automated sorting line, developed in **Siemens TIA Portal V15.1**. The system manages a rotary table, multiple pneumatic pistons, and a conveyor belt to sort objects based on height detection.

## 🛠 Technologies
* [cite_start]**Environment:** Siemens TIA Portal V15.1 
* **Language:** Ladder Logic (LAD)
* **Hardware:** S7-1200 1215C DC/DC/DC

## ⚙️ Key Features
* **Modular Architecture:** Uses generic Function Blocks (FB) for pneumatic pistons to ensure code reusability.
* **Sequential Control:** Implements precise timing and synchronization between the rotary table and actuators.
* **Data Handling:** Uses Data Blocks (DB) to track object properties (ID, Height) as they move through the station positions.
* **Mode Handling:** Supports initialization and cyclic operation modes.

## 📸 Logic Snapshots

### Main Organization Block (OB1)
*Overview of the main cycle and function calls.*
![OB1 Logic](img/screen_ob1.png) *(Здесь вставь путь к своему скриншоту)*

### Piston Function Block (FB)
*Reusable logic for pneumatic cylinder control including timer interlocking.*
![Piston FB](img/screen_fb_piest.png)

### Data Structure
*Data Block showing the tracking of object positions.*
![DB Structure](img/screen_db.png)

## 🚀 How to Run
1.  Download the archived project file: `plc_project.zap15_1`.
2.  Open **TIA Portal V15.1** (or newer).
3.  Select "Retrieve" project and select the `.zap15_1` file.
