### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */
1. Type the program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations generate the timing diagram.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 
![Screenshot 2024-12-07 114434](https://github.com/user-attachments/assets/f60429e8-fe13-4c3c-959c-1d1b2075c5d6)

Developed by:G.Ramanujam

RegisterNumber:24000309
*/

**RTL LOGIC UP COUNTER**
![Screenshot 2024-12-07 114448](https://github.com/user-attachments/assets/c14bd1a5-d39d-4387-8c46-6264d80aece0)

**TIMING DIAGRAM FOR IP COUNTER**
![Screenshot 2024-12-07 115258](https://github.com/user-attachments/assets/dbc269ed-cc84-4d0d-a0b3-0ac1b5ba1e02)

**STATE DIAGRAM**
![Screenshot 2024-12-07 115644](https://github.com/user-attachments/assets/7bed0855-a9c6-4d2c-8630-3ed15588e07f)

**RESULTS**
Thus, the RTL Logic and Timing Digram for UP COUNTER has been verified and implemented
