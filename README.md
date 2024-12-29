
# GOAT Robot - VTOL Gliding System

This repository contains the design, code, and test setup for the GOAT robot, a compliant robot based on a VTOL (Vertical Take-Off and Landing) design that glides efficiently while retaining the ability to drive and swim. The project aims to achieve energy-efficient flight with the added functionality of ground and water mobility.

<img src="https://github.com/user-attachments/assets/3a97b29b-489d-403d-9799-33ce839eb9e6" alt="2024_GOAT_GH_MAIN_ASSEMBLY_V3_2024-Dec-27_02-59-24PM_cut" width="600"/>


## Features
- **VTOL Design**: Transition from vertical lift-off to gliding flight, optimizing energy efficiency.
- **Dual-mode Functionality**: Capable of both aerial flight and ground/water navigation.
- **PID Control**: Stabilized yaw control in the forward flight configuration.
- **Adaptable Structure**: The robot's structure is locked in an oval configuration, allowing for rigidity during test flights.

## Hardware
- **Brushless Motors**: Two brushless motors mounted on separate aluminum tubes.
- **Servomotors**: Two servomotors for controlling rotation of the tubes via 3D-printed gears.
- **3D-Printed Components**: Custom parts for motor mounts, gears, and bushings.
- **Plastic Sides**: The sides of the structure are covered with plastic to trap air and generate lift in the wind.

## Setup
1. Clone the repository:
2. Install dependencies (e.g., PID control libraries, flight controller libraries).
3. Flash the firmware onto the flight controller (e.g., Teensy 3.0).
4. Set up the hardware as described in the repo with brushless motors, servos, and other components.

## Test Setup
- The robot was tested in various configurations, including forward flight and wind tunnel experiments.
- Wind speed was varied from 6.8 m/s to 9.6 m/s during the wind test.
- Tests showed that the robot maintained stability and was able to generate sufficient lift, although higher wind speeds led to instability.

## Test Results

- Unstable recorded reaction (untuned PID)  
  <img src="https://github.com/user-attachments/assets/34d5b4fb-87e7-4fba-a421-5eb507ebe9cc" alt="Unstable reaction (untuned PID)" width="600"/>

- Mostly stable recorded reaction (tuned PID)  
  <img src="https://github.com/user-attachments/assets/9717d1be-be87-46d0-b1a7-5e72c06c75fd" alt="Stable reaction (tuned PID)" width="600"/>

- Yaw comparisons with the wind  
  <img src="https://github.com/user-attachments/assets/85c2b22c-0eee-4fc9-8a65-f8eacadeecb9" alt="Yaw comparisons with the wind" width="600"/>



## Future Work
- Improve PID controller for better performance under dynamic wind conditions.
- Enhance aerodynamic design to increase lift and stability.
- Expand testing to outdoor environments.


## Acknowledgments
- The dRehmFlight VTOL flight controller is used for controlling the robot's flight dynamics. [GitHub Link](https://github.com/nickrehm/dRehmFlight)
