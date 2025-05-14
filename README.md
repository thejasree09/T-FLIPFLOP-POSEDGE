# T-FLIPFLOP-POSEDGE

**AIM:**

To implement  T flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**T Flip-Flop**

T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/458a68fe-2d08-4a9d-ac4f-7ae0480ce0bd)

 
This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/cdd7fb32-539f-4b66-bb8d-f305a153c886)

 
From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

**Procedure**

Design the T flip-flop module in Verilog with inputs T, clk and outputs Q, Qbar.

Use always @(posedge clk) to toggle Q when T = 1, and retain Q when T = 0.

Develop a testbench to apply different T values synchronized with clock pulses.

Simulate the module and observe the outputs (Q, Qbar) at each clock edge.

Compare the simulated results with the T flip-flop truth table for validation.


**PROGRAM**

![program](https://github.com/user-attachments/assets/3b51a5a5-3c27-4a5a-865b-b0c86f762b46)


**RTL LOGIC FOR FLIPFLOPS**

![simulation](https://github.com/user-attachments/assets/0825c987-a5c7-4879-bbce-6dc9ce562fa3)

**TIMING DIGRAMS FOR FLIP FLOPS**

![waveform](https://github.com/user-attachments/assets/e686b9d4-3c2f-421b-a050-c51ec6274278)

**RESULTS**

The T flip-flop was successfully implemented and verified in Verilog, with outputs conforming to its functional truth table.
