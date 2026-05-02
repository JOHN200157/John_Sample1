# AUTOMATION MASTERY COURSE - COMPLETE TEXTBOOK
## MODULE 1: PROGRAMMING FOUNDATIONS WITH PYTHON

---

## 📚 MODULE 1 OVERVIEW

**Duration**: 4-6 weeks | **Learning Hours**: 60-80  
**Difficulty Level**: Beginner | **Prerequisites**: None  
**Projects**: 5 complete projects  
**Exercises**: 50+ practice problems  
**Code Examples**: 100+  

### 🎯 Learning Objectives

By the end of this module, you will:

1. ✅ Install and configure Python development environment
2. ✅ Write and execute basic Python programs
3. ✅ Understand and use variables, data types, and operators
4. ✅ Control program flow with conditionals and loops
5. ✅ Create and manipulate data structures (lists, dicts, tuples, sets)
6. ✅ Define and use functions effectively
7. ✅ Read and write files in multiple formats
8. ✅ Apply Object-Oriented Programming principles
9. ✅ Use Python Standard Library modules
10. ✅ Build 5 complete automation projects

---

# SECTION 1.1: INTRODUCTION TO PROGRAMMING AND AUTOMATION

## 1.1.1 What is Programming?

### 📝 Definition

**Programming** is the process of writing instructions that tell a computer what to do. These instructions are written in a specific language (like Python) that the computer can understand and execute.

### 💡 Key Concept

Think of programming like writing a recipe:
- A recipe has step-by-step instructions
- A recipe uses specific ingredients
- The result depends on following the steps correctly
- Programming works exactly the same way

### 📊 Programming vs Automation

**Programming**: Writing code to solve problems  
**Automation**: Using code to reduce manual, repetitive work

```
Manual Work (100 hours)
          ↓
Write Automation Script (5 hours of coding)
          ↓
Run Script (5 minutes of execution)
          ↓
Done! (Saved 95 hours)
```

---

## 1.1.2 Why Learn Python for Automation?

### ✅ Advantages of Python

| Feature | Benefit |
|---------|---------|
| Easy to Read | Code looks like English sentences |
| Powerful | Can automate complex tasks |
| Large Community | Millions of solutions online |
| Rich Libraries | Pre-built tools for common tasks |
| Cross-Platform | Works on Windows, macOS, Linux |
| Free and Open Source | No licensing costs |
| Fast to Learn | Beginners can write useful code quickly |

### 📈 Python Popularity

```
2024 Most Popular Programming Languages (TIOBE Index):
1. Python        ████████████████████ 28%
2. C             ████████████░░░░░░░░ 15%
3. C++           ██████████░░░░░░░░░░ 12%
4. Java          ██████████░░░░░░░░░░ 10%
5. C#            ████████░░░░░░░░░░░░ 8%
```

### 🎯 Real-World Automation Examples

**Example 1: File Organization**
```
Manual: Manually sort 1000 files into folders → 2 hours
Python: Write 20-line script → 30 seconds
```

**Example 2: Email Reports**
```
Manual: Copy data, create email, send to 100 people → 3 hours
Python: Write script, schedule it → 15 minutes
```

**Example 3: Web Testing**
```
Manual: Click through website, check 50 features → 1 hour
Python: Write test script → 10 seconds
```

---

## 1.1.3 Your First Python Program

### 📝 Simple Example: Hello World

Create a new file called `hello.py`:

```python
# This is a comment - it doesn't run
print("Hello, World!")
```

### ▶️ How to Run It

**Option 1: Using Command Line**
```bash
python hello.py
```

**Option 2: Using VS Code**
1. Open the file in VS Code
2. Click the ▶️ "Run" button (top right)
3. See output in terminal

**Output:**
```
Hello, World!
```

### 🎯 Breaking Down the Code

```python
print("Hello, World!")
```

| Part | Meaning |
|------|---------|
| `print` | Built-in function that displays text |
| `(` `)` | Parentheses contain the input to the function |
| `"Hello, World!"` | The text to display (in quotes) |

---

## 1.1.4 Understanding Code Execution Flow

### 📊 Flowchart: Program Execution

```
Program Start
  ↓
Read Line 1
  ↓
Execute Line 1
  ↓
Read Line 2
  ↓
Execute Line 2
  ↓
(Continue until last line)
  ↓
Program End
```

### 💡 Key Concept: Sequential Execution

Python reads and executes code **line by line**, **from top to bottom**.

### 📝 Example: Execution Order

```python
print("First line")
print("Second line")
print("Third line")
```

**Execution Order:**
```
Line 1: Prints "First line"
Line 2: Prints "Second line"
Line 3: Prints "Third line"
```

**Output:**
```
First line
Second line
Third line
```

### ⚠️ Common Mistake: Order Matters

```python
# WRONG - This will cause an error
print(name)
name = "Alice"
```

Error: `name is not defined`

**Why?** You can't use `name` before you create it.

**Correct:**
```python
name = "Alice"
print(name)
```

---

# SECTION 1.2: VARIABLES AND DATA TYPES

## 1.2.1 Variables: Storing Information

### 🎯 What is a Variable?

A variable is a container that stores a value. Think of it like a labeled box.

```
Variable Name: age
Variable Value: 25

┌─────────────┐
│    age      │ (label)
│    25       │ (value)
└─────────────┘
```

### 📝 Creating Variables (Assignment)

```python
# Create a variable named 'age' and set its value to 25
age = 25

# Create a variable named 'name' and set its value to "Alice"
name = "Alice"

# Create a variable named 'height' and set its value to 5.7
height = 5.7
```

### 💡 How Assignment Works

```python
age = 25
```

```
    age = 25
     ↑   ↑
     │   └── The value
     └────── The variable name
```

**Read as**: "Assign the value 25 to the variable age"

### 🎨 Variable Naming Rules

✅ **Valid Variable Names:**
```python
name = "Alice"
age = 25
first_name = "Bob"
total_price = 99.99
user_id_123 = 456
_private = "secret"
```

❌ **Invalid Variable Names:**
```python
123age = 25        # Can't start with number
first-name = "Bob" # Can't use hyphens
my variable = 5    # Can't have spaces
for = 10           # Can't use reserved words
```

---

## 1.2.2 Python Data Types

### 🎯 What are Data Types?

Data types describe what kind of value a variable holds.

### 📊 Main Data Types

| Type | Name | Example | Use Case |
|------|------|---------|----------|
| `str` | String | `"Hello"` | Text |
| `int` | Integer | `25` | Whole numbers |
| `float` | Float | `5.7` | Decimal numbers |
| `bool` | Boolean | `True` | True/False values |

---

## 1.2.3 Strings (Text)

### 📝 What is a String?

A string is text enclosed in quotes.

```python
name = "Alice"
greeting = 'Hello'
long_text = """This is
a multi-line
string"""
```

### 🔄 String Concatenation (Joining)

```python
first_name = "Alice"
last_name = "Smith"

# Method 1: Using +
full_name = first_name + " " + last_name
print(full_name)  # Output: Alice Smith

# Method 2: Using f-strings (better)
full_name = f"{first_name} {last_name}"
print(full_name)  # Output: Alice Smith
```

### 📝 String Methods

```python
text = "hello world"

# Convert to uppercase
print(text.upper())  # Output: HELLO WORLD

# Convert to lowercase
print(text.lower())  # Output: hello world

# Capitalize first letter
print(text.capitalize())  # Output: Hello world

# Replace text
print(text.replace("world", "Python"))  # Output: hello Python

# Split into words
print(text.split())  # Output: ['hello', 'world']
```

### 📝 String Indexing

```
String: "Python"
Index:   012345
         
P → Index 0
y → Index 1
t → Index 2
h → Index 3
o → Index 4
n → Index 5
```

```python
text = "Python"

print(text[0])   # Output: P
print(text[1])   # Output: y
print(text[5])   # Output: n
print(text[-1])  # Output: n (last character)
```

---

## 1.2.4 Numbers: Integers and Floats

### 🔢 Integers

```python
age = 25
temperature = -5
count = 1000

# Operations
print(age + 5)      # Output: 30
print(age - 3)      # Output: 22
print(age * 2)      # Output: 50
print(age / 2)      # Output: 12.5
print(age // 2)     # Output: 12 (integer division)
print(age % 2)      # Output: 1 (remainder)
print(age ** 2)     # Output: 625 (power)
```

### 💯 Floats

```python
price = 9.99
height = 5.7
percentage = 0.85

# Operations
print(price + 1.50)     # Output: 11.49
print(height * 2)       # Output: 11.4
```

### 🔀 Type Conversion

```python
# String to Integer
age_str = "25"
age_int = int(age_str)
print(age_int)  # Output: 25

# String to Float
price_str = "9.99"
price_float = float(price_str)
print(price_float)  # Output: 9.99

# Number to String
age = 25
age_str = str(age)
print(age_str)  # Output: "25"
```

---

## 1.2.5 Booleans (True/False)

### 🎯 What is a Boolean?

A boolean is a value that is either `True` or `False`.

```python
is_student = True
is_raining = False
is_adult = True
```

### 🔍 Comparison Operators

```python
age = 25

print(age == 25)      # Output: True
print(age != 25)      # Output: False
print(age > 20)       # Output: True
print(age < 30)       # Output: True
print(age >= 25)      # Output: True
print(age <= 25)      # Output: True
```

### 🧠 Logical Operators

```python
age = 25
is_student = True

# AND
print(age > 18 and is_student)  # Output: True

# OR
print(age > 30 or is_student)   # Output: True

# NOT
print(not is_student)            # Output: False
```

---

# SECTION 1.3: OPERATORS

## 1.3.1 Arithmetic Operators

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `+` | Addition | `10 + 3` | `13` |
| `-` | Subtraction | `10 - 3` | `7` |
| `*` | Multiplication | `10 * 3` | `30` |
| `/` | Division | `10 / 3` | `3.333...` |
| `//` | Floor Division | `10 // 3` | `3` |
| `%` | Modulo | `10 % 3` | `1` |
| `**` | Power | `10 ** 2` | `100` |

### 📝 Examples

```python
# Addition
total = 10 + 5
print(total)  # Output: 15

# Subtraction
difference = 10 - 3
print(difference)  # Output: 7

# Multiplication
product = 4 * 5
print(product)  # Output: 20

# Division
quotient = 10 / 3
print(quotient)  # Output: 3.3333...

# Floor Division
quotient_floor = 10 // 3
print(quotient_floor)  # Output: 3

# Modulo
remainder = 10 % 3
print(remainder)  # Output: 1

# Power
power = 2 ** 3
print(power)  # Output: 8
```

---

## 1.3.2 Comparison Operators

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `==` | Equal to | `5 == 5` | `True` |
| `!=` | Not equal to | `5 != 3` | `True` |
| `>` | Greater than | `5 > 3` | `True` |
| `<` | Less than | `5 < 3` | `False` |
| `>=` | Greater or equal | `5 >= 5` | `True` |
| `<=` | Less or equal | `5 <= 3` | `False` |

### 📝 Examples

```python
age = 25

print(age == 25)      # Output: True
print(age != 20)      # Output: True
print(age > 20)       # Output: True
print(age < 30)       # Output: True
print(age >= 25)      # Output: True
print(age <= 25)      # Output: True
```

---

## 1.3.3 Logical Operators

### 🧠 AND Operator

```python
age = 25
has_license = True

can_drive = age >= 18 and has_license
print(can_drive)  # Output: True

print(True and True)    # Output: True
print(True and False)   # Output: False
```

### 🧠 OR Operator

```python
has_money = True
has_credit_card = False

can_buy = has_money or has_credit_card
print(can_buy)  # Output: True

print(True or False)    # Output: True
print(False or False)   # Output: False
```

### 🧠 NOT Operator

```python
is_raining = True
is_not_raining = not is_raining
print(is_not_raining)  # Output: False

print(not True)   # Output: False
print(not False)  # Output: True
```

---

## 1.3.4 Assignment Operators

| Operator | Equivalent | Example |
|----------|-----------|---------|
| `+=` | `x = x +` | `x += 5` |
| `-=` | `x = x -` | `x -= 3` |
| `*=` | `x = x *` | `x *= 2` |
| `/=` | `x = x /` | `x /= 2` |

### 📝 Examples

```python
x = 10
x += 5  # Same as: x = x + 5
print(x)  # Output: 15

y = 20
y -= 3
print(y)  # Output: 17

z = 4
z *= 2
print(z)  # Output: 8

count = 0
count += 1
print(count)  # Output: 1
```

---

# HANDS-ON EXERCISES - SECTION 1.2 & 1.3

## ✅ Exercise 1: Variables and Types

```python
# Create variables for a person
name = "Alice"
age = 25
height = 5.7
is_student = False

# Print each variable
print(name)
print(age)
print(height)
print(is_student)
```

---

## ✅ Exercise 2: String Operations

```python
# Create string variables
first_name = "John"
last_name = "Doe"

# Create full name
full_name = first_name + " " + last_name
print(full_name)

# Print name length
print(len(full_name))

# Print in uppercase
print(full_name.upper())
```

**Expected Output:**
```
John Doe
8
JOHN DOE
```

---

## ✅ Exercise 3: Math Operations

```python
# Calculate total price
price_per_item = 9.99
quantity = 5
tax_rate = 0.10

subtotal = price_per_item * quantity
tax = subtotal * tax_rate
total = subtotal + tax

print(f"Subtotal: ${subtotal:.2f}")
print(f"Tax: ${tax:.2f}")
print(f"Total: ${total:.2f}")
```

**Expected Output:**
```
Subtotal: $49.95
Tax: $4.99
Total: $54.94
```

---

## ✅ Exercise 4: Logical Operations

```python
# Check eligibility for senior discount
age = 65
is_student = False
is_military = True

# Eligible if: (65+ OR student) AND military
eligible = (age >= 65 or is_student) and is_military
print(f"Eligible for discount: {eligible}")
```

**Expected Output:**
```
Eligible for discount: True
```

---

# QUICK REFERENCE CHEAT SHEET - MODULE 1 PART 1

## Data Types

| Type | Example | Code |
|------|---------|------|
| String | Text | `name = "Alice"` |
| Integer | Whole number | `age = 25` |
| Float | Decimal | `height = 5.7` |
| Boolean | True/False | `is_valid = True` |

## Operators

| Category | Operator | Example |
|----------|----------|---------|
| Arithmetic | `+` `-` `*` `/` `**` | `10 + 5` |
| Comparison | `==` `!=` `>` `<` `>=` `<=` | `age > 18` |
| Logical | `and` `or` `not` | `age > 18 and valid` |

## String Methods

| Method | Purpose | Example |
|--------|---------|---------|
| `.upper()` | Convert to uppercase | `"hello".upper()` |
| `.lower()` | Convert to lowercase | `"HELLO".lower()` |
| `.replace()` | Replace text | `"hello".replace("h", "H")` |
| `.split()` | Split into list | `"hello world".split()` |

## Built-in Functions

| Function | Purpose | Example |
|----------|---------|---------|
| `print()` | Display text | `print("Hello")` |
| `len()` | Get length | `len("hello")` |
| `int()` | Convert to integer | `int("25")` |
| `str()` | Convert to string | `str(25)` |
| `float()` | Convert to float | `float("3.14")` |
| `type()` | Check type | `type(25)` |

---

**✅ Module 1 Part 1 Complete!**

**Next: Module 1 Part 2 will cover:**
- 1.4 Data Structures (Lists, Dictionaries, Tuples, Sets)
- 1.5 Control Flow (If/Elif/Else, For/While Loops)
- 1.6 Functions

