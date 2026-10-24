Stack – Matching Delimiters

Laboratory activity for Data Structures and Algorithms (BSIT) at Ramon Magsaysay Memorial Colleges.

Programmed by: Kristel Protacio
Course: BSIT
CN: 48079
Subject: CC104

Description

This Java program uses a stack to check whether delimiters in a user-entered sequence are properly matched. It supports parentheses (), square brackets [], and curly braces {}.

The program follows the Last-In, First-Out (LIFO) principle to check the order of opening and closing delimiters. It identifies mismatched delimiters, closing delimiters without an opening delimiter, and opening delimiters that remain unmatched after the sequence is processed.

Files

File

Purpose

DelimiterChecker.java

Checks whether the entered sequence is valid or invalid.

DelimiterCheckerTrace.java

Displays the stack operations and stack contents during delimiter checking.

README.md

Contains the project description, instructions, sample outputs, and test cases.

How It Works

Push: Adds an opening delimiter to the stack.

Peek: Checks the delimiter at the top of the stack.

Pop: Removes the top delimiter when it matches the closing delimiter.

isEmpty: Checks whether any unmatched opening delimiters remain.

A sequence is valid when every opening delimiter has a matching closing delimiter in the correct order and the stack is empty at the end.

How to Run

Make sure Java is installed on your computer. Open a terminal in the folder containing the Java files.

To compile and run the main program:

javac DelimiterChecker.java
java DelimiterChecker

To compile and run the program with the stack execution trace:

javac DelimiterCheckerTrace.java
java DelimiterCheckerTrace

Enter a sequence when prompted and press Enter.

Sample Output

Valid Input

Enter a sequence: ({[]})
Valid

Invalid Input

Enter a sequence: {[(])}
Invalid: mismatched delimiters. ']' does not match '(' at the top of the stack.

Test Cases

Input

Expected Result

()

Valid

()[]{}

Valid

{[()]}

Valid

({[]})

Valid

{[(])}

Invalid

([)]

Invalid

{[()]

Invalid

{[()]}]

Invalid

Empty input

Valid

((a+b)*[c-d])

Valid

Acknowledgements

OpenAI ChatGPT (GPT-6) assisted with code drafting and explanations.

Prompt: Help me complete the Stack - Matching Delimiters activity.
