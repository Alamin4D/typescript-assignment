# 📘 TypeScript Advanced Problem Solving Assignment

## 📌 Overview

This project demonstrates advanced TypeScript concepts through problem-solving and technical blog writing.  
It focuses on **type safety, OOP principles, generics, interfaces, and data manipulation** using clean and scalable code practices.

---

## 📂 Project Structure
├── solutions.ts
├── blog-1.md
├── blog-2.md
└── README.md


---

## 💻 Coding Problems Covered

### 🔢 Problem 1: Even Number Filter
Filters only even numbers from an array using TypeScript array methods.

---

### 🔁 Problem 2: Reverse String
Reverses a given string using built-in string and array methods.

---

### 🔍 Problem 3: Type Checking
Uses union types and type guards to check whether a value is a string or number.

---

### 🧠 Problem 4: Generic Property Getter
Implements a reusable generic function to safely access object properties.

---

### 📚 Problem 5: Book Interface
Uses TypeScript interfaces to extend a `Book` type with an `isRead` property.

---

### 👨‍🏫 Problem 6: OOP Inheritance
Implements `Person` and `Student` classes using inheritance and method overriding.

---

### 🔗 Problem 7: Array Intersection
Finds common elements between two arrays using filtering logic.

---

## 📝 Blog Topics

### ✍️ Blog 2: Why any is called a “type safety hole” and why unknown is safer
 any disables TypeScript’s type checking. Once a value is any, you can do anything with it, and TypeScript won’t warn you—even if it’s wrong. This removes type safety completely and can easily cause runtime errors.

On the other hand, unknown also represents an unknown value, but TypeScript forces you to check its type before using it. You cannot directly perform operations on it without validation. This keeps type safety intact and prevents unsafe usage.

### ✍️ Blog 2: Generics in TypeScript
Explains how generics help create reusable, flexible, and type-safe components.

---

## 🛠️ Technologies Used

- TypeScript  
- Object-Oriented Programming (OOP)  
- Functional Programming Concepts  
- Generics & Type Safety  

---

## 🎯 Learning Outcome

After completing this assignment, you will understand:

- How to write type-safe TypeScript code  
- How to use generics effectively  
- How OOP improves code structure  
- How to design reusable functions and classes  

---

## 🚀 How to Run

```bash
# Install TypeScript globally (if not installed)
npm install -g typescript

# Compile TypeScript file
tsc solutions.ts

# Run compiled JavaScript
node solutions.js