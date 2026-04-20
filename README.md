 Main Features

✔ 32-bit addition with carry detection
✔ 32-bit subtraction with borrow detection
✔ Full 32×32 → 64-bit multiplication
✔ 32-bit ÷ 16-bit division (8086 DIV compliant)
✔ Hexadecimal input/output formatting
✔ Internal flag analysis (Carry & Borrow)
✔ Real-time output visualization
✔ Error handling (e.g., division by zero)
✔ Text-based User Interface (DOS-Style)
✔ Fully compatible with EMU8086 simulator

 Tech Stack / Tools

EMU8086

Assembly Language (x86)

Real-mode 16-bit Execution Model

DOS Interrupts (INT 21h / INT 10h)

 How It Works (Program Flow)

User enters two 32-bit numbers as HIGH + LOW hex words

User selects an operation from the menu:

ADD

SUB

MUL

DIV

ANALYZE

CPU performs the operation

Results are displayed in suitable format:

32-bit → res1:res0

64-bit (MUL) → res3:res2:res1:res0

Flags such as Carry or Borrow are evaluated and printed

User may repeat operations without restarting

🛠 Installation & Setup
1. Download EMU8086 from: https://emu8086.com
2. Clone this repository:
   git clone https://github.com/<your-username>/<repository-name>.git
3. Open EMU8086 and load the .asm file
4. Assemble & run (Make EXE)

🧪 Input Format

Each 32-bit number is entered as:

HIGH (4 hex digits)
LOW  (4 hex digits)


Example:

NUM1 HIGH = 1234
NUM1 LOW  = 5678
NUM2 HIGH = 0000
NUM2 LOW  = 8000

📤 Output Format

Depending on the operation:

✔ ADD / SUB / DIV → 32-bit output:
0xHHHHLLLL

✔ MUL → 64-bit output:
0xHHHHHHHHLLLLLLLL


(Mapped to res3:res2:res1:res0)

 📌 Use Cases

Computer architecture education

Microprocessor labs (8086 / x86)

Understanding CPU flags

Teaching low-level arithmetic

Debugging 8086 assembly
