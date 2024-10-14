---
tags:
  - note
  - inti
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Internet, Fundamental of Data, and Signal]]"
---

# Data Codes

Data codes are essential for representing textual characters in digital form, enabling computers and electronic devices to communicate effectively. The three most common data codes are **EBCDIC**, **ASCII**, and **Unicode**. Each of these codes has its unique characteristics, applications, and limitations.

## EBCDIC (Extended Binary Coded Decimal Interchange Code)

### Overview
- EBCDIC is an 8-bit character encoding system developed by IBM in the 1960s. It was primarily used in mainframe and midrange computer systems.
- EBCDIC supports 256 different characters, including uppercase and lowercase letters, numbers, punctuation marks, and control characters.

### Characteristics
- **Character Set:** EBCDIC includes control characters similar to ASCII but organizes them differently. It also provides additional characters that are not available in ASCII.
- **Usage:** While EBCDIC was widely used in IBM systems, its adoption has declined with the rise of ASCII and Unicode. It is still found in legacy systems and certain industries like banking and finance.

### Applications
- Primarily used in IBM mainframe environments.
- Legacy applications that require compatibility with older systems may still utilize EBCDIC.

## ASCII (American Standard Code for Information Interchange)

### Overview
- ASCII is a 7-bit character encoding standard that represents text in computers, telecommunications equipment, and other devices. It was developed in the early 1960s.
- ASCII defines 128 unique characters, including letters (both uppercase and lowercase), digits (0-9), punctuation marks, and control characters.

### Characteristics
- **Character Set:** The first 32 characters (0-31) are control characters used for text formatting (e.g., carriage return, line feed). The remaining characters include printable symbols.
- **Limitations:** ASCII's limitation to 128 characters restricts its ability to represent non-English characters or symbols from other languages.

### Applications
- Widely used in programming languages, text files, and data communication protocols.
- Forms the basis for many other character encoding standards, including UTF-8 (a Unicode variant).

### Example of ASCII Characters

| Character | Decimal | Hexadecimal |
|-----------|---------|-------------|
| A         | 65      | 41          |
| a         | 97      | 61          |
| 0         | 48      | 30          |
| !         | 33      | 21          |
| Space     | 32      | 20          |

## Unicode

### Overview
- Unicode is a comprehensive character encoding standard designed to support the representation of text from all writing systems around the world. It was developed to address the limitations of earlier encoding schemes like ASCII and EBCDIC.
- Unicode can represent over a million code points, allowing it to include virtually every character from every language.

### Characteristics
- **Encoding Forms:** Unicode can be implemented using different encoding forms:
  - **UTF-8:** A variable-width encoding that uses one to four bytes per character. It is backward compatible with ASCII for the first 128 characters.
  - **UTF-16:** Uses two bytes for most common characters but can extend to four bytes for less common ones.
  - **UTF-32:** Uses four bytes for all characters, providing a fixed-width representation but at the cost of increased storage requirements.

### Applications
- Unicode is widely used in modern software applications, web development (HTML), databases, and operating systems to ensure consistent text representation across different platforms.
