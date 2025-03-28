# DD-24-25-FLLSubmerged
# LEGO Robotics Competition Run Execution Script

## Overview
This Python script is designed for a LEGO robotics competition, specifically for controlling a robot's movements and executing multiple runs with precise motor control and gyroscopic navigation.

## Features

### Robot Capabilities
- Precise movement control using motor pairs
- Gyroscopic angle tracking and navigation
- Autonomous run execution with customizable run sequences

### Key Functions
- `execute()`: Main function to run multiple competition runs
- `follow_gyro_angle()`: Implements PID-like control for straight-line movement
- `pivot_gyro_turn_abs()`: Precise turning using gyroscopic angle measurement
- Utility functions for:
  - Distance calculation
  - Yaw angle tracking
  - Motor positioning
  - Time tracking

## Run Configurations
The script supports multiple run configurations:
- Slot 0: Execute all runs (1-19)
- Slot 1: Run 2 onwards
- Slot 2: Run 3 onwards
- Slot 3: Run 4 onwards
- Slot 4: Run 5 onwards
- ........

## Initialization
- Resets motion sensor yaw
- Configures motor pairs
- Provides visual feedback using light matrix

## Execution Details
- Waits for left button press to start each run
- Tracks and reports:
  - Individual run times
  - Transition times between runs
  - Total execution time

## Hardware Requirements
- LEGO robotics hub
- Motors connected to ports A (wheel), E(wheel), B(attachment), and C(attachment)
- Motion sensor
- Light matrix

## Dependencies
- `hub`
- `sys`
- `time`
- Custom modules: `color`, `motor`, `motor_pair`, `runloop`

## Usage
Uncomment the desired run configuration in the script and run using a LEGO robotics programming environment.

## Note
This script appears to be part of a specific robotics competition, likely involving marine or ocean-related missions based on references to plankton, shipping lanes, and seabed samples.