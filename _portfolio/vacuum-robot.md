---
title: "Autonomous Vacuum Robot (Mechatronics System Design)"
excerpt: "An autonomous mobile vacuum robot integrating embedded control, PID-based navigation, and sensor-driven system integration."
collection: portfolio
permalink: /projects/autonomous-vacuum-robot/
project_start: 2024-09-01
project_end: 2024-12-14
project_type: "Mechatronics / Robotics"
layout: single
order: 3
---

## Project Context

This project was conducted as a **course-based mechatronics system design project**
focusing on autonomous navigation and embedded control for mobile robotic platforms.

**Project Type:** Mechatronics system design & robotics  
**Application Domain:** Autonomous mobile robots  
**Problem Focus:** Embedded control, sensing integration, and closed-loop navigation  

This page documents the **components I personally designed and implemented**
within the overall system.

## My Role and Contributions

I was responsible for key aspects of the **embedded systems, hardware integration,
and vision-based perception** of the autonomous vacuum robot.

My contributions include:

- Designing the **robot control circuitry**, including power distribution and
  motor interface considerations
- Co-configuring the **Raspberry Pi environment**, including system setup and
  integration with peripheral sensors
- Participating in **robot chassis assembly and hardware integration**, ensuring
  reliable mounting, wiring, and component accessibility
- Developing and optimizing **vision-based image recognition algorithms**
  for real-time perception tasks
- Supporting system-level debugging across hardware, embedded software,
  and perception modules

My work focused on ensuring **reliable interaction between sensing, computation,
and physical hardware** within the autonomous system.

---

## System Overview

The autonomous vacuum robot consists of an embedded control architecture
that integrates sensing, computation, and actuation for autonomous navigation.

The system includes:

- Embedded motor control with closed-loop feedback
- Sensor-based distance measurement for obstacle avoidance
- Vision-assisted perception using Raspberry Pi
- Inter-processor communication for coordinated decision-making

---

## Control and Embedded Implementation

### PID-Based Navigation Control

I implemented a **PID control strategy** to regulate robot motion during wall-following
and obstacle-avoidance behaviors.

Key aspects include:

- Defining distance and orientation error metrics using ultrasonic sensor feedback
- Tuning proportional, integral, and derivative gains to ensure stable motion
- Limiting motor speed to prevent control-induced oscillations
- Achieving consistent navigation without predefined trajectories

---

## Embedded Vision and System Integration

To support perception-driven behaviors, I contributed to the development
and optimization of the embedded vision pipeline.

My work includes:

- Implementing image recognition algorithms for color-based detection
- Optimizing perception performance for real-time execution on Raspberry Pi
- Configuring the embedded software environment for stable operation
- Assisting with integration between vision outputs and control logic

These components enabled perception-informed decision-making
within the autonomous navigation system.

---

## Outcomes and Impact

My contributions enabled:

- Stable autonomous wall-following behavior using embedded PID control
- Reliable integration between sensing, computation, and actuation
- Successful demonstration of a fully autonomous control strategy
- Identification of system-level limitations related to hardware reliability
  and inter-processor communication

This project strengthened my experience in **robot control systems,
embedded software development, and system integration**.

---

## Skills and Tools Used

- Arduino IDE
- Raspberry Pi
- PID control
- Embedded systems programming
- Sensor integration
- Inter-processor communication
- System-level debugging and testing
