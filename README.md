# I²C Communication Protocol in Verilog

A complete implementation of the **I²C (Inter-Integrated Circuit) protocol** designed in **Verilog HDL**, featuring both **Master** and **Slave** modules.  
This project fully supports **read/write operations**, **7-bit addressing**, **ACK/NACK handling**, and **accurate START/STOP condition generation**.

All modules are verified with a structured **testbench** and **waveform simulations** to ensure protocol-accurate timing and behavior.

## 🚀 Features

### ✅ **I²C Master Module**
- START and STOP condition generation  
- 7-bit addressing with R/W bit  
- ACK/NACK detection  
- SCL clock generation (100 kHz from 40 MHz system clock)  
- Tri-state SDA driver  
- Byte-level read/write sequencing  
- Master-side NACK generation after read completion  

### ✅ **I²C Slave Module**
- Address recognition (configurable address)  
- ACK generation for address & data  
- Data storage memory (128-byte array)  
- Supports read & write operations  
- Timing-aligned SDA response  
- STOP detection and transaction completion  

### ✅ **Testbench**
- Master → Slave write operation  
- Master → Slave read operation  
- START/STOP validation  
- ACK/NACK verification  
- Full waveform inspection  
- Timing compliance checks  

---

## 🧪 Simulation

The protocol was verified using:

- START → Address → ACK → Write → ACK → STOP  
- START → Address → ACK → Read → NACK → STOP  
- Full waveform inspection  
- SDA/SCL edge timing validation  
- Tri-state SDA correctness  

Waveforms confirm **complete I²C protocol compliance**.

---

## 🔧 Tools Used

- **Verilog HDL**
- ** Vivado Simulator**
- **FPGA Design Flow**

---

## 📎 Repository Purpose

This project is intended for:

- FPGA learners  
- Digital design students  
- Protocol design practice  
- RTL design and verification training  
- Communication interface understanding  

---

