# VLSI / RTL Project Portfolio

A collection of digital design projects covering RTL design, protocol implementation,
verification, and physical design — built while progressing from core digital logic
toward SoC-level design and silicon submission.

## Projects

| # | Project | Description | Status |
|---|---------|-------------|--------|
| 01 | [8-bit ALU](./01-8bit-alu) | Arithmetic/logic unit, foundation module, taken through OpenLANE synthesis | ✅ Complete |
| 02 | [UART Tx/Rx](./02-uart-txrx) | UART transmitter/receiver, protocol proof of concept | ✅ Complete |
| 03 | [SPI Master](./03-spi-master) | SPI master supporting all 4 clock/phase modes | ✅ Complete |
| 04 | [FPGA PWM Controller](./04-fpga-pwm-controller) | PWM generator bridging RTL design to real FPGA hardware | ✅ Complete |
| 05 | [AXI4-Lite Slave](./05-axi4-lite-slave) | AXI4-Lite slave interface, SoC-level design differentiator | 🔧 In progress |
| 06 | [FIR Filter](./06-fir-filter) | Configurable FIR filter, DSP building block | 🔧 In progress |
| 07 | [SV Testbench (UART)](./07-sv-testbench-uart) | Class-based SystemVerilog verification environment | 🔧 In progress |
| 08 | [TinyTapeout Submission](./08-tinytapeout-submission) | RTL taped out to real silicon via TinyTapeout | 🚀 Planned |

## Toolchain

- **RTL / Simulation:** Verilog, SystemVerilog, Icarus Verilog / ModelSim
- **Synthesis / Physical Design:** OpenLANE (open-source RTL-to-GDSII flow)
- **FPGA target:** *(fill in your board, e.g. Basys3 / Nexys A7)*
- **Silicon:** TinyTapeout (Sky130 PDK)

## Repo structure

Each numbered folder is self-contained:
<project>/ ├── rtl/ → synthesizable design source ├── tb/ → testbenches ├── sim/ → simulation outputs (gitignored) └── README.md → module description, interface, how to run
## How to run a testbench (example)

```bash
cd 01-8bit-alu
iverilog -o sim/alu_tb tb/alu_8bit_tb.v rtl/alu_8bit.v
vvp sim/alu_tb
```

## Author

Animesh Kullu — B.Tech ECE, Jalpaiguri Government Engineering College
[LinkedIn](https://www.linkedin.com/in/animesh-kullu-91834b424)
