# Enhanced Regenerative Braking Control for Dual-Motor Electric Vehicles

## Overview

This project focuses on regenerative braking control for a dual-motor electric vehicle.

During braking, the kinetic energy of the vehicle is converted into electrical energy instead of being completely dissipated as heat. The recovered electrical energy is stored using a hybrid energy storage system consisting of a Lithium-ion battery and a supercapacitor.

A Deep Reinforcement Learning (DRL) based control strategy is used to determine an appropriate energy-management action during regenerative braking.

The main objective of the project is to improve energy recovery, efficiently manage the battery and supercapacitor, and increase the overall efficiency of the electric vehicle.

## Project Title

Enhanced Regenerative Braking Control for Dual-Motor Electric Vehicles with Supercapacitor-Assisted Energy Recovery Using Deep Reinforcement Learning

## Key Features

- Dual-motor electric vehicle model
- Regenerative braking
- Hybrid energy storage system
- Lithium-ion battery
- Supercapacitor
- Deep Reinforcement Learning based control
- Energy recovery optimization
- Intelligent energy management
- Improved electric vehicle efficiency

## Introduction

Electric vehicles use electric motors for propulsion and can recover a portion of the vehicle's kinetic energy during braking.

In conventional braking, a large portion of the vehicle's kinetic energy is converted into heat and dissipated through the braking system.

Regenerative braking allows the electric motors to operate as generators during deceleration. The generated electrical energy can be recovered and stored in an energy storage system.

In this project, a dual-motor electric vehicle is considered along with a hybrid energy storage system consisting of a Lithium-ion battery and a supercapacitor.

A Deep Reinforcement Learning based control strategy is used to manage the recovered energy and determine an appropriate energy-sharing strategy.

## Regenerative Braking

Regenerative braking is a technique in which the electric motor operates as a generator during vehicle deceleration.

The kinetic energy of the moving vehicle is converted into electrical energy and supplied to the energy storage system.

The basic energy flow is:

Vehicle Kinetic Energy
        ↓
   Braking Event
        ↓
 Electric Motor
   as Generator
        ↓
 Regenerated Electrical Energy
        ↓
 Energy Management Controller
        ↓
 ┌──────┴──────────┐
 ↓                 ↓
Battery       Supercapacitor

This process helps recover energy that would otherwise be lost as heat.

## Why Dual-Motor?

A dual-motor electric vehicle uses two electric motors for propulsion and braking.

The use of two motors provides additional flexibility in controlling the distribution of torque and regenerative braking power.

During braking, the recovered energy from the motors can be managed according to the operating condition of the vehicle and the energy storage system.

## Why Supercapacitor?

A supercapacitor can charge and discharge very quickly and can handle high power over short periods.

During regenerative braking, a high amount of electrical power may be generated within a short time.

The supercapacitor is suitable for handling these high-power transient events, while the Lithium-ion battery is better suited for longer-duration energy storage.

Therefore, combining a Lithium-ion battery with a supercapacitor provides a hybrid energy storage system for improved energy management.

### Advantages of Supercapacitor

- Fast charging
- Fast discharging
- High power capability
- Suitable for short-duration high-power events
- Reduces the stress associated with high-power transient operation of the battery
- Useful for regenerative braking applications

## Hybrid Energy Storage System

The project uses two energy storage elements:

### Lithium-ion Battery

The Lithium-ion battery provides high energy density and is suitable for storing energy for longer durations.

### Supercapacitor

The supercapacitor provides high power density and can rapidly absorb and release energy during transient events such as regenerative braking.

The combination of both storage elements allows the system to manage recovered braking energy more effectively.

## Deep Reinforcement Learning

Deep Reinforcement Learning (DRL) is used to develop an intelligent control strategy for energy management.

The controller learns suitable control actions by interacting with the electric vehicle system and receiving feedback based on the system performance.

The objective is to determine an appropriate power-sharing strategy between the battery and supercapacitor while improving energy recovery and maintaining system constraints.

The basic concept is:

System State
     ↓
DRL Controller
     ↓
Control Action
     ↓
EV Energy Management
     ↓
System Response
     ↓
Reward / Feedback
     ↓
DRL Controller

Through this interaction, the controller learns an effective energy-management strategy.

## TD3 Algorithm

TD3 stands for:

Twin Delayed Deep Deterministic Policy Gradient.

TD3 is a Deep Reinforcement Learning algorithm designed for continuous control problems.

In this project, TD3 is used to learn an appropriate control action for regenerative energy management.

TD3 uses two critic networks and delayed policy updates to reduce overestimation and improve the stability of the learning process.

The learned controller determines an appropriate control action based on the operating condition of the electric vehicle and energy storage system.

## Project Methodology

The project follows the following general process:

1. Develop the dual-motor electric vehicle model.
2. Model the regenerative braking system.
3. Model the Lithium-ion battery.
4. Model the supercapacitor.
5. Develop the hybrid energy storage system.
6. Define the energy-management control problem.
7. Apply Deep Reinforcement Learning.
8. Train the TD3 based controller.
9. Evaluate the regenerative braking performance.
10. Analyze the recovered energy and system efficiency.

## System Concept

                    ┌─────────────────────┐
                    │   Dual-Motor EV     │
                    │                     │
                    │ Motor 1 + Motor 2   │
                    └──────────┬──────────┘
                               │
                         Braking Event
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Regenerative        │
                    │ Braking System      │
                    └──────────┬──────────┘
                               │
                        Recovered Energy
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Energy Management   │
                    │ Controller          │
                    │       TD3 / DRL     │
                    └──────────┬──────────┘
                               │
                     ┌─────────┴─────────┐
                     │                   │
                     ▼                   ▼
              ┌─────────────┐     ┌──────────────┐
              │ Lithium-ion │     │ Supercapacitor│
              │   Battery   │     │              │
              └─────────────┘     └──────────────┘

## Energy Flow During Regenerative Braking

During braking, the electric motors operate as generators and convert part of the vehicle's kinetic energy into electrical energy.

The recovered energy is then managed by the energy-management controller.

The controller determines how the recovered power should be distributed between the Lithium-ion battery and supercapacitor.

The overall concept is:

Braking
   ↓
Motor Generating Mode
   ↓
Electrical Energy Recovery
   ↓
Energy Management Controller
   ↓
Battery + Supercapacitor
   ↓
Stored Electrical Energy

## Project Objectives

The main objectives of this project are:

- Improve regenerative braking energy recovery
- Efficiently manage recovered braking energy
- Utilize a supercapacitor for high-power transient energy
- Improve battery and supercapacitor energy management
- Develop an intelligent control strategy
- Reduce energy losses during braking
- Improve overall electric vehicle efficiency

## Expected Benefits

- Improved regenerative energy recovery
- Better utilization of the hybrid energy storage system
- Improved energy-management performance
- Reduced energy losses during braking
- Better utilization of the supercapacitor during high-power events
- Improved electric vehicle efficiency

## Applications

The concepts developed in this project can be applied to:

- Electric vehicles
- Hybrid electric vehicles
- Dual-motor electric vehicles
- Electric buses
- Electric commercial vehicles
- Regenerative braking systems
- Battery-supercapacitor hybrid energy storage systems

## Technologies and Concepts

- Electric Vehicle Technology
- Regenerative Braking
- Dual-Motor Drive
- Lithium-ion Battery
- Supercapacitor
- Hybrid Energy Storage System
- Energy Management
- Deep Reinforcement Learning
- TD3 Algorithm
- MATLAB/Simulink

## Project Outcomes

The project demonstrates the use of Deep Reinforcement Learning for intelligent energy management in a dual-motor electric vehicle.

The use of a supercapacitor along with a Lithium-ion battery provides a suitable approach for handling both energy and high-power transient requirements during regenerative braking.

The DRL-based controller is designed to improve the management of recovered braking energy and contribute to improved electric vehicle efficiency.

## Future Improvements

The project can be further improved by:

- Implementing the controller on a real-time embedded platform
- Testing with real electric vehicle hardware
- Integrating real-time battery and supercapacitor measurements
- Developing hardware-in-the-loop testing
- Improving the reinforcement learning model
- Comparing additional DRL algorithms
- Developing real-time energy-management control
- Integrating advanced vehicle drive-cycle testing

## Project Reference

IEEE Xplore:

https://ieeexplore.ieee.org/document/11507980

## Repository Structure

The repository can contain the following files:

Dual-Motor-EV-Regenerative-Braking/
│
├── README.md
├── Simulation/
│   └── Simulation files
├── Results/
│   └── Simulation results and graphs
└── Images/
    └── Project diagrams and results

## Author

Sabari

Electrical & Electronics Engineering

Embedded Systems / Firmware Engineer Fresher
