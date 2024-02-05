## Two-Pass Assembler
This is a simple two-pass assembler written in Python that processes assembly language code and generates intermediate code. The assembler supports a set of predefined mnemonics and directives.

## Usage
Make sure you have Python installed on your system.
Save your assembly code in a file named input.txt in the same directory as the assembler script.
Run the assembler script.
bash
Copy code
python assembler.py
The intermediate code will be generated in the inter_code.txt file, and additional information such as the symbol table and pool table will be saved in SymTab.txt and PoolTab.txt, respectively.

## Supported Mnemonics and Directives
## Supported Mnemonics and Directives

- **Mnemonics:**
  - STOP
  - ADD
  - SUB
  - MUL
  - MOVER
  - MOVEM
  - COMP
  - BC
  - DIV
  - READ
  - PRINT

- **Directives:**
  - LTORG
  - ORIGIN
  - START
  - EQU
  - DS
  - DC
  - END

Input File
Ensure your assembly code is written in input.txt in the specified format. Labels, mnemonics, and operands should be separated by spaces.

## Intermediate Code
The generated intermediate code will be stored in ```inter_code.txt```. This file contains the processed instructions and their corresponding opcodes.

## Symbol Table
The symbol table (SymTab.txt) provides information about the symbols used in the assembly code, including their names and addresses.

## Pool Table
The pool table (PoolTab.txt) keeps track of the starting index of each literal pool. Literal pools are generated for the LTORG directive.

## Note
The assembler performs a two-pass scan of the input code to resolve symbols and generate the necessary tables.
The code handles basic mnemonics, directives, and identifies different types of operands (registers, literals, symbols).
Feel free to customize the assembler for your specific needs or extend its functionality based on your requirements.
