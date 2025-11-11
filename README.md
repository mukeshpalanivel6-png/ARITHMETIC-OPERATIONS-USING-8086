# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

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
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
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
![WhatsApp Image 2025-11-11 at 19 59 44_d930639e](https://github.com/user-attachments/assets/7c93f4f2-e0d9-428d-ad8d-47e15924ed25)


---

## OUTPUT IMAGE FROM MASM SOFTWARE

![WhatsApp Image 2025-09-22 at 13 09 55_e757caf6](https://github.com/user-attachments/assets/e504973d-ee73-4bf2-98d4-79d2b7c6993e)

## 2. SUBTRACTION

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
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
SUB AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
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
![WhatsApp Image 2025-11-11 at 19 59 47_91628f93](https://github.com/user-attachments/assets/4c127b5c-a754-405b-a6c6-da8d7ad3920c)

(Add your calculation here)





## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-09-22 at 13 09 15_ff1a7271](https://github.com/user-attachments/assets/597bd091-38e7-4e24-a5e3-21deb15c5d6a)

## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
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
![WhatsApp Image 2025-11-11 at 20 05 06_91d1f8a6](https://github.com/user-attachments/assets/7245d10d-b8e1-482a-8eef-c3ad2d0a4c64)

(Add your calculation here)

---


## OUTPUT SCREEN FROM MASM SOFTWARE

![WhatsApp Image 2025-10-29 at 16 31 18_24c71f18](https://github.com/user-attachments/assets/57110235-d14c-4d39-a2b4-1062ed1bfb90)

## 4. DIVISION

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
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
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

![WhatsApp Image 2025-11-11 at 20 10 23_7754b22a](https://github.com/user-attachments/assets/1a4b5c0b-3f5f-4874-b059-104d4a342d46)

(Add your calculation here)


---
## OUTPUT FROM MASM SOFTWARE

![WhatsApp Image 2025-10-29 at 16 53 02_daec1455](https://github.com/user-attachments/assets/536bd11f-1749-40a7-9411-db67e5dd8164)


## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

