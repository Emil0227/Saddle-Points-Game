# Saddle Points Game
This project implements the **Saddle Point Problem** using **Java** with an object-oriented design.  
Developed as part of the MSc Computer Science module *Object-Oriented Programming*, it demonstrates my ability to apply **OOP principles, algorithm design, and unit testing** in Java.

---

## Project Overview
- Simulates a two-player matrix game between **Maxie** (row chooser) and **Minnie** (column chooser).
- Payoff is determined by the matrix entry at the chosen row/column.
- The **saddle point** is the stable strategy where:
  - The chosen row is *minimum in its row but maximum in its column*.
  - Neither player benefits from deviating.

---

## Core Features
- **Random Matrix Generation**
  - `createRandomArray(rows, cols, minVal, maxVal)`
  - Generates test matrices with values in a given range.

- **Array Utilities**
  - `largest(int[] array)` / `smallest(int[] array)`
  - `largestValues(int[][] array)` → max per column  
  - `smallestValues(int[][] array)` → min per row  

- **Saddle Point Detection**
  - `boolean hasSaddlePoint(int[][] array)`  
  - `int saddlePointRow(int[][] array)`  
  - `int saddlePointColumn(int[][] array)`  

- **I/O and Runner**
  - `printArray` and `printArrayInfo` for clear console output.
  - Repeatedly generates random arrays until both “with” and “without” saddle point cases are shown.

---

## Tech Stack
- **Java 17** (compatible with IntelliJ IDEA)  
- **JUnit 5** for unit testing  
- **java.util.Random** for reproducibility of random arrays  

---
