# -COMPILER-DESIGN-BASICS  
*COMPANY*: CODTECH IT SOLUTIONS PVT.LTD
**NAME*: SHAHIL MURMU
*INTERN ID*: CT04DF2444
*DOMAIN*: C LANGUAGE
*DURATION*: 4 WEEKS
*MENTOR*: NEELA SANTOSH KUMAR
#Task 3 Description – Lexical Analyzer Implementation in C

Task 3 involves building a basic Lexical Analyzer using the C programming language. This task introduces one of the fundamental concepts in compiler design: the lexical analysis phase. The lexical analyzer, also known as a scanner or tokenizer, is the first stage of a compiler that reads the source code and breaks it down into meaningful units called tokens. These tokens are classified into types such as keywords, identifiers, operators, constants, and more.

In this particular task, the objective was to design a simple program that can recognize and classify keywords, identifiers, and operators from a single line of source code entered by the user. The user is prompted to input a line of C code, and the program scans each character to determine the appropriate classification for each token it encounters.

The implementation begins with the declaration of a list of predefined keywords such as "int", "float", "if", "else", "while", "for", and "return". These are stored in a 2D character array for comparison during lexical analysis. Additionally, a character array is used to define valid operators, including symbols like +, -, *, /, =, <, and >.

Two helper functions are defined:

1. isKeyword(char *word) – This function checks if a given string matches any of the known keywords. If a match is found, it returns 1 (true); otherwise, it returns 0.


2. isOperator(char ch) – This function checks if a character is one of the predefined operators. It iterates through the operators array and returns 1 if a match is found.



The main function handles the lexical scanning process. It starts by accepting a single line of C code from the user using fgets(). It then scans each character using a loop. If a character is alphanumeric (i.e., a letter or digit), it is assumed to be part of a word or identifier and is stored in a temporary buffer called word. When a non-alphanumeric character is encountered, the buffered word is terminated and passed through the isKeyword() function to determine whether it is a keyword or an identifier. If the character itself is an operator, it is printed as an operator token.

To ensure proper token recognition at the end of the input string, a final check is made after the loop to process any remaining word stored in the buffer. This guarantees that all tokens are identified, even if they appear at the very end of the input line.

This program, although basic, accurately reflects how lexical analysis is performed in real-world compilers. It breaks down complex source code into recognizable parts, forming the groundwork for the syntax analysis (parsing) and semantic analysis stages that follow.

Through this task, the intern gains hands-on experience with:

Tokenization techniques

String manipulation in C

Use of character functions like isalnum()

Arrays and string comparisons using strcmp()

Understanding of compiler phases


The program is designed in a modular, easy-to-understand format that emphasizes clarity and logical flow. Its functionality can be expanded further by including support for:

Numbers and constants

Special characters

Multi-character operators (==, <=, !=, etc.)

Comments and whitespace handling


This task also emphasizes the importance of compiler design in software development, especially for developers interested in programming languages, interpreters, or building tools like IDEs and static code analyzers.

In conclusion, this lexical analyzer project serves as an essential step in grasping how high-level code is broken into basic components before actual compilation. It helps students and beginners appreciate the lower-level functioning of a compiler while reinforcing concepts of string processing and decision-making logic in C.
#OUTPUT: 

