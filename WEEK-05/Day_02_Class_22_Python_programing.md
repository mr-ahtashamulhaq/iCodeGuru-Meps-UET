# Class 22 – Python For All (Part 1)  
**Topic:** Python Basics – Variables, If-Else, and Loops  

---

## 🐍 Introduction to Python  
- High-level, interpreted programming language.  
- Easy syntax → beginner-friendly.  
- Widely used in **web development, AI/ML, automation, data science**.  

---

## 📦 Variables in Python  
- **Definition:** Variables store data values.  
- No need to declare type explicitly (Python is **dynamically typed**).  

### Example:
```python
name = "Ali"         # String
age = 20             # Integer
pi = 3.14            # Float
is_student = True    # Boolean
⚡ If-Else Statements
Used for decision making.

Syntax:

python
Copy code
if condition:
    # code if condition is true
elif another_condition:
    # code if this condition is true
else:
    # code if none are true
Example:

marks = 75

if marks >= 80:
    print("Grade: A")
elif marks >= 60:
    print("Grade: B")
else:
    print("Grade: C")
🔁 Loops in Python
For Loop
Used for iterating over a sequence (list, string, range, etc.).


for i in range(5):
    print("Iteration:", i)
While Loop
Repeats while a condition is True.


count = 1
while count <= 5:
    print("Count:", count)
    count += 1
🧠 Key Takeaways
Variables → store values without declaring types.

If-Else → used for conditions and decision making.

Loops (for/while) → repeat tasks efficiently.

🔜 Next: Python Part 2 – Functions, Lists, Strings.