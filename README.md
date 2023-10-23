# Cpp-Stacks

# Stack Implementation in C++

This C++ program demonstrates a basic implementation of a stack data structure. A stack is a fundamental data structure that follows the Last-In, First-Out (LIFO) principle, and it's used in various applications in computer science. In this program, we'll create a simple stack and provide algorithms for common stack operations.

## Stack Overview

### What is a Stack?

A **stack** is a linear data structure that follows the LIFO (Last-In, First-Out) principle. This means that the last element added to the stack is the first one to be removed. Imagine a stack of plates: you add a new plate on top and remove the topmost plate when needed. This characteristic is crucial for solving many algorithmic problems and managing data efficiently.

### Key Operations

In this implementation, we provide the following key stack operations:

1. **Push**: Add an element to the top of the stack.
2. **Pop**: Remove and return the top element from the stack.
3. **Peek (or Top)**: Return the top element without removing it.
4. **isEmpty**: Check if the stack is empty.
5. **Size**: Return the number of elements in the stack.

### Implementation

The stack is implemented using a dynamically allocated array. Here's a brief overview of the stack implementation:

- **Stack Initialization**: The stack is initialized with a given capacity, and a dynamic array is allocated to store the elements.

- **Push Operation**: Elements are added to the top of the stack. If the stack is full, it cannot push more elements.

- **Pop Operation**: The top element is removed and returned. If the stack is empty, there's nothing to pop.

- **Peek Operation**: The top element is returned without removing it. If the stack is empty, there's nothing to peek.

- **isEmpty Operation**: Checks if the stack is empty by examining the top index.

- **Size Operation**: Returns the number of elements currently in the stack.

## Algorithm

### Stack Initialization

```cpp
class Stack {
    int* data;
    int top;
    int capacity;
public:
    Stack(int size);
    // Constructor to initialize the stack with the given size.

    ~Stack();
    // Destructor to release allocated memory.

    void push(int element);
    // Push an element onto the stack.

    int pop();
    // Pop the top element from the stack.

    int peek();
    // Return the top element.

    bool isEmpty();
    // Check if the stack is empty.

    int size();
    // Return the number of elements in the stack.
};

![Screenshot 2023-10-23 144549](https://github.com/Arjun378/Cpp-Stacks/assets/74441883/2df5aa9c-b418-4d2c-a493-3f05bf7d5129)

