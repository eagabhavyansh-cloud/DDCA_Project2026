# 4-Bit Binary to Hex Digit Display — DDCA Project

A simple digital logic circuit built in Logisim that takes a 4-bit binary input and displays its equivalent hex digit (0–F) on a seven-segment-style display.

## Team

- Guntaka Rishika (2620030103)
- Eaga Bhavyansh (2620030142)
- Keta Pravalika (2620030144)
- Kadiyam Jai Siva Sai Sri (2620030145)

**Course:** Digital Design & Computer Architecture (DDCA)
**Institution:** KLH
**Faculty:** L R Rahul

## Components Used

| Component | Category | Quantity | Settings |
|---|---|---|---|
| Input Pin | Wiring | 4 (B1–B4) | 1-bit wide, each toggles 0/1 |
| Splitter | Wiring | 1 | Fan Out = 4, Bit Width In = 4 — combines the 4 separate 1-bit inputs into a single 4-bit bus |
| Hex Digit Display | Input/Output | 1 | 4-bit input, decodes binary value and displays digit 0–F |

**Total components: 6**

## Circuit Design

The circuit consists of:

- **4 Input Pins (B1–B4)** — each a single-bit toggle switch, individually set to 0 or 1 by clicking it in Logisim.
- **1 Splitter** — merges the four individual 1-bit signals into one 4-bit bus so they can feed a single multi-bit input.
- **1 Hex Digit Display** — a built-in Logisim I/O component with a 4-bit input. It internally decodes any 4-bit binary value and lights up the correct segments to show the matching digit.

B1–B4 are wired into the Splitter, which combines them into a 4-bit bus feeding the Hex Digit Display (B1 = most significant bit, B4 = least significant bit). No hand-built logic gates or decoder are used — the Hex Digit Display component handles the binary-to-segment decoding internally.
