
# Logic-Based Room Booking System – NIMA Learning Center

## Overview
This project presents a digital logic-based room booking system developed in Logisim for the NIMA Learning Center.  
It automates the process of discussion room allocation using basic logic gates and flip-flops.

The motivation for this project originated from the inefficiencies in the library’s existing system, where students must submit separate Google Forms for each room to check availability. Only after submission do they learn whether a room is occupied. This process is repetitive and time-consuming.  
To address this issue, the system was designed to automatically detect available rooms and assign them efficiently through hardware-based logic design.

---

## Objective
The objective of this project is to design and simulate a hardware-based booking logic system that:
- Detects available rooms among a fixed set (10 in this case).
- Allocates the next available room upon request.
- Maintains room status (occupied or free) using flip-flops.
- Displays the assigned room number or indicates if all rooms are full.

---

## Project Concept
The system operates as follows:
- When a booking request (REQ) is received, it scans all rooms sequentially.
- The first available room (logic 0) is assigned.
- The corresponding flip-flop is toggled to logic 1, indicating the room is now occupied.
- If all rooms are occupied, the circuit outputs -1, signaling “No Room Available.”
- The system continuously monitors room status and updates availability.

---

## Motivation
This is my first project using Logisim. Initially, the tool was challenging to use, but through experimentation, I gained a deeper understanding of how digital systems can solve practical problems.  
By modeling this system, I developed hands-on experience with sequential circuits, flip-flops, and logic design concepts.

---

## Current Status
The current circuit implementation:
- Successfully identifies and assigns the next available room.
- Displays the room number in binary or Boolean form.
- Uses flip-flops to store the occupancy status of each room.

**Known Limitation:**
- The circuit currently lacks an occupy button and automatic release mechanism.
- Pressing the REQ button multiple times can activate multiple LEDs simultaneously.
- The next step is to implement an OCCUPY button that locks a room once assigned, and a timing circuit to automatically reset room availability after a fixed duration.

---

## Logic Components Used
- **Logic Gates:** AND, OR, NOT  
- **Memory Elements:** D Flip-Flops  
- **Input Devices:** Buttons (Request, Occupy, Reset)  
- **Output Devices:** LEDs for status indication  
- **Clock Generator:** To manage synchronization and timing

---

## Applications
- Automated discussion room allocation in libraries and study centers.
- Resource allocation systems such as computer lab or meeting room booking.
- Queue or token management systems requiring sequential assignment.
- Potential extension to IoT-based smart facility management systems.

---

## Advantages
- Reduces manual effort in room allocation.
- Provides immediate feedback on room availability.
- Ensures efficient utilization of resources.
- Simple and cost-effective hardware implementation using basic logic components.
- Can be scaled for more rooms or different booking intervals.

---

## Future Enhancements
- Add an Occupy and Release mechanism for dynamic state management.
- Implement a Timer circuit for automatic room release after a fixed time.
- Integrate a 7-segment display for room number visualization.
- Use subcircuits to improve modularity and readability.
- Interface the circuit with a microcontroller or Raspberry Pi for real-time application.

---

## File Information
- `innovassi.circ` – Logisim circuit file  
- `Project_Report.docx` – Documentation of project methodology  
- `Circuit_Diagram.png` – Schematic diagram for reference

---

## Author
**Heer**  
Second-year engineering student exploring digital logic design and automation systems.  
This project was developed as part of a college assignment using guided experimentation and online resources.

---

**Note:** This project is currently in development. Suggestions and feedback for improvement are welcome.
