# VHDL Counter Overflow Bug

This repository demonstrates a subtle bug in a simple VHDL counter. The counter overflows incorrectly, leading to unexpected behavior. The bug lies in how the counter handles the case where it reaches its maximum value.  The solution shows how to correctly reset the counter to 0. 

## Bug Description

The `buggy_counter.vhdl` file contains a VHDL counter that increments on each rising clock edge.  When the counter reaches its maximum value (15), it should reset to 0. However, there's a logic error that causes it to incorrectly remain at 15. 

## Solution

The `fixed_counter.vhdl` file provides the corrected code. The fix involves ensuring that the counter correctly resets to 0 when it reaches its maximum value. 

## How to Reproduce

1.  Simulate `buggy_counter.vhdl` using your favorite VHDL simulator (e.g., ModelSim, GHDL).
2. Observe that the counter gets stuck at 15 and never resets to 0.
3. Simulate `fixed_counter.vhdl` to see the corrected behavior. 