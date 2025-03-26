# 🔹 Python Basics – Learn with Code Examples & Comments

This guide covers essential Python concepts with **detailed explanations and code examples** for **Lists, Dictionaries, Loops, and Functions**.

---

## **1️⃣ Lists in Python**  
A **list** is an **ordered**, **mutable** (changeable) collection of elements. It can store multiple data types.

### **🔹 Creating Lists**
```python
# Creating a list
fruits = ["apple", "banana", "cherry", "mango"]

# Mixed data types
random_list = [10, "hello", 3.14, True]

# Empty list
empty_list = []
```

### **🔹 Accessing List Elements**
```python
fruits = ["apple", "banana", "cherry"]

print(fruits[0])  # Output: apple (first element)
print(fruits[-1]) # Output: cherry (last element)
```

### **🔹 Modifying Lists**
```python
fruits = ["apple", "banana", "cherry"]

# Changing an element
fruits[1] = "orange"
print(fruits)  # Output: ['apple', 'orange', 'cherry']

# Adding elements
fruits.append("grapes")  # Adds to the end
print(fruits)

fruits.insert(1, "blueberry")  # Adds at index 1
print(fruits)

# Removing elements
fruits.remove("apple")  # Removes by value
print(fruits)

deleted_item = fruits.pop(2)  # Removes item at index 2
print(f"Removed: {deleted_item}")
```

### **🔹 List Slicing**
```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7]

print(numbers[2:5])   # Output: [2, 3, 4] (index 2 to 4)
print(numbers[:4])    # Output: [0, 1, 2, 3] (start to index 3)
print(numbers[3:])    # Output: [3, 4, 5, 6, 7] (index 3 to end)
print(numbers[::2])   # Output: [0, 2, 4, 6] (step of 2)
```

---

## **2️⃣ Dictionaries in Python**  
A **dictionary** is an **unordered collection** of key-value pairs.

### **🔹 Creating a Dictionary**
```python
# Creating a dictionary
student = {
    "name": "John",
    "age": 20,
    "grade": "A",
    "subjects": ["Math", "Science"]
}

# Accessing values
print(student["name"])  # Output: John
print(student.get("age"))  # Output: 20
```

### **🔹 Modifying a Dictionary**
```python
student["age"] = 21  # Modifying an existing key
student["city"] = "New York"  # Adding a new key
print(student)
```

### **🔹 Deleting a Key**
```python
del student["grade"]  # Removes 'grade' key
print(student)

removed_value = student.pop("age")  # Removes and returns the value
print(f"Removed Age: {removed_value}")
```

### **🔹 Looping Through a Dictionary**
```python
for key, value in student.items():
    print(f"{key}: {value}")
```

---

## **3️⃣ Loops in Python**  

### **🔹 `for` Loop**
Used to iterate over sequences like lists, strings, and dictionaries.

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(f"I like {fruit}")  
```

**Looping with `range()`**
```python
for i in range(5):  # Loops from 0 to 4
    print(i)
```

**Looping Through a Dictionary**
```python
student = {"name": "John", "age": 20, "grade": "A"}

for key, value in student.items():
    print(f"{key}: {value}")
```

---

### **🔹 `while` Loop**
Used when the number of iterations is unknown.

```python
x = 0
while x < 5:
    print(f"x is {x}")
    x += 1  # Incrementing x
```

### **🔹 `break` and `continue`**
- `break`: Stops the loop.
- `continue`: Skips the current iteration.

```python
for num in range(10):
    if num == 5:
        break  # Stops when num is 5
    print(num)

for num in range(5):
    if num == 2:
        continue  # Skips 2
    print(num)
```

---

## **4️⃣ Functions in Python**  
A **function** is a reusable block of code that performs a specific task.

### **🔹 Defining and Calling Functions**
```python
def greet():
    print("Hello, welcome!")

greet()  # Calling the function
```

### **🔹 Function with Parameters**
```python
def greet_user(name):
    print(f"Hello, {name}!")

greet_user("Alice")  # Output: Hello, Alice!
```

### **🔹 Function with Return Value**
```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

### **🔹 Default Arguments**
```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()       # Output: Hello, Guest!
greet("Alex") # Output: Hello, Alex!
```

### **🔹 Lambda Functions (Anonymous Functions)**
```python
square = lambda x: x * x
print(square(4))  # Output: 16

add = lambda a, b: a + b
print(add(3, 7))  # Output: 10
```

---

## **🔥 Summary**
✅ **Lists** → Ordered, mutable collection. Supports indexing, slicing, modification.  
✅ **Dictionaries** → Unordered, key-value pairs. Fast lookups.  
✅ **Loops** → `for` and `while` loops for iteration. Use `break` & `continue`.  
✅ **Functions** → Code reusability, parameters, return values, default arguments, lambda functions.  

---

### 🚀 Happy Coding! 🎯
