# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit, leading to more efficient, faster, and less costly hardware for minimizing Boolean expressions,we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.

Identity Law A ⋅ 1 = A, A + 0 = A Null Law A ⋅ 0 = 0, A + 1 = 1 Idempotent Law A ⋅ A = A, A + A = A Complement Law A ⋅ A′ = 0, A + A' = 1 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′ Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C Commutative law A B = B A,A + B = B + A

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
module boolean_function_4var (
    input  wire A,
    input  wire B,
    input  wire C,
    input  wire D,
    output wire F
);

assign F = (~A & B) | (C & D) | (A & ~D);

endmodule

```

Developed by:Bhuvanesh S  RegisterNumber:25017596


**RTL realization**

**Output:**

![WhatsApp Image 2025-11-22 at 14 50 14_1bd5e836](https://github.com/user-attachments/assets/19cdbf9d-aeea-40c7-967f-ca6e3dbba08d)

**RTL**

**Timing Diagram**

![WhatsApp Image 2025-11-22 at 14 48 27_b9fbcd34](https://github.com/user-attachments/assets/c0c0f5bb-8117-405d-895f-2a68c46e22cb)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

