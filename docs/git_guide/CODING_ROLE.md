---
layout: default
title: CodingRole
parent: Git Guide
nav_order: 1
---


### 1. Coding principle
* In principle, comments should be described in detail in all codes.
* In principle, duplication of source code is prohibited except for inevitable content.
* All words used in the source code are based on the contents of the glossary.
* When developing and testing, pay special attention to security as well as function and performance.


### 2. Coding Style
* Coding style defines the rules for source development and aims to ensure standardization and consistency.

### 2.1 indent
* Indent does not use tabs, only spaces.
* The size of indent is set to 4.

### 2.2 space
* Only one statement is described per line.
* Leave a space after semicolon, comma, and reserved words.
* Unary operation does not leave a space. (ex. i++;)
* Binary operation has a space on both sides. (ex. i = i + 1;)
* If there are parentheses in parentheses, use them without spaces between the parentheses.

### 2.3 brace
* ‘{’ and ‘}’ are written on a new line, not together with other contents. (Excluding comments)
*'{' uses indent(4-space) compared to the existing'{'.
* ‘}’ uses indent(4-space) in the same way as ‘{’
* When writing comments on the brace, use ‘//’ comments.

### 2.4 Terminology
* As for terms, in principle, follow the glossary and use English that matches the term.
* When using one word, use English terms.
* When using multiple words in combination, use the combination of English abbreviations.
* Pay attention to homophones when using terms.
* The system code to be used is defined in 3 letters in English as follows.

### 2.5 Logging
* Log is used by distinguishing debug, info, warn, and error.
* Log must include the time, location and contents of the occurrence.
* Log outputs only one line (except debug log).
* Debug log is used only during development, not during operation.
* The info log records contents that will be helpful to the operator.
* The warn log is not an error, but records the possible occurrence of potential errors.
* The error log records the contents of the error along with the error code.
 
### 2.6 File Name and Line
* The file name should not exceed 50 characters.
* The file name is written based on the contents of the glossary, and special symbols and numbers are not used.


### 3. UI
* In principle, use absolute path.
* Under sub-system, the directory consists of 3-level or less.
* Files are located only in the lowest directory.
* The system name and sub-system name should be written in 3 letters as possible by combining the first letter of the term English name or English abbreviation name, but not more than 6 letters.
* Use only lowercase letters for the system name and sub-system name used in the directory.
