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

identity law

<img width="900" height="480" alt="image" src="https://github.com/user-attachments/assets/e62da25f-2398-4b85-acf3-5e168942ffca" />

NULL law

<img width="1034" height="573" alt="image" src="https://github.com/user-attachments/assets/1af28eed-c74d-4661-8d9b-d8e64194cde2" />

idempotent law


<img width="460" height="279" alt="image" src="https://github.com/user-attachments/assets/7a79a62e-7b15-4d7d-99d0-a5dababa8af4" />

complement law

<img width="497" height="275" alt="image" src="https://github.com/user-attachments/assets/0a0fe44f-2ca9-4d1e-a228-3b6ee6838a9e" />

Distributive law

<img width="1035" height="716" alt="image" src="https://github.com/user-attachments/assets/4646f65f-8dc7-473e-bb75-0e6ea1978bfc" />

De-morgan's law

<img width="1036" height="538" alt="image" src="https://github.com/user-attachments/assets/46204424-8bbd-441f-aca3-593a4545882c" />

Absorption law

<img width="433" height="158" alt="image" src="https://github.com/user-attachments/assets/ff3c0749-9bb3-4dbc-89d8-c93f52566ff3" />

Associative law

<img width="691" height="713" alt="image" src="https://github.com/user-attachments/assets/219672d0-1e11-4e8a-9efd-f40b0c588637" />

commutative law

<img width="684" height="766" alt="image" src="https://github.com/user-attachments/assets/8d837ac6-3425-4c62-ad2f-fee60fd9d8e6" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**

**Output:**

<img width="1235" height="582" alt="image" src="https://github.com/user-attachments/assets/aa77e0d8-da95-497e-898c-cf6f8c395737" />


<img width="1201" height="577" alt="image" src="https://github.com/user-attachments/assets/4eb60c3a-b10b-4fee-8d2e-694e1f7e8012" />



**RTL**

**Timing Diagram**

(i)<img width="1280" height="716" alt="image" src="https://github.com/user-attachments/assets/c610eb76-4bf3-49cb-9216-9c5d9d874bc7" />


(ii)<img width="1279" height="679" alt="image" src="https://github.com/user-attachments/assets/cefad552-5162-487b-ba85-eda4f8dede6d" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

