# Stack – Matching Delimiters

Laboratory activity for **Data Structures and Algorithms** (BSIT) at Ramon Magsaysay Memorial Colleges.

**Programmed by:** Kristel Angel R. Protacio  
**Course:** BSIT  
**CN:** 48079  
**Subject:** CC104

## Description

This program uses a stack to check if delimiters in a user-entered sequence are properly matched. It supports parentheses `()`, square brackets `[]`, and curly braces `{}`.

The program follows the Last-In, First-Out (LIFO) principle. It checks whether each closing delimiter matches the most recent unmatched opening delimiter. It also detects mismatched delimiters and opening delimiters that remain unmatched at the end.

## Files

| File | Purpose |
|---|---|
| `DelimiterChecker.java` | Checks whether a sequence of delimiters is valid or invalid. |
| `DelimiterCheckerTrace.java` | Displays the stack operations and stack contents while checking a sequence. |
| `README.md` | Contains the project description, instructions, sample outputs, and test cases. |

## How It Works

- **Push:** Adds an opening delimiter to the stack.
- **Peek:** Checks the opening delimiter at the top of the stack.
- **Pop:** Removes the top delimiter when it matches the closing delimiter.
- **isEmpty:** Checks whether the stack is empty.

A sequence is valid if all delimiters are correctly matched and no opening delimiters remain in the stack after processing.

## How to Run

Make sure Java is installed on your computer. Open a terminal in the folder containing the Java files.

Compile and run the main program:

    javac DelimiterChecker.java
    java DelimiterChecker

Compile and run the stack trace program:

    javac DelimiterCheckerTrace.java
    java DelimiterCheckerTrace

Enter a sequence when prompted and press Enter.

## Sample Output

**Valid Input**

    Enter a sequence: ({[]})
    Valid

**Invalid Input**

    Enter a sequence: {[(])}
    Invalid: mismatched delimiters. ']' does not match '(' at the top of the stack.

## Test Cases

| Input | Expected Result |
|---|---|
| `()` | Valid |
| `()[]{}` | Valid |
| `{[()]}` | Valid |
| `({[]})` | Valid |
| `{[(])}` | Invalid |
| `([)]` | Invalid |
| `{[()]` | Invalid |
| `{[()]}]` | Invalid |
| Empty input | Valid |
| `((a+b)*[c-d])` | Valid |

## Acknowledgements

OpenAI ChatGPT (GPT-6) assisted with code drafting and explanations.

**Prompt:** Help me complete the Stack - Matching Delimiters activity.
