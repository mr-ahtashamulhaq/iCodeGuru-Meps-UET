 # Class 23 – Python For All (Part 2)  

---

## 📋 Lists in Python  
- **Definition:** A list is a **mutable, ordered collection** that can store multiple items in a single variable.  
- **Characteristics:**  
  - Ordered (elements keep their insertion order).  
  - Mutable (can be modified after creation).  
  - Can contain **mixed data types** (integers, strings, floats, etc.).  

### Example:
```python
# Creating a list
numbers = [1, 2, 3, 4, 5]
mixed = [1, "hello", 3.14, True]

# Accessing elements
print(numbers[0])   # 1
print(mixed[1])     # hello

# Adding elements
numbers.append(6)   # [1, 2, 3, 4, 5, 6]

# Removing elements
numbers.remove(3)   # [1, 2, 4, 5, 6]

# Iterating over list
for item in mixed:
    print(item)
🆔 id() Function in Python
The id() function returns the unique identity (memory address) of an object.

Two variables with the same value may point to the same memory location (especially with immutable data types like integers, strings, tuples).

Example:
python
Copy code
a = 100
b = 100
print(id(a))   # e.g., 140721...
print(id(b))   # same as id(a), because Python optimizes memory for immutable objects

c = [1, 2, 3]
d = [1, 2, 3]
print(id(c))   # different memory
print(id(d))   # different memory (lists are mutable, so each gets unique memory)
🔑 Key Insight:

Immutable objects → may share memory if values are same (Python uses interning).

Mutable objects → always different memory locations, even with same values.

🔄 Typecasting in Python
Definition: Converting one data type into another.

Common Conversions:

# Integer to String
num = 123
print(str(num))        # "123"

# String to Integer
s = "456"
print(int(s))          # 456

# Float to Integer
pi = 3.14
print(int(pi))         # 3 (truncates decimals)

# List to Set
nums = [1, 2, 2, 3]
unique_nums = set(nums)   # {1, 2, 3}
⚠️ Important:

Conversion may cause data loss (e.g., float → int drops decimals).

Invalid conversions throw ValueError.

int("hello")   # ❌ ValueError
🧠 Memory Management in Python
Python handles memory automatically with:

Reference Counting:

Each object has a reference counter.

When no variables reference the object → memory is freed.

Garbage Collection (GC):

Python has a built-in garbage collector to clean up unused objects (especially cyclic references).

Same Value Optimization:

Immutable objects like small integers (-5 to 256) and strings are cached in memory (called object interning) for reuse.

Example:
# Small integers (-5 to 256) share memory
x = 10
y = 10
print(id(x) == id(y))   # True

# Larger integers → may create new objects
a = 1000
b = 1000
print(id(a) == id(b))   # False (depends on Python implementation)

# Strings with same literal → may share memory
s1 = "hello"
s2 = "hello"
print(id(s1) == id(s2))   # True
🧠 Key Takeaways
Lists → mutable, ordered, can store mixed types.

id() → shows memory address of objects.

Typecasting → allows flexible conversion between types.

Memory Management → Python optimizes immutable objects, uses garbage collection, and reference counting.

🔜 Next: Python Part 3 – Strings, Functions, and Data Structures.