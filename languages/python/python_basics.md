# Python Basics

Python is a widely used programming language known for its simplicity, readability, and flexibility. It is especially popular in scientific research, data analysis, and automation. Its straightforward syntax makes it an ideal first language for anyone new to programming.

This page provides a general overview of important foundational concepts in Python. You will encounter these ideas frequently as you work through assignments, labs, or self-guided learning. The goal is to build familiarity with how Python code is written and what its main components look like.

## **Variables and Values**

A fundamental part of programming is storing and working with data. In Python, we use **variables** to store values. A variable is like a labeled container — you can name it, fill it with something (a number, word, or list), and refer back to it later.

```python
age = 25
name = "Alice"
```

Here, `age` stores the number 25 and `name` stores the string `"Alice"`. Once you assign a value to a variable, you can reuse or modify it. Variables make your code dynamic and adaptable — you don’t need to hard-code values every time.

## **Data Types**

Every piece of data in Python has a type, and different types are used for different kinds of information. A few of the most common include:

- **Integers (`int`)** – Whole numbers like `5`, `42`, or `-3`
- **Floating-point numbers (`float`)** – Decimal numbers like `3.14` or `0.5`
- **Strings (`str`)** – Text surrounded by quotes, like `"hello"`
- **Booleans (`bool`)** – Logical values, either `True` or `False`
- **Lists (`list`)** – Ordered groups of values, like `[1, 2, 3]`

Each data type supports different operations. For example, strings can be joined together (`"hello" + " world"`), and lists can be sorted or extended. Understanding data types will help you know what kind of operations make sense — and what kinds of errors to avoid.

## **Dictionaries**

Another very useful data structure in Python is the **dictionary**. Dictionaries let you store data in pairs: a key and a value. Instead of accessing a value by position (as with lists), you access it by name.

```python
student = {
    "name": "Alice",
    "age": 25,
    "grade": "A"
}
```

This structure makes it easy to represent real-world data, like the attributes of a person or the contents of a record. It’s especially useful when dealing with structured or labeled data.

## **Functions**

Functions are blocks of code designed to perform a specific task. They are reusable and help organize your program into logical sections. Python has many built-in functions — like `print()`, `len()`, or `range()` — but you can also define your own:

```python
def greet(name):
    print("Hello, " + name)
```

Functions help reduce repetition and improve clarity. Instead of copying and pasting the same logic multiple times, you write it once and reuse it by calling the function. This is a core part of writing clean, maintainable code.

## **Indentation and Structure**

Python uses **indentation** (spacing at the beginning of a line) to define blocks of code. This makes the structure of your program very clear — visually and logically. Unlike some languages that use brackets or other symbols, Python requires consistent indentation to know where a block starts and ends.

```python
if age >= 18:
    print("You are an adult")
```

If your indentation is inconsistent, Python will give you an error. For beginners, this might feel strict, but it’s one of the reasons Python code is so readable. It encourages good habits from the start.

## **Comments and Clarity**

In any codebase — even small ones — it's helpful to include **comments**. These are lines that Python ignores when running your program, but they’re extremely useful for explaining what your code is doing.

```python
# Convert temperature from Celsius to Fahrenheit
celsius = 20
fahrenheit = (celsius * 9/5) + 32  # Apply the conversion formula
print("Temperature in Fahrenheit:", fahrenheit)
```

Commenting helps you and others understand your logic. When you come back to a project after several days or weeks, a few comments can make a huge difference.

## **Recommended Learning Resources**

The best way to learn Python is by writing Python. Here are two free platforms that provide guided practice for beginners:

- **Exercism – Python Track**  
  https://exercism.org/tracks/python  
  A structured set of exercises with feedback and explanations. You can explore both the **"Exercises"** and **"Learn"** sections to build your understanding at your own pace.

- **HackInScience: Python Practice Exercises**  
  https://www.hackinscience.org/exercises/  
  A set of progressively challenging problems that focus on syntax, logic, and structure. Try completing at least the first 15–20 to build confidence and fluency.

These platforms are not just about getting the right answer — they’re about building your intuition for how Python works.

## **What Next?**

Once you're comfortable with these basic ideas, you’ll be ready to take the next step: using **libraries**. Python libraries are collections of reusable code that provide tools for specific tasks — such as working with data, creating visualizations, or interacting with files and APIs. These libraries are written and maintained by experts and communities, and using them allows you to solve complex problems without writing every function yourself.

See [Python Libraries](./python_libraries.md) to learn about tools like `pandas`, `matplotlib`, and others that are commonly used in scientific computing and research workflows.
