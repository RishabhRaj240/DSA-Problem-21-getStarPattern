⭐ Pattern 21 – Hollow Square Star Pattern in C++

A C++ program that generates a hollow square star pattern using nested loops and conditional statements. Only the boundary of the square is filled with stars, while the inside remains empty.

📌 Overview

The program takes an integer n and generates an n × n hollow square.

For n = 5, the output is:

*****
*   *
*   *
*   *
*****

The program also supports multiple test cases.

✨ Features
Generates a hollow square pattern.
Uses nested for loops.
Uses conditional statements to identify boundary positions.
Supports multiple test cases.
Demonstrates 2D grid traversal.
Simple and beginner-friendly implementation.
🛠️ Technologies Used
Technology	Purpose
C++	Programming language
iostream	Input and output
Nested Loops	Grid and pattern traversal
if-else	Boundary detection
📝 Problem Statement

Given an integer n, print an n × n square where:

The first row contains stars.
The last row contains stars.
The first column contains stars.
The last column contains stars.
All other positions contain spaces.
Example

For n = 5:

*****
*   *
*   *
*   *
*****
🧠 Approach

The program uses two nested loops to traverse every position in the n × n grid.

A star is printed when the current position belongs to the boundary:

if (i == 0 || j == 0 || i == n - 1 || j == n - 1)

This checks four conditions:

Condition	Represents
i == 0	Top boundary
i == n - 1	Bottom boundary
j == 0	Left boundary
j == n - 1	Right boundary

If none of these conditions are true, a space is printed.

💻 Source Code
#include <iostream>
using namespace std;

void Pattern21(int n) {
    for (int i = 0; i < n; i++) {

        for (int j = 0; j < n; j++) {

            if (i == 0 || j == 0 || i == n - 1 || j == n - 1) {
                cout << "*";
            }
            else {
                cout << " ";
            }
        }

        cout << endl;
    }
}

int main() {
    int t;
    cin >> t;

    for (int i = 0; i < t; i++) {
        int n;
        cin >> n;
        Pattern21(n);
    }

    return 0;
}
📥 Example Input
2
4
5
📤 Example Output
****
*  *
*  *
****

*****
*   *
*   *
*   *
*****
▶️ How to Run
1. Clone the repository
git clone <repository-url>
cd <repository-folder>
2. Compile the program
g++ main.cpp -o main
3. Run the program
./main

Windows: Use main.exe instead of ./main.

📚 Learning Concepts

This program demonstrates:

Nested for loops
2D grid traversal
Pattern printing
Boundary conditions
if-else statements
Logical OR operator ||
Functions in C++
Multiple test cases
Console input/output
⏱️ Complexity Analysis

For an n × n pattern:

Time Complexity: O(n²)
Auxiliary Space: O(1)

The program visits every position in the n × n grid exactly once.

📸 Screenshot

Add your program output screenshot to:

screenshots/output.png

Then include it in the README:

<img width="58" height="106" alt="Screenshot 2026-09-29 at 9 33 23 PM" src="https://github.com/user-attachments/assets/a93b0460-925c-4e83-937b-6c2a949bccb9" />

Recommended project structure:

Pattern21/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
👤 Author

Rishab Raj Chourasia

C++ | Data Structures & Algorithms | Problem Solving
