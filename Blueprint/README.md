# Blueprint Project 

## Overview
This Java project simulates a building design system, inspired by an Apple AppStore-like blueprint framework.  
It demonstrates object-oriented programming (OOP) principles such as **composition**, **encapsulation**, and **overriding methods**, while using only **primitive arrays** to manage collections.

The project includes three main classes:
- `Unit` – Represents individual rooms with a name, width, and length. Supports toggling between feet and meters.
- `Floor` – Represents a floor of a building, containing multiple `Unit`s. Handles capacity limits and ensures that no floor exceeds its maximum area.
- `Blueprint` – Represents the entire building blueprint, composed of multiple `Floor` instances. Tracks completion percentage based on added floor plans.

JUnit tests are provided to verify functionality and serve as usage examples.

---

## Features
- Add, manage, and compare `Unit`s and `Floor`s.
- Convert unit measurements between **feet** and **meters**.
- Track building blueprint completion as floors are added.
- Ensure proper exception handling when a floor exceeds capacity.
- Equality checks for floors and blueprints, ignoring the order of units/floors.
- Fully tested via JUnit with comprehensive test coverage.

---

## Requirements
- Java 11 or later
- JUnit 4 for testing

---

## How to Run
1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
Navigate to the Blueprint folder:

bash
Copy code
cd Blueprint
Compile the source code:

bash
Copy code
javac -d bin src/model/*.java junit_tests/*.java
Run the JUnit tests:

bash
Copy code
java -cp bin org.junit.runner.JUnitCore junit_tests.StarterTests
