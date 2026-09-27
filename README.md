# FIR Filter Co-processor in VHDL (MAPD-A Final Project)

Final project for *Management and Analysis of Physics Datasets*, module A (M.Sc. Physics of Data,
University of Padova, 2023): a 4-tap FIR filter on an FPGA that receives 8-bit samples from a PC over
UART, filters them and sends the result back.

| File | Role |
|---|---|
| `top.vhd` | Top level (100 MHz board clock) |
| `uart_receiver.vhd`, `uart_transmitter.vhd` | UART state machines |
| `baudrate.vhd`, `sampler_generator.vhd` | Baud-rate generation (about 115 200 baud) |
| `my_fir.vhd`, `DFF.vhd` | 4-tap FIR filter with a D flip-flop delay line |
| `VHDL_generation_of_optimized_FIR_filters.pdf` | Reference paper (F. F. Daitx *et al.*) |

This is the first version of the project. The final version, with the design report, the assignment and
the lab exercises, is in [MAPD-mod_A](https://github.com/alireza-mollaalihosseini/MAPD-mod_A).
