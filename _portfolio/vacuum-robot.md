---
title: "Autonomous Vacuum Robot (Mechatronics System Design)"
excerpt: "An autonomous mobile vacuum robot integrating embedded control, PID-based navigation, and vision-assisted perception."
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
focused on autonomous navigation and embedded control for mobile robotic platforms.

**Project Type:** Mechatronics system design and robotics  
**Application Domain:** Autonomous mobile robots  
**Problem Focus:** Embedded control, sensing integration, and closed-loop autonomous navigation  

This page documents **only the components I personally designed, implemented,
and tested** within the overall system.

---

## My Role and Contributions

I was responsible for key aspects of the **hardware control, embedded perception,
and system-level integration** of the autonomous vacuum robot.

My contributions include:

- Designing and validating the **robot control circuitry**, including motor power
  distribution and interface considerations
- Co-configuring the **Raspberry Pi software environment** for embedded vision
  and sensor integration
- Participating in **robot chassis assembly and hardware integration**, ensuring
  stable mounting, wiring reliability, and accessibility for debugging
- Developing and optimizing **vision-based image recognition algorithms**
  for real-time color detection
- Assisting with **PID control testing and parameter tuning**, focusing on
  system stability and real-world behavior
- Supporting **system-level debugging** across hardware, embedded software,
  and perception modules

My work focused on ensuring **reliable interaction between sensing, computation,
and physical actuation** under real-time constraints.

---

## System Overview

The autonomous vacuum robot integrates embedded control, perception, and actuation
to achieve autonomous navigation and debris collection.

Key system components include:

- Arduino-based motor control with closed-loop feedback
- Raspberry Pi for real-time image-based perception
- Ultrasonic sensors for distance measurement and obstacle detection
- H-bridge motor driver for differential drive control
- Inter-processor communication between Arduino and Raspberry Pi

---

## Control and Embedded Implementation

### PID-Based Autonomous Navigation

I participated in the **testing and validation of a PID-based control strategy**
used for wall-following and autonomous navigation.

My involvement included:

- Assisting with the definition of distance error metrics using ultrasonic sensor feedback
- Supporting PID parameter tuning through repeated testing
- Evaluating system stability and responsiveness under different gain settings
- Identifying control-induced oscillations and mechanical stress issues during testing

This process helped refine the control behavior
and improve navigation reliability under real-world conditions.

---

## Embedded Vision and System Integration

To support perception-driven behaviors, I developed and optimized
the embedded vision pipeline on the Raspberry Pi.

My contributions include:

- Implementing **real-time color detection algorithms** for visual event recognition
- Configuring the Raspberry Pi environment for stable camera operation
- Supporting communication between Raspberry Pi and Arduino
  for perception-driven control decisions
- Assisting with debugging issues related to processing latency
  and hardware reliability

This perception module enabled the robot to react to visual cues
and modify behavior accordingly.

---

## System Operation and Limitations

During testing and competition deployment, the system demonstrated:

- Fully autonomous operation using embedded control logic
- Reliable wall-following behavior under PID control
- Successful integration of vision-based perception with motion control

However, real-world deployment revealed system-level limitations, including:

- Mechanical reliability issues after extensive testing
- Sensitivity to hardware wear, such as motor gear loosening
- Limited opportunity for full-scale environment testing prior to competition

These constraints highlighted the importance of **robust hardware validation**
and **system-level fault tolerance** in autonomous robotic systems.

---

## Outcomes and Impact

My contributions enabled:

- Successful demonstration of a **fully autonomous control strategy**
- Reliable integration of embedded perception with motion control
- Practical experience with system uncertainty, hardware failure modes,
  and real-world testing constraints

This project strengthened my experience in **embedded robotics,
system integration, and experimental validation**.

---

## Skills and Tools Used

- Arduino IDE
- Raspberry Pi
- Embedded C and Python
- PID control testing and tuning
- Sensor integration
- Embedded vision systems
- System-level debugging and testing
