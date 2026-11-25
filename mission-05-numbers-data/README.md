# Mission 5 – Numbers and Data

## 1. Task / objective

To understand how computers represent numbers and text using binary and hexadecimal systems. Practise manual number conversions, verify the answers using Python, build a number converter program and learn about character encoding.

## 2. Work completed

- Converted decimal numbers to binary by hand.
- Converted binary numbers to decimal.
- Converted hexadecimal values to decimal.
- Converted binary values to hexadecimal.
- Verified the conversions using Python.
- Created a Python number converter that accepts decimal input and displays binary and hexadecimal results.
- Tested the converter using three different numbers.
- Learned about ASCII and UTF-8 character encoding.

## 3. Commands / tools used

| Command / Tool | Purpose |
|---|---|
| `python3` | Opens the Python interactive environment. |
| `bin()` | Converts a decimal number to binary. |
| `int(value, 2)` | Converts a binary value to decimal. |
| `int(value, 16)` | Converts a hexadecimal value to decimal. |
| `hex()` | Converts a number to hexadecimal. |
| `ord()` | Returns the Unicode code point of a character. |
| `touch number_converter.py` | Creates a Python file if it does not exist. |
| `open -a "Visual Studio Code" number_converter.py` | Opens the converter in VS Code. |
| `python3 number_converter.py` | Runs the number converter. |

## 4. Task 5.1 – Convert numbers by hand

| Question | Working | Answer |
|---|---|---|
| Decimal 13 to binary | 13 = 8 + 4 + 1 | 1101 |
| Decimal 25 to binary | 25 = 16 + 8 + 1 | 11001 |
| Binary 1010 to decimal | 8 + 2 | 10 |
| Binary 1101 to decimal | 8 + 4 + 1 | 13 |
| Hexadecimal A to decimal | A = 10 | 10 |
| Hexadecimal 1F to decimal | 1 × 16 + 15 | 31 |
| Binary 1111 to hexadecimal | 1111 = 15 | F |

## 5. Task 5.2 – Verify using Python

Used Python's built-in conversion functions to verify the manual calculations.

**Expressions used:**

```python
bin(13)
bin(25)
int("1010", 2)
int("1101", 2)
int("A", 16)
int("1F", 16)
hex(int("1111", 2))
```

**Results:**

| Expression | Result |
|---|---|
| `bin(13)` | 0b1101 |
| `bin(25)` | 0b11001 |
| `int("1010", 2)` | 10 |
| `int("1101", 2)` | 13 |
| `int("A", 16)` | 10 |
| `int("1F", 16)` | 31 |
| `hex(int("1111", 2))` | 0xf |

The Python results matched the manual calculations.

## 6. Task 5.3 – Build a small number converter

Created a Python file named `number_converter.py`.

**Program code:**

```python
number = int(input("Enter a decimal number: "))

binary = bin(number)[2:]
hexadecimal = hex(number)[2:].upper()

print("Binary:", binary)
print("Hexadecimal:", hexadecimal)
```

**Test results:**

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 1010 | A |
| 25 | 11001 | 19 |
| 100 | 1100100 | 64 |

The program successfully converted all three test numbers.

**Explanation:**

The input() function accepts a number from the user, and int() converts it into an integer. The bin() function converts the number into binary, while hex() converts it into hexadecimal. The [2:] operation removes the prefixes, and upper() displays hexadecimal letters in uppercase.

## 7. Task 5.4 – How is text stored?

- The ASCII decimal code for uppercase A is 65.
- The ASCII decimal code for lowercase a is 97.

**Why is character encoding needed?**

Computers store information in binary form. Character encoding assigns numerical values to characters so that computers can store, process and display text correctly.

**Example of a character outside basic ASCII:**

The Indian Rupee symbol (₹) is an example of a character that is not included in basic ASCII.

UTF-8 can represent a much wider range of characters than basic ASCII.

## 8. My understanding

Through this mission, I learned how decimal, binary and hexadecimal number systems work and how to convert values between them. I also learned how Python's built-in functions can perform these conversions and how character encoding allows computers to represent text using binary data.

## 9. Difficulties faced

Initially, understanding the different number systems and converting values between them required some practice. I also had to understand how Python's conversion functions work.

## 10. How I resolved them

I practised the conversions manually and verified the results using Python. I tested the number converter with different inputs to check that it produced the correct binary and hexadecimal outputs.

## 11. Evidence / files

- `mission-05-numbers-data/README.md` – Contains manual calculations, Python verification, explanations and test results.
- `mission-05-numbers-data/number_converter.py` – Contains the working Python number converter.

## 12. Commit details

- Commit message: Build number converter and practise data representation.
- The completed Mission 5 files were committed and pushed to GitHub. The updated files were verified in the repository.