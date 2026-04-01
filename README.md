 WHILE Language Compiler – Infinite Loop Detector


This project implements a **WHILE language compiler simulator** that demonstrates all major compiler phases and detects infinite loops using static analysis.

---

🎯 Aim
To design and implement a compiler for a WHILE language that:
- Simulates all compiler phases
- Detects infinite loops during semantic analysis

---

 ⚙️ Features
- Lexical Analysis (Tokenization)
- Syntax Analysis (Parsing & AST)
- Semantic Analysis
- Intermediate Representation (IR)
- Control Flow Graph (CFG)
- Loop Analysis
- Infinite Loop Detection
- Visual Report Generation



## 🧠 How It Works
1. Input program is given in WHILE language  
2. Lexer converts code into tokens  
3. Parser builds Abstract Syntax Tree (AST)  
4. Semantic analysis checks logic  
5. IR and CFG are generated  
6. Loop analysis detects infinite loops  
7. Final report is displayed  



## 🧪 Test Cases

### TC-1: Classic Case
i = 1;
while (i >= 10) goto L2;
TC-2: Safe Loop

Loop terminates correctly.

TC-3: Infinite Loop
x = 1;
while (x > 0) {
    x = x + 1;
}
TC-4: Dead Modifier
k = 10;
while (k != 0) {
    m = k * 2;
    k = k;
}
TC-5: Nested Loop

Inner loop terminates and outer loop is safe.

🔍 Infinite Loop Detection

The compiler detects infinite loops by analyzing:

Loop condition variables
Variable updates inside the loop
Control flow (goto / loops)

📊 Output Types
Control flow generation using labels
Infinite loop detection report
