# Stack - Matching Delimiters

Data Structures and Algorithms laboratory activity about using a stack to check matching delimiters.

## Description

This Java program checks whether parentheses (), square brackets [], and curly braces {} are properly matched and nested.

It uses the stack operations push, peek, pop, and isEmpty.

## Files

- DelimiterChecker.java - Checks whether a sequence is valid or invalid.
- DelimiterCheckerTrace.java - Displays the stack operations and stack contents.

## How to Run

Run either Java file using a Java IDE such as JCreator.

## Sample Output

Input:
({[]})

Output:
Valid

## Test Cases

| Input | Expected Result |
|---|---|
| () | Valid |
| ()[]{} | Valid |
| {[()]} | Valid |
| ({[]}) | Valid |
| {[(])} | Invalid |
| ([)] | Invalid |
| {[()] | Invalid |
| {[()]}] | Invalid |
| Empty input | Valid |
| ((a+b)*[c-d]) | Valid |
