---
date: 2022-09-06T22:42:23+08:00
title: Basics of progamming
linkTitle: Module 3
nav_weight: 3
series: 
  - Guide
categories:
  - Installation
tags:
  - Windows
images:
  - sdlc.webp
featured: false
authors:
  - Sulaiman
nav_icon:
  vendor: bs
  name: book
  color: indigo
---
### Understanding Programming Languages

Programming languages serve as the foundation of all computer operations, enabling developers to instruct machines and automate tasks efficiently. These languages are broadly classified based on abstraction levels and execution mechanisms, each optimized for particular functions and environments. 

This summary delves into the distinctions between high-level and low-level languages, examines the role of query languages in database management, explains branching and looping logic in programming, and contrasts interpreted and compiled languages. By understanding these categories and their applications, we gain insights into the diverse tools available for solving computational challenges, ranging from managing data to creating advanced software systems.


---

**Programming Languages Overview**

**High-Level vs. Low-Level Programming Languages**  
Programming languages are categorized into high-level and low-level languages. High-level languages, such as Python and SQL, use English-like syntax to simplify coding and debugging. Query languages like SQL are prevalent for database operations, including CRUD tasks (Create, Read, Update, Delete). Low-level languages like assembly language directly map to machine code, using symbols to represent binary instructions. Assembly languages are hardware-specific and translated via assemblers.

**Query Languages**  
Query languages, primarily SQL, facilitate database interaction to retrieve or manipulate data. SQL databases use structured schemas, while NoSQL databases, with dynamic schemas, handle unstructured data. SQL queries are divided into "select" (data retrieval) and "action" commands (data manipulation).

**Branching and Looping Logic**  
Programming logic uses **Boolean expressions** (true/false) and **variables** to control program flow.  
- **Branching Logic**: Guides decisions based on conditions. Common constructs include `if`, `if-else`, and `switch`.  
- **Looping Logic**: Repeats code until a condition is met. Loop types include:
  - **While**: Condition checked before execution.
  - **For**: Executes for a set range.
  - **Do-While**: Executes at least once, checking conditions afterward.

**Interpreted vs. Compiled Programming Languages**  
Programming languages fall into two categories based on execution methods:  
- **Interpreted Languages**: Examples include Python, JavaScript, and HTML. These are platform-independent and execute scripts line-by-line using interpreters. They are ideal for repetitive tasks and ease of use.  
- **Compiled Languages**: Examples include C, Java, and C++. These translate source code into executable files, which run faster but are OS-specific. Compiled languages are suited for larger, complex tasks like operating systems.

**Examples and Use Cases**  
- **Python and JavaScript**: Popular interpreted languages for tasks like scripting and web development.  
- **C and Java**: Core compiled languages used for operating systems and cross-platform programs.  
- **HTML**: A markup language used for web page structuring.  
- **Assembly**: A low-level language closely tied to processor architecture, with a one-to-one mapping to machine code instructions.

In essence, the choice between interpreted and compiled languages, as well as between high-level and low-level, depends on project requirements such as complexity, speed, and hardware constraints.

### FAQ

{{< bs/accordion data="software_engineering.faq" flush=true >}}