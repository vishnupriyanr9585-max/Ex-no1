# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION
<img width="611" height="426" alt="EX 1 ADD" src="https://github.com/user-attachments/assets/e2140051-e598-4a33-8a9c-5514d51412af" />

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />

#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,124H
ADD AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI], AX
MOV [SI+2], CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|       1200🔢       01         12

|         1200                    |

#### Manual Calculations
![WhatsApp Image 2026-02-02 at 11 31 02 AM (1)](https://github.com/user-attachments/assets/703a9016-179e-45d5-834e-3456d68d31ae)

---

## OUTPUT IMAGE FROM MASM SOFTWARE

## 2. SUBTRACTION
<img width="638" height="427" alt="ex 2 sub" src="https://github.com/user-attachments/assets/b616df60-fbc3-406e-b790-166093eda6b3" />

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program
```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,124H
SUB AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI], AX
MOV [SI+2], CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```


#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations
![WhatsApp Image 2026-02-02 at 11 31 02 AM](https://github.com/user-attachments/assets/167909e0-b26c-45a0-8dfe-ac77c457eb49)

---


## OUTPUT SCREEN FROM MASM SOFTWARE

## 3. MULTIPLICATION
<img width="637" height="418" alt="ex 3 mul" src="https://github.com/user-attachments/assets/e52cc22e-d410-4744-8a68-1b282f14407e" />

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm

```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

(Add your calculation here)

---CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,124H
MUL AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI], AX
MOV [SI+2], CL
MOV AH,4CH
INT 21H
CODE ENDS
END

## OUTPUT SCREEN FROM MASM SOFTWARE

## 4. DIVISION
<img width="635" height="422" alt="ex 4 div" src="https://github.com/user-attachments/assets/2e096a26-6e26-4551-92de-6bf2dd8f2992" />

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,124H
DIV AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI], AX
MOV [SI+2], CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

(Add your calculation here)

---
## OUTPUT FROM MASM SOFTWARE



## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

