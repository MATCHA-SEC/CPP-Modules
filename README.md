# C++ Modules | The Object-Oriented Programming Journey

[![42 School](https://img.shields.io/badge/42-Network-000000?style=flat-square&logo=42)](https://github.com/souad-hadria)
[![Language: C++98](https://img.shields.io/badge/Language-C%2B%2B98-00599C?style=flat-square&logo=cplusplus)](https://en.cppreference.com/w/)

A complete, intensive series of sub-projects designed to master the paradigms of **Object-Oriented Programming (OOP)**, memory management, and advanced data structures in **C++98**. The curriculum forces a deep understanding of what happens under the hood of a compiler, moving systematically from basic syntax to complex template containers.

---

## 🗂️ Modules Overview & Core Concepts

### [Module 00] Namespace, Classes, Member Functions & Streams
* **Focus**: Transitioning from C structural programming to basic C++ initialization.
* **Concepts**: `std::cout`, `std::cin`, namespacing, class declarations, visibility modifiers (`public`/`private`), and static attributes.

### [Module 01] Memory Allocation, Pointers to Members, References & File Streams
* **Focus**: Dynamic memory control and object lifetimes.
* **Concepts**: Stack vs. Heap allocation, usage of `new` and `delete`, avoiding memory leaks, references (`&`) vs. raw pointers, and file manipulation using `std::ifstream`/`std::ofstream`.

### [Module 02] Ad-hoc Polymorphism, Operator Overloading & Orthodox Canonical Class Form
* **Focus**: Structural class design and custom arithmetic rules.
* **Concepts**: Fixed-point math representations, operator overloading (`+`, `-`, `=`, `<<`), and strict compliance with the **Orthodox Canonical Class Form** (Default Constructor, Copy Constructor, Copy Assignment Operator, Destructor).

### [Module 03] Inheritance & Overriding
* **Focus**: Code reusability and relational hierarchy.
* **Concepts**: Base classes and derived classes, construction/destruction chaining orders, public/protected inheritance, and resolving the classic "Diamond of Death" issue using virtual inheritance.

### [Module 04] Subtype Polymorphism, Abstract Classes & Interfaces
* **Focus**: Dynamic runtime behavior and strict abstraction.
* **Concepts**: Virtual functions, pure virtual functions, building abstract interfaces, virtual destructors (preventing memory leaks in derived objects), and deep vs. shallow copying.

### [Module 05] Repetitive Exceptions & Try-Catch Blocks
* **Focus**: Robust error-handling structures.
* **Concepts**: Building custom nested exception classes inheriting from `std::exception`, throwing exceptions (`throw`), and shielding blocks using `try` / `catch` routines.

### [Module 06] Type Castings
* **Focus**: Explicit and safe memory/type reinterpretation.
* **Concepts**: Mastering C++ style explicit casts:
  * `scalar_cast` operations via `static_cast` (implicit/numeric conversion).
  * `dynamic_cast` (safe down-casting on polymorphic hierarchies).
  * `const_cast` (dropping/adding const volatility modifiers).
  * `reinterpret_cast` (low-level pointer bit re-mapping).

### [Module 07] Templates Meta-programming
* **Focus**: Generic programming and reusable code blueprints.
* **Concepts**: Function templates, class templates, instantiation rules, and generic specialization to write code that operates seamlessly across any standard data type.

### [Module 08] Standard Template Library (STL) Containers & Algorithms
* **Focus**: Standard algorithmic components.
* **Concepts**: Iterators, sequential and associative containers (`std::vector`, `std::list`, `std::map`), and using ready-made `<algorithm>` functions (like `std::find`, `std::count`, `easyfind`).

### [Module 09] Advanced STL Data Structure Pipelines
* **Focus**: Algorithmic complexity and strict choice of data layout.
* **Concepts**: Developing optimized mathematical models using specific constraints:
  * **Reverse Polish Notation (RPN)** calculator.
  * **Bitcoin Exchange** processing using chronological map indexes.
  * **PmergeMe**: Implementing the **Merge-Insertion Sort (Ford-Johnson)** algorithm across multiple complex STL containers to optimize comparisons.

---

## General Rules & Project Hygiene

* **Compilation**: Every single module compiles using the strict flags:
  ```bash
  c++ -Wall -Wextra -Werror -std=c++98 main.cpp Class.cpp -o program
No Modern C++ Shortcuts: Forbidden to use C++11/C++20 smart pointers (unique_ptr, shared_ptr), auto keywords, or range-based for loops. Memory preservation is verified via explicit stack-handling or raw delete cleanups.

Standard Library Discipline: Forbidden to use forbidden external C-libraries. The focus relies strictly on native C++ classes (<iostream>, <string>, <vector>, etc.).
