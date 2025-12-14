---
title: "Autonomous Vacuum Robot (Mechatronics System Design)"
excerpt: "Designed and built an autonomous mobile vacuum robot integrating mechanical design, embedded control, sensing, and system-level integration."
collection: portfolio
permalink: /projects/autonomous-vacuum-robot/
project_start: 2024-09-01
project_end: 2024-12-14
project_type: "Mechatronics / Robotics"
layout: single
order: 3
---

## Project Context

This project was conducted as a **mechatronics system design and robotics integration project**, with the goal of developing a fully autonomous mobile vacuum robot capable of real-world navigation and debris collection.

**Project Type:** Course-based mechatronics and robotics system design  
**Application Domain:** Autonomous mobile robotics  
**Engineering Focus:** Mechanical design, embedded control, sensing, and system integration  

The project emphasized **end-to-end system development**, from mechanical design and airflow optimization to embedded control, sensing, and autonomous behavior without predefined trajectories.

## My Role and Contributions

I was responsible for the **overall system design and integration**, covering mechanical, electrical, and software components.

My contributions include:

- Designing the complete mechanical structure, vacuum module, and chassis
- Implementing embedded motor control and PID-based navigation algorithms
- Integrating ultrasonic sensing and vision-based perception
- Managing inter-processor communication between Arduino and Raspberry Pi
- Performing system-level tuning, testing, and failure analysis
- Leading system integration and final autonomous deployment

This project reflects hands-on experience in **robotics system engineering**, where mechanical design, control, sensing, and computation must function cohesively.

## System Overview

The autonomous vacuum robot consists of multiple tightly coupled subsystems:

- Embedded motor control and navigation
- Ultrasonic-based obstacle avoidance and wall-following
- Vision-based color detection
- Custom-designed vacuum and debris collection module

The system operates fully autonomously, relying on onboard sensing and control without external localization or predefined paths.

## Embedded Control and Navigation

### Motor Control and PID Regulation

- Implemented Arduino-based motor control using DC motors and an H-bridge driver
- Designed PID controllers for wall-following navigation
- Defined distance and orientation error metrics using dual ultrasonic sensors
- Tuned control gains to achieve stable motion and reduce oscillations
- Applied wheel speed limits to prevent instability during tight maneuvers

This control strategy enabled smooth navigation while maintaining consistent wall-following behavior.

## Sensing and Perception

### Ultrasonic Sensing

- Integrated ultrasonic sensors for real-time distance measurement
- Used sensor logic to support obstacle avoidance and wall-following
- Addressed noisy measurements through filtering and control constraints

### Vision-Based Detection

- Developed a Raspberry Pi pipeline for real-time color detection
- Used vision cues to support navigation and task-specific behaviors
- Designed communication protocols between Raspberry Pi and Arduino

## Mechanical Design and Fabrication

- Designed vacuum fan, intake geometry, and dust container from scratch
- Optimized airflow performance using Autodesk CFD simulations
- Redesigned chassis for improved stability, wiring organization, and accessibility
- Fabricated structural and vacuum components using 3D printing
- Integrated mechanical design constraints with electrical and sensing layouts

The mechanical subsystem was designed to support both **functional vacuum performance** and **robust system integration**.

## System Integration and Reliability

- Coordinated sensing, control, and actuation across heterogeneous hardware
- Identified and mitigated communication overload between processors
- Designed fault-handling strategies to improve runtime stability
- Performed iterative debugging and system-level testing

This phase highlighted the challenges of **real-world robotics integration**, where performance is constrained by hardware reliability and communication limits.

## Results and Demonstration

- Successfully demonstrated fully autonomous navigation in the final competition
- Achieved reliable debris collection and wall-following behavior
- Only team to deploy a completely autonomous control strategy
- Completed the task without predefined trajectories or external control

## Lessons Learned and Impact

This project reinforced key principles in robotics and mechatronics engineering:

- Effective robotics systems require tight coordination between mechanics, control, sensing, and computation
- System-level reliability is often the limiting factor, not individual algorithm performance
- Early integration and iterative testing are critical for autonomous systems

The project demonstrates my ability to **design, implement, and debug complex mechatronic systems** in realistic engineering settings.

## Skills and Tools Used

Arduino, Raspberry Pi, Embedded systems, Motor control, PID control, Ultrasonic sensing, Vision pipelines, CAD, Autodesk CFD, 3D printing, Robotics system integration
