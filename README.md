# FPGA-Based Glass Bridge Survival Game

## Overview

The FPGA-Based Glass Bridge Survival Game is a hardware implementation of a memory-based survival game inspired by the famous Glass Bridge challenge. Developed using **Verilog HDL** and deployed on the **Xilinx Basys 3 (Artix-7 FPGA)** platform, the project demonstrates practical applications of digital logic design concepts including **Finite State Machines (FSMs)**, **Linear Feedback Shift Registers (LFSRs)**, input debouncing, display multiplexing, and real-time hardware interaction.

Players are briefly shown a randomly generated safe path across a virtual glass bridge. After the pattern disappears, they must accurately recall and select the safe panels using FPGA switches. Incorrect choices result in elimination, while successful navigation advances the player through increasingly difficult stages.

---

## Features

* FSM-based game control architecture
* LFSR-powered random bridge generation
* Four progressive difficulty levels
* Real-time player input validation
* LED-based bridge visualization
* 4-digit 7-segment display interface
* Hardware button debouncing and synchronization
* Win and lose animations
* Fully implemented on FPGA hardware

---

## Hardware Platform

* AMD/Xilinx Basys 3 FPGA Development Board
* Artix-7 FPGA
* 100 MHz System Clock
* 16 User LEDs
* 16 Slide Switches
* Push Buttons
* 4-Digit Seven-Segment Display

---

## System Architecture

The design consists of several interconnected hardware modules:

* Input Synchronization Unit
* Button Debounce Circuit
* 32-bit LFSR Random Generator
* Finite State Machine Controller
* Bridge Pattern Storage
* Choice Validation Logic
* LED Display Driver
* Seven-Segment Display Multiplexer

---

## Game Flow

### 1. Initialization

The system waits for the player to start the game.

### 2. Bridge Generation

A pseudo-random bridge pattern is generated using an LFSR.

### 3. Pattern Display

The safe path is displayed on LEDs for memorization.

### 4. Player Input

The player selects glass panels using switches and confirms selections via push buttons.

### 5. Validation

The FPGA compares the selected panel against the stored safe path.

### 6. Result

* Correct Choice → Advance
* Incorrect Choice → Game Over
* Complete All Rows → Stage Victory

---

## Difficulty Levels

| Stage | Rows | Columns | Display Time |
| ----- | ---- | ------- | ------------ |
| 1     | 10   | 2       | 1.0 s        |
| 2     | 10   | 3       | 0.75 s       |
| 3     | 15   | 7       | 0.5 s        |
| 4     | 15   | 12      | 0.3 s        |

---

## Technologies Used

* Verilog HDL
* Xilinx Vivado Design Suite
* Basys 3 FPGA Board
* Artix-7 Architecture
* Finite State Machines (FSM)
* Linear Feedback Shift Registers (LFSR)

---

## Learning Outcomes

This project provided practical experience in:

* FPGA-based system design
* Verilog HDL development
* Finite State Machine implementation
* Random number generation using LFSRs
* Hardware timing and synchronization
* Input debouncing techniques
* Seven-segment display multiplexing
* Real-time digital system integration

---

## Future Improvements

* Multiplayer gameplay mode
* Adaptive difficulty scaling
* Countdown timer challenges
* VGA graphical display output
* Audio feedback and sound effects
* Score tracking and leaderboard system

---

## Project Demonstration

This project was developed as part of the **Digital Logic Design Laboratory** coursework and successfully demonstrates how core digital logic concepts can be integrated into a complete hardware-based gaming application.

---

## Author

**Md Atif Absar** & **Agomon Das Dhrubo**
Computer Science & Engineering (CSE)
Khulna University of Engineering & Technology (KUET)

GitHub: https://github.com/atifabsar007
