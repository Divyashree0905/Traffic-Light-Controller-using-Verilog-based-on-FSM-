# Traffic-Light-Controller-using-Verilog-based-on-FSM

This repository contains the Verilog code, testbench, and simulation outputs for a Traffic Signal Controller modeled using a Finite State Machine (FSM). Designed and simulated using Vivado 2015.2, this project demonstrates a basic embedded system design for real-time traffic signal management based on vehicle presence.

🎯 Objective
To implement a Traffic Signal Controller for a two-way intersection using Verilog. The controller gives priority to highway traffic and switches signals when a vehicle is detected on the country road (X = 1).

🛠️ Tools Used
Vivado 2015.2 (Xilinx)

Verilog HDL

Simulation + RTL Analysis tools

🧠 FSM Design
🚧 States:
| State | Highway Light | Country Light | Description        |
| ----- | ------------- | ------------- | ------------------ |
| S0    | GREEN         | RED           | Default state      |
| S1    | YELLOW        | RED           | Highway slowing    |
| S2    | RED           | RED           | Both stop          |
| S3    | RED           | GREEN         | Country gets green |
| S4    | RED           | YELLOW        | Country slowing    |


📶 Transition Logic:

*If a car is detected on the country road (X = 1), the FSM moves from S0 → S1 → S2 → S3.

*After a predefined delay or when X = 0, it transitions back to S0.

🧪 Testbench
The testbench initializes the clock, control signals (clear, X) and toggles them with appropriate delays to simulate different traffic conditions.

📊 Simulation Output
 The simulation output RTL shematic and Run Bheavioural Simulation is attatched in the files.

 📝 Learnings
 *Gained hands-on experience with FSM design using Verilog.
 
 *Learned testbench writing and signal debugging in Vivado.
 
 *Learnt to resolve errors during simulation.
 
 *By doing this project I understood the real time applications of vivado and verilog.

 **👩‍💻 Author
Divyashree Vyas

Department of ECE

Matrusri Engineering College**


_Feel free to fork and improve this project for learning purposes!_

_This project is licensed for educational purposes. If reused in other works, kindly cite the source._
