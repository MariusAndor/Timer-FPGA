# FPGA - Timer
### Xilinx FPGA Timer — Verilog HDL

A hardware timer implemented on an FPGA board that counts seconds and minutes using the board's 50 MHz processor clock, displaying the output on a seven-segment display.

---

### What it does

- Counts seconds and minutes in real time
- Displays output on the onboard seven-segment display
- Uses clock division to derive a 1 Hz signal from the 50 MHz system clock
- Implemented entirely in Verilog HDL

---

### How it works

The 50 MHz clock is divided down to 1 Hz using a counter. A state machine tracks seconds (0–59) and minutes (0–59), incrementing each value at the correct interval. The output is encoded and sent to the seven-segment display driver.

```
50 MHz clock → Clock Divider → 1 Hz signal → Counter (ss:mm) → 7-seg Display
```

---

### Tech Stack

- **Language:** Verilog HDL
- **Board:** Xilinx FPGA
- **Display:** Seven-segment display
- **Clock:** 50 MHz system clock

---

### What I learned

- Clock division and timing in hardware
- State machine design in Verilog
- Seven-segment display encoding
- How to think about time constraints at the hardware level


