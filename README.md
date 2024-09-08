# CANoe ECU Speed and Acceleration Control

## Project Overview

This project involves creating a simulation system for ECU speed and acceleration control using CANoe. The system includes two virtual ECUs:
1. **ACC ECU**: Manages the accelerator control.
2. **Speed ECU**: Controls and monitors the speed.

The simulation operates on a virtual CAN bus and includes a CANoe database, CAPL scripts for ECU simulation, and a custom panel with interactive controls. The panel features a switch to toggle acceleration and a speed gauge that dynamically updates based on the speed value.

## Components

### 1. CANoe Database

- **Description**: Contains the database configuration for CANoe, including message definitions, signals, and network configurations for both ECUs.
- **Files**: (List specific files here, e.g., `ecu_database.dbc`)

### 2. CAPL Scripts

- **`speed_control.capl`**: Script for the Speed ECU. Simulates ECU speed control by adjusting speed values based on accelerator input and sending the updated speed values periodically.
- **`acceleration_control.capl`**: Script for the ACC ECU. Manages the acceleration signal by reading from the system variable and periodically sending the signal.

### 3. Custom Panel

- **Description**: A panel created in CANoe that provides user interface elements for controlling the ECUs.
- **Features**:
  - **Switch**: Toggles acceleration on and off for the ACC ECU.
  - **Speed Gauge**: Displays and updates the current speed for the Speed ECU in real-time.

## System Configuration

- **ECUs**: The system simulates two ECUs:
  - **ACC ECU**: Controls the acceleration.
  - **Speed ECU**: Manages and reports the speed.

- **Simulation Mode**: The system is configured to operate in simulation mode using a virtual CAN bus. This setup allows for testing and validation of ECU interactions in a controlled virtual environment.
