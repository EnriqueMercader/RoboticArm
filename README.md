# 3-DOF Industrial Robotic Arm (Electronics & Firmware)

**Complete embedded control system for a 3-DOF + gripper robotic arm** built from scratch using only a PIC16F18876 microcontroller and DC motors (no servos or steppers).

![Robotic Arm Hero](https://www.enrique-mercader.com/assets/images/projects/robotic-arm/hero-arm.jpg)  
*Precise PID position control with encoders, PWM H-bridge drives, UART PC interface, and RGB status indication*

## Highlights
- Full custom electronics and firmware for 3 axes + gripper using DC motors only
- PWM-driven H-bridge control with quadrature encoders
- Custom PID algorithms for accurate position and speed control
- UART command protocol for PC-based kinematics and real-time control
- RGB LED status system (calibration, motion, idle, error)
- All firmware and supporting libraries written from scratch with focus on efficiency and reliability

**Full Project Page** → [enrique-mercader.com/projects/3-dof-industrial-robotic-arm](https://www.enrique-mercader.com/projects/3-dof-industrial-robotic-arm)  
**Live Demo Video** → 

---

## Repository Structure

```bash
# 3-DOF-Industrial-Robotic-Arm/
├── README.md
├── Hardware/
│   ├── Schematic.pdf
│   ├── Gerber/
│   ├── BOM.csv
│   └── Photos/
├── Firmware/
│   └── roboticArm.X/          # Full MPLAB X project
├── Code Files/                # (existing folder - we'll keep & organize)
├── Media/
│   ├── Demo_Videos/
│   ├── Action_GIFs/
│   └── Build_Photos/
└── Docs/
    └── Design_Notes_PID_Tuning.pdf
```

## Technical Deep Dive

- Microcontroller: PIC16F18876 (bare-metal C)
- Motor Control: PWM H-bridge drivers with dead-time and current limiting
- Feedback: Quadrature encoders + custom PID position loops
- Communication: UART protocol for external kinematics commands
- User Feedback: RGB LED states + optional 7-segment or LCD
- Tools: MPLAB X, EasyEDA, oscilloscope, custom test rigs

Every line of code was written emphasizing minimal resource usage, real-time performance, and clean, maintainable architecture.

## How to Use / Replicate
0. Clone the repository
1. Open Firmware/roboticArm.X in MPLAB X IDE
2. Program the PIC16F18876
3. Assemble the power stage using the schematic and Gerbers
4. Connect DC motors with encoders and power supply
5. Use the UART protocol to send position commands from a PC

**Safety Note: Motors can move quickly — use in a controlled environment.

## Results & Impact
- Achieved precise, repeatable motion under strict course constraints (DC motors only)
- Delivered complete ownership: electronics design + firmware + integration + testing
- Demonstrates strong skills in real-time control, PID, embedded systems, and mechatronics integration — directly relevant to industrial automation and robotics roles

---

**Connect with me**  
[LinkedIn](https://www.linkedin.com/in/enrique-mercader/) | [Personal Website](https://www.enrique-mercader.com) | [Resume](https://www.enrique-mercader.com/resume)
