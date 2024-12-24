# String Manipulation with Threads

## Overview
This C++ program demonstrates multithreading by performing various string manipulations concurrently. It uses threads to process an input string for reversing, capitalization, and character shifting. Mutexes and condition variables are employed to synchronize the threads, ensuring proper execution order.

---

## Features
- Input Thread: Reads a string from the user.
- Reverse Thread: Reverses the input string.
- Capitalization Thread: Converts the input string to uppercase.
- Shift Thread: Shifts each character in the string by a fixed number of positions in the alphabet.

---

## How It Works
1. ** Synchronization:** A condition variable ensures that manipulation threads wait for the input thread to complete before starting their operations.
2. ** Concurrency:** Each manipulation is handled in a separate thread, demonstrating the power of multithreading for independent tasks.

---

## Requirements
C++11 or higher.
A C++ compiler such as `g++`.

---

## How to Run
1. Clone the repository or download the file `string_manipulation_threads.cpp`.
2. Compile the code using:
```bash
g++ -std=c++11 -o string_threads string_manipulation_threads.cpp -pthread
```
3. Run the program:
```bash
./string_threads
```
4. Enter a string when prompted, and view the manipulated outputs.

---

## Sample Output
```plaintext
Enter a string: hello
Reversed string: olleh
Capitalized string: HELLO
Shifted string: jgnnq
