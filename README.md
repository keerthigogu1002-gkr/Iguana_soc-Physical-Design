# Iguana_SoC Physical Design

## Project Overview

RTL-to-GDSII implementation of Iguana_SoC using Synopsys Design Compiler (DC) and Synopsys IC Compiler II (ICC2).

## Tools and Technologies

- Synopsys Design Compiler
- Synopsys IC Compiler II (ICC2)
- Verilog/SystemVerilog
- TCL
- Linux

## Physical Design Flow

RTL
→ Synthesis
→ Floorplanning
→ Macro Placement
→ Power Planning
→ Placement
→ Clock Tree Synthesis (CTS)
→ Routing
→ Post-Route Optimization
→ Timing Analysis
→ Physical Verification
→ GDSII

## Repository Structure

```text
Iguana_soc-Physical-Design/
├── README.md
├── rtl/
├── constraints/
├── scripts/
│   ├── dc/
│   └── icc2/
├── reports/
├── results/
└── screenshots/
```

## Implementation Stages

### 1. Synthesis
RTL is synthesized using Synopsys Design Compiler to generate a gate-level netlist.

### 2. Floorplanning
Core area, utilization, aspect ratio, IOs, and macro locations are defined.

### 3. Macro Placement
Hard macros are placed and optimized for timing and congestion.

### 4. Power Planning
Power rings, straps, and standard-cell power connections are implemented.

### 5. Placement
Standard cells are placed and optimized for timing, congestion, and legality.

### 6. Clock Tree Synthesis
Clock trees are synthesized and optimized for skew, latency, and timing.

### 7. Routing
Signal and clock nets are routed followed by route optimization.

### 8. Post-Route Analysis
Setup, hold, clock skew, congestion, DRC, and other physical/timing checks are performed.

### 9. Signoff
Final timing and physical verification are performed before GDSII generation.

## Results

The following results will be documented after implementation:

- Area
- Utilization
- Setup WNS/TNS
- Hold WNS/TNS
- Clock skew
- Clock latency
- Congestion
- DRC violations
- Power

## Author

Gogu Keerthi Reddy
