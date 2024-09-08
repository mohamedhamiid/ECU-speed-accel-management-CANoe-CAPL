# CANoe ECU Speed and Acceleration Control

## Project Overview

This project involves creating a simulation system for ECU speed and acceleration control using CANoe. The system includes two virtual ECUs:
1. **ACC ECU**: Manages the accelerator control.
2. **Speed ECU**: Controls and monitors the speed.

The simulation operates on a virtual CAN bus that is tested using XL CAN Control before starting and includes a CANoe database, CAPL scripts for ECU simulation, and a custom panel with interactive controls. The panel features a switch to toggle acceleration and a speed gauge that dynamically updates based on the speed value.
#### XL Control 
![XL driver](https://github.com/user-attachments/assets/d3224578-af63-4d3a-90ff-1589a2035a1c)
#### Network Components
![System](https://github.com/user-attachments/assets/fec755ae-9f4a-442f-9862-955be9f2b47c)

## Components

### 1. CANoe Database

- **Description**: Contains the database configuration for CANoe, including message definitions, signals, and network configurations for both ECUs.
- **Files**: (List specific files here, e.g., `ecu_database.dbc`)
<br></br>
![Database](https://github.com/user-attachments/assets/77e3a8eb-69ef-4236-a60b-0a71050588b3)

### 2. CAPL Scripts

- **`ECU1_ACC.capl`**: Script for the Speed ECU. Simulates ECU speed control by adjusting speed values based on accelerator input and sending the updated speed values periodically.
- **`ECU2_SPEED.capl`**: Script for the ACC ECU. Manages the acceleration signal by reading from the system variable and periodically sending the signal.

### 3. Custom Panel

- **Description**: A panel created in CANoe that provides user interface elements for controlling the ECUs.
- **Features**:
  - **Switch**: Toggles acceleration on and off for the ACC ECU.
  - **Speed Gauge**: Displays and updates the current speed for the Speed ECU in real-time.
<br></br>
![Panel](https://github.com/user-attachments/assets/29491738-ac6d-47b1-b798-1e51acadf501)
