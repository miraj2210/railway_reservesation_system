# 🚆 Railway Reservation System (C++)

A lightweight, console-based **Railway Reservation System** written in C++ demonstrating fundamental **Object-Oriented Programming (OOP)** concepts. The application enables users to store, manage, display, and search for train records through an interactive command-line interface.

---

## 📌 Table of Contents

1. [Features](#-features)
2. [OOP Concepts Used](#-oop-concepts-used)
3. [Project Structure](#-project-structure)
4. [How the Code Works](#-how-the-code-works)
5. [How to Compile and Run](#-how-to-compile-and-run)
6. [Menu Options](#-menu-options)
7. [Sample Output](#-sample-output)
8. [Screenshots](#-screenshots)
9. [Limitations and Future Improvements](#-limitations-and-future-improvements)
10. [Author](#-author)

---

## ✨ Features

- **Mandatory Initialization:** Prompts for the entry of 3 initial train records upon startup.
- **Add Records:** Dynamically add new train entries (up to 100 records).
- **View All Records:** Display formatted route and schedule details for all registered trains.
- **Search Functionality:** Quickly find train details using a unique train number.
- **Persistent Menu Loop:** Continuously prompts user actions until explicit exit.

### Data Attributes Stored Per Record

| Field | Data Type | Example Value |
| :--- | :--- | :--- |
| Train Number | `int` | `12901` |
| Train Name | `string` | `Gujarat Mail` |
| Source Station | `string` | `Mumbai` |
| Destination Station | `string` | `Ahmedabad` |
| Departure/Arrival Time | `string` | `10:30 PM` |

---

## 🧠 OOP Concepts Used

| Concept | Implementation Details |
| :--- | :--- |
| **Classes & Objects** | Encapsulated entity logic in `Train` and orchestration logic in `RailwaySystem`. |
| **Encapsulation** | Sensitive fields are marked `private` and accessed strictly via public getters/setters. |
| **Constructors** | Default and parameterized constructors implemented for `Train` initialization. |
| **Destructor** | `~Train()` decrements active instances upon object termination. |
| **Static Members** | `static int train_count` tracks total active objects; managed via `get_train_count()`. |
| **Array of Objects** | `Train trains[100]` utilized for sequential in-memory storage. |
| **Composition** | `RailwaySystem` maintains a "has-a" relationship with `Train`. |

---

## 📁 Project Structure

```text
railway_reservation_system/
├── main.cpp          # Complete source code (Train, RailwaySystem, main)
├── output.png        # Execution screenshot
└── README.md         # Project documentation



## output
[Project Output](output.png)