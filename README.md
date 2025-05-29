Compiler Design Project
This project implements a simple compiler in multiple phases, from lexical analysis to code optimization. Each phase corresponds to a standard component in the compiler design pipeline.

📁 Project Structure
bash
Copy
Edit
├── Phase_1/                      # Lexical Analysis
├── Phase_2_AST/                 # Abstract Syntax Tree (AST) Construction
├── Phase_3_ICG/                 # Intermediate Code Generation
├── Phase_4_CodeOptimization/   # Code Optimization
├── inputfile.cpp               # Sample source code for compilation
🔍 Phase 1 - Lexical Analysis
Goal: Tokenize the input source code into meaningful lexemes.

Tools: Custom C++ lexer or Lex (flex).

Output: List of tokens with their types and lexemes.

🌲 Phase 2 - AST (Abstract Syntax Tree)
Goal: Parse the tokens and construct an AST.

Tools: Recursive descent parser or Yacc (bison).

Output: Tree representation of the program showing grammatical structure.

⚙️ Phase 3 - Intermediate Code Generation (ICG)
Goal: Convert AST to intermediate representation (IR), such as Three Address Code (TAC).

Output: IR that can be used for optimization and translation to machine code.

🚀 Phase 4 - Code Optimization
Goal: Improve the intermediate code by applying optimizations like:

Constant Folding

Dead Code Elimination

Common Subexpression Elimination

Output: Optimized IR.

📄 inputfile.cpp
Sample C++ file that is used as input for lexical and syntactic analysis.

✅ How to Run
Compile the lexer/parser and run each phase separately:

bash
Copy
Edit
g++ Phase_1/lexer.cpp -o lexer
./lexer inputfile.cpp
For AST and further phases, follow the compilation instructions inside each folder’s README (if available) or run using:

bash
Copy
Edit
g++ Phase_2_AST/parser.cpp -o parser
./parser
🧑‍💻 Authors
Rajeev Ranjan (Assumed from project)

[Add your teammates if any]

📚 References
Aho, Lam, Sethi, and Ullman — Compilers: Principles, Techniques, and Tools

Compiler Explorer

Flex/Bison Documentation
