# Chapter 2: Basics of Bend

Welcome to Chapter 2 of the Unofficial Bend Programming Language Guide. This chapter is designed to introduce you to the fundamental concepts of the Bend programming language. We will cover the basics, from writing your first program to understanding the core data types and control flow mechanisms in Bend.

## 2.1 Hello, World! in Bend

Starting with the traditional "Hello, World!" program, we will write a simple Bend script that outputs this greeting.

```python
def main():
  return "Hello, World!"
```

To run this program, save it in a file named `hello_world.bend`. Then, execute it using the following command in your terminal:

```sh
bend run hello_world.bend
```

You should see the output "Hello, World!" in your console.

## 2.2 Understanding Syntax Variants: Imp vs. Fun

Bend offers two syntax variants, Imp and Fun. Imp is imperative and resembles languages like Python, while Fun is functional and similar to Haskell or ML. You can use either syntax or even mix both in the same project. However, in this guide, we'll primarily focus on the Imp syntax for its simplicity and readability for beginners.

## 2.3 Variables and Basic Data Types

In Bend, variables are immutable, meaning once a value is assigned to a variable, it cannot be changed.

```python
def main():
  message = "Hello, Bend!"
  return message
```

Bend supports several basic data types:

- **Integers (u24, i24)**: Unsigned and signed 24-bit integers.
- **Floats (f24)**: 24-bit floating-point numbers.
- **Booleans**: Represented as `true` or `false`.
- **Characters**: Single unicode characters like `'A'` or `'🌟'`.
- **Strings**: Sequences of characters like `"Hello"`.
- **Lists**: Collections of items like `[1, 2, 3]`.

## 2.4 Control Flow: If, Switch, and Match

Control flow in Bend allows you to make decisions in your code. The `if` statement is used to execute code conditionally.

```python
def is_even(number):
  if number % 2 == 0:
    return true
  else:
    return false

def main():
  return is_even(10)
```

The `switch` statement is used for matching against multiple values of a u24 number.

```python
def classify_number(number):
  switch number:
    case 0:
      return "zero"
    case 1:
      return "one"
    case _:
      return "other"

def main():
  return classify_number(1)
```

The `match` statement is used for pattern matching against data types.

```python
type Option:
  Some { value }
  None

def get_option_value(option):
  match option:
    case Option/Some:
      return option.value
    case Option/None:
      return "No value"

def main():
  my_option = Option/Some { value: "Bend is great!" }
  return get_option_value(my_option)
```

In the next chapter, we will delve deeper into functions, exploring how to define and use them effectively in Bend.