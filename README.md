# D-FLIPDLOP-NEGEDGE

*AIM:*

To implement  D flipflop using verilog and validating their functionality using their functional tables

*SOFTWARE REQUIRED:*

Quartus prime

*THEORY*

*D Flip-Flop*

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

*Procedure*

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

*PROGRAM*
Program for flipflops and verify its truth table in quartus using Verilog programming.
## Developed by: RAJKUMAR T
## RegisterNumber:212224040263
verilog

module D_FF(D,Clock,reset,Q);
input D,Clock,reset;
output reg Q;
always@(negedge Clock)//use negative edge clock for triggering condition
if(!reset)
Q<=0;
else
Q<=D;
endmodule



*RTL LOGIC FOR FLIPFLOPS*

![328371883-f5eba0a8-c79f-4887-92da-60ad8c959e61](https://github.com/Charanteja-01/D-FLIPDLOP-NEGEDGE/assets/145693038/badf39b7-7346-4433-8653-5cecd31c27ea)


*TIMING DIGRAMS FOR FLIP FLOPS*

![328371899-5f087c34-9bb3-43c4-a83b-83be5815a3ad](https://github.com/Charanteja-01/D-FLIPDLOP-NEGEDGE/assets/145693038/64def090-be24-47b2-a8ab-044c192818c4)


*RESULTS*
Thus the program to implement a D flipflop using verilog and validating their functionality using their functional tables.
