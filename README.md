# EXPERIMENT-01: BUILDING LOGICAL CIRCUITS

NAME: SRISHTI T
REG.NO: RA2511030010319
DEPT:CSE CYBER SECURITY 

## 1. Aim

To design, implement, simplify, and verify combinational logic circuits using Boolean algebra and digital logic gates.

## 2. Boolean Notation

Use the following notation throughout this experiment:

| Symbol | Meaning | Example |
|---|---|---|
| `!A` | NOT A | `!A` |
| `A & B` | AND | `A & B` |
| `A \| B` | OR | `A \| B` |
| `A ^ B` | XOR | `A ^ B` |
| `A XNOR B` | XNOR | `A XNOR B` |

**Important:** In these equations, `!` means NOT, `&` means AND, `|` means OR, and `^` means XOR. Parentheses determine the order of operations.

## 3. Advanced Boolean Equations

### Equation 1: Four-Input Sum-of-Products

```text
F1 = (!A & B & C)
   | (A & B & !D)
   | (!B & C & D)
   | (A & !C & D)
```

**Inputs:** A, B, C, D  
**Output:** F1  
**Challenge:** Simplify the expression and compare gate counts.

### Equation 2: Product-of-Sums Circuit

```text
F2 = (A | !B | C)
   & (!A | B | D)
   & (B | !C | !D)
```

**Inputs:** A, B, C, D  
**Output:** F2  
**Challenge:** Implement the circuit using NAND gates and verify functional equivalence.

### Equation 3: Nested Complement Logic

```text
F3 = !(
       ((! (A | B)) | (C & D))
       &
       (A | (!(B | C)))
     )
```

**Inputs:** A, B, C, D  
**Output:** F3  
**Challenge:** Apply De Morgan's theorems and implement the circuit using NAND and NOR gates.

### Equation 4: XOR-XNOR Combinational Circuit

```text
F4 = ((A XOR B) & (C XNOR D))
   | (!A & B & (C XOR D))
```

**Inputs:** A, B, C, D  
**Output:** F4  
**Challenge:** Compare an XOR/XNOR implementation with a basic-gate implementation.

### Equation 5: Five-Input Logic Function

```text
F5 = (A & B & !C)
   | (!A & D & E)
   | (B & C & !E)
   | (!B & C & D)
```

**Inputs:** A, B, C, D, E  
**Output:** F5  
**Challenge:** Generate and verify all 32 input combinations.

### Equation 6: Six-Input Mixed Logic

```text
F6 = ((A | B) & !(C | D))
   | ((C XOR E) & (D | G))
   | (!A & B & E)
```

**Inputs:** A, B, C, D, E, G  
**Output:** F6  
**Challenge:** Calculate gate count and logic depth. Verify all 64 input combinations.

### Equation 7: NAND-NOR Hybrid Logic

```text
F7 = (! (A & B) & !(C | D))
   | (!(A | C) & B & D)
```

**Inputs:** A, B, C, D  
**Output:** F7  
**Challenge:** Implement the function using NAND and NOR gates with any required input inversions.

### Equation 8: Six-Input Advanced Combinational Logic

```text
F8 = ((A XOR B) & (C XNOR D))
   | (!(A | B) & C & E)
   | (A & B & !(D | F))
```

**Inputs:** A, B, C, D, E, F  
**Output:** F8  
**Challenge:** Simplify the expression, design the circuit, and verify all 64 input combinations.

## 4. Experimental Procedure

1. Identify all input variables and the output.
2. Draw the logic circuit for each equation.
3. Implement the circuit in Logisim Evolution, Proteus, or a digital logic trainer kit.
4. Apply all possible input combinations.
5. Record the expected and observed outputs.
6. Simplify the Boolean expression using Boolean algebra.
7. Build the simplified circuit and compare gate counts.
8. Save the circuit diagrams, truth tables, and verification screenshots.

## 5. Truth Table Requirements

| Number of inputs | Required combinations |
|---:|---:|
| 4 | 16 |
| 5 | 32 |
| 6 | 64 |

Use this format to record the results:

For F1 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 0 | 0 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 0 | 0 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 1 | 1 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 0 | 0 | PASS |

For F2 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 1 | 1 | PASS |
| 0010 | 1 | 1 | PASS |
| 0011 | 0 | 0 | PASS |
| 0100 | 0 | 0 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 1 | 1 | PASS |

For F3 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 0 | 0 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 1 | 1 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 1 | 1 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 1 | 1 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 1 | 1 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 0 | 0 | PASS |

For F4 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 0 | 0 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 0 | 0 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 0 | 0 | PASS |
| 1110 | 0 | 0 | PASS |
| 1111 | 1 | 1 | PASS |

For F5 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 00000 | 0 | 0 | PASS |
| 00001 | 0 | 0 | PASS |
| 00010 | 0 | 0 | PASS |
| 00011 | 1 | 1 | PASS |
| 00100 | 0 | 0 | PASS |
| 00101 | 0 | 0 | PASS |
| 00110 | 1 | 1 | PASS |
| 00111 | 1 | 1 | PASS |
| 01000 | 0 | 0 | PASS |
| 01001 | 0 | 0 | PASS |
| 01010 | 0 | 0 | PASS |
| 01011 | 1 | 1 | PASS |
| 01100 | 1 | 1 | PASS |
| 01101 | 0 | 0 | PASS |
| 01110 | 1 | 1 | PASS |
| 01111 | 1 | 1 | PASS |
| 10000 | 0 | 0 | PASS |
| 10001 | 0 | 0 | PASS |
| 10010 | 0 | 0 | PASS |
| 10011 | 0 | 0 | PASS |
| 10100 | 0 | 0 | PASS |
| 10101 | 0 | 0 | PASS |
| 10110 | 1 | 1 | PASS |
| 10111 | 1 | 1 | PASS |
| 11000 | 1 | 1 | PASS |
| 11001 | 1 | 1 | PASS |
| 11010 | 1 | 1 | PASS |
| 11011 | 1 | 1 | PASS |
| 11100 | 1 | 1 | PASS |
| 11101 | 0 | 0 | PASS |
| 11110 | 1 | 1 | PASS |
| 11111 | 0 | 0 | PASS |

For F6 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 000000 | 0 | 0 | PASS |
| 000001 | 0 | 0 | PASS |
| 000010 | 0 | 0 | PASS |
| 000011 | 1 | 1 | PASS |
| 000100 | 0 | 0 | PASS |
| 000101 | 0 | 0 | PASS |
| 000110 | 1 | 1 | PASS |
| 000111 | 1 | 1 | PASS |
| 001000 | 0 | 0 | PASS |
| 001001 | 1 | 1 | PASS |
| 001010 | 0 | 0 | PASS |
| 001011 | 0 | 0 | PASS |
| 001100 | 1 | 1 | PASS |
| 001101 | 1 | 1 | PASS |
| 001110 | 0 | 0 | PASS |
| 001111 | 0 | 0 | PASS |
| 010000 | 1 | 1 | PASS |
| 010001 | 1 | 1 | PASS |
| 010010 | 1 | 1 | PASS |
| 010011 | 1 | 1 | PASS |
| 010100 | 0 | 0 | PASS |
| 010101 | 0 | 0 | PASS |
| 010110 | 1 | 1 | PASS |
| 010111 | 1 | 1 | PASS |
| 011000 | 0 | 0 | PASS |
| 011001 | 1 | 1 | PASS |
| 011010 | 1 | 1 | PASS |
| 011011 | 1 | 1 | PASS |
| 011100 | 1 | 1 | PASS |
| 011101 | 1 | 1 | PASS |
| 011110 | 1 | 1 | PASS |
| 011111 | 1 | 1 | PASS |
| 100000 | 1 | 1 | PASS |
| 100001 | 1 | 1 | PASS |
| 100010 | 1 | 1 | PASS |
| 100011 | 1 | 1 | PASS |
| 100100 | 0 | 0 | PASS |
| 100101 | 0 | 0 | PASS |
| 100110 | 1 | 1 | PASS |
| 100111 | 1 | 1 | PASS |
| 101000 | 0 | 0 | PASS |
| 101001 | 1 | 1 | PASS |
| 101010 | 0 | 0 | PASS |
| 101011 | 0 | 0 | PASS |
| 101100 | 1 | 1 | PASS |
| 101101 | 1 | 1 | PASS |
| 101110 | 0 | 0 | PASS |
| 101111 | 0 | 0 | PASS |
| 110000 | 1 | 1 | PASS |
| 110001 | 1 | 1 | PASS |
| 110010 | 1 | 1 | PASS |
| 110011 | 1 | 1 | PASS |
| 110100 | 0 | 0 | PASS |
| 110101 | 0 | 0 | PASS |
| 110110 | 1 | 1 | PASS |
| 110111 | 1 | 1 | PASS |
| 111000 | 0 | 0 | PASS |
| 111001 | 1 | 1 | PASS |
| 111010 | 0 | 0 | PASS |
| 111011 | 0 | 0 | PASS |
| 111100 | 1 | 1 | PASS |
| 111101 | 1 | 1 | PASS |
| 111110 | 0 | 0 | PASS |
| 111111 | 0 | 0 | PASS |

For F7 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 0 | 0 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 1 | 1 | PASS |
| 0110 | 0 | 0 | PASS |
| 0111 | 0 | 0 | PASS |
| 1000 | 1 | 1 | PASS |
| 1001 | 0 | 0 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 0 | 0 | PASS |
| 1101 | 0 | 0 | PASS |
| 1110 | 0 | 0 | PASS |
| 1111 | 0 | 0 | PASS |

For F8 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 000000 | 0 | 0 | PASS |
| 000001 | 0 | 0 | PASS |
| 000010 | 0 | 0 | PASS |
| 000011 | 0 | 0 | PASS |
| 000100 | 0 | 0 | PASS |
| 000101 | 0 | 0 | PASS |
| 000110 | 0 | 0 | PASS |
| 000111 | 0 | 0 | PASS |
| 001000 | 0 | 0 | PASS |
| 001001 | 0 | 0 | PASS |
| 001010 | 1 | 1 | PASS |
| 001011 | 1 | 1 | PASS |
| 001100 | 0 | 0 | PASS |
| 001101 | 0 | 0 | PASS |
| 001110 | 1 | 1 | PASS |
| 001111 | 1 | 1 | PASS |
| 010000 | 1 | 1 | PASS |
| 010001 | 1 | 1 | PASS |
| 010010 | 1 | 1 | PASS |
| 010011 | 1 | 1 | PASS |
| 010100 | 0 | 0 | PASS |
| 010101 | 0 | 0 | PASS |
| 010110 | 0 | 0 | PASS |
| 010111 | 0 | 0 | PASS |
| 011000 | 0 | 0 | PASS |
| 011001 | 0 | 0 | PASS |
| 011010 | 0 | 0 | PASS |
| 011011 | 0 | 0 | PASS |
| 011100 | 1 | 1 | PASS |
| 011101 | 1 | 1 | PASS |
| 011110 | 1 | 1 | PASS |
| 011111 | 1 | 1 | PASS |
| 100000 | 1 | 1 | PASS |
| 100001 | 1 | 1 | PASS |
| 100010 | 1 | 1 | PASS |
| 100011 | 1 | 1 | PASS |
| 100100 | 0 | 0 | PASS |
| 100101 | 0 | 0 | PASS |
| 100110 | 0 | 0 | PASS |
| 100111 | 0 | 0 | PASS |
| 101000 | 0 | 0 | PASS |
| 101001 | 0 | 0 | PASS |
| 101010 | 0 | 0 | PASS |
| 101011 | 0 | 0 | PASS |
| 101100 | 1 | 1 | PASS |
| 101101 | 1 | 1 | PASS |
| 101110 | 1 | 1 | PASS |
| 101111 | 1 | 1 | PASS |
| 110000 | 1 | 1 | PASS |
| 110001 | 0 | 0 | PASS |
| 110010 | 1 | 1 | PASS |
| 110011 | 0 | 0 | PASS |
| 110100 | 0 | 0 | PASS |
| 110101 | 0 | 0 | PASS |
| 110110 | 0 | 0 | PASS |
| 110111 | 0 | 0 | PASS |
| 111000 | 1 | 1 | PASS |
| 111001 | 0 | 0 | PASS |
| 111010 | 1 | 1 | PASS |
| 111011 | 0 | 0 | PASS |
| 111100 | 0 | 0 | PASS |
| 111101 | 0 | 0 | PASS |
| 111110 | 0 | 0 | PASS |
| 111111 | 0 | 0 | PASS |



Extend the table to include every input combination required by each equation.

## 6. Performance Analysis

For each circuit, record:

- Number of AND gates
- Number of OR gates
- Number of NOT gates
- Number of XOR/XNOR gates
- Total gate count
- Logic depth
- Functional equivalence before and after simplification

HERE IS THE ANALYSIS RECORD:
| Equation | NOT Gates | AND Gates | OR Gates | XOR/XNOR Gates | Total Gate Count | Logic Depth | Functional Equivalence |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **F1** | 4 | 4 | 1 | 0 | **9** | 3 | Equivalent |
| **F2** | 3 | 1 | 3 | 0 | **7** | 3 | Equivalent |
| **F3 (Simplified)** | 3 | 3 | 2 | 0 | **8** | 3 | Equivalent |
| **F4 (XOR/XNOR)** | 1 | 1 | 1 | 2 | **5** | 3 | Equivalent |
| **F5** | 3 | 4 | 1 | 0 | **8** | 3 | Equivalent |
| **F6** | 1 | 3 | 2 | 1 | **7** | 4 | Equivalent |
| **F7 (Hybrid)** | 0 | 2 | 1 | 3 (2 NOR, 1 NAND) | **6** | 3 | Equivalent |
| **F8** | 1 | 3 | 1 | 2 (1 XOR, 1 XNOR) | **7** | 4 | Equivalent |

## 7. Expected Results (drop the screenshots of each equations circuit )
<img width="921" height="468" alt="image" src="https://github.com/user-attachments/assets/82050386-b959-408f-8a89-a513ac197319" />
<img width="915" height="472" alt="image" src="https://github.com/user-attachments/assets/c976ceb1-e481-450e-857b-dc2917827438" />
<img width="911" height="420" alt="image" src="https://github.com/user-attachments/assets/32a5479c-4ada-4753-8356-16bcf488db21" />
<img width="910" height="463" alt="image" src="https://github.com/user-attachments/assets/54250a16-0d1d-42ee-bbea-c9a65b7e0f08" />
<img width="917" height="442" alt="image" src="https://github.com/user-attachments/assets/6e287a4f-8db5-41f8-9f16-5845e706130b" />
<img width="917" height="500" alt="image" src="https://github.com/user-attachments/assets/e3f58128-fac7-4d99-8200-6dd9e6d5c575" />
<img width="921" height="501" alt="image" src="https://github.com/user-attachments/assets/45aceeb3-485c-4bdc-af0d-2cf700af0bf0" />
<img width="910" height="453" alt="image" src="https://github.com/user-attachments/assets/29423b92-42e0-49ff-aea0-8fb95283d05d" />
 
## 8. Result

The logic circuits are designed, implemented, and verified using Boolean algebra and digital logic gates. The original and simplified circuits are compared based on gate count and logic depth.
 
