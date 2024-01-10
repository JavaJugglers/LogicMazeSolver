## Overview

In this project, we explore the application of propositional logic to model and solve various planning and reasoning problems in a Pacman-inspired environment. Using Python and logical expressions, we'll delve into tasks like action planning, localization, mapping, and Simultaneous Localization and Mapping (SLAM).

### Key Components

- **Expr Class**: Utilizes propositional logic to describe the environment and Pacman's actions.
- **SAT Solver (pycosat)**: A core tool for solving logical inference tasks.
- **Logic Functions**: Includes various custom functions to represent logical sentences and operations.
- **Pacphysics**: A set of rules that govern the Pacman universe.

## Getting Started

### Prerequisites

- Python 3
- pycosat module: Install via `pip install pycosat`.
- For Windows users, ensure you have Microsoft Visual C++ 14.0 or greater.

### Installation

1. Clone or download the project repository.
2. Navigate to the project directory.
3. Install required packages: `pip install -r requirements.txt`.

### Running Tests

To ensure the pycosat installation is successful, run `python pycosat_test.py` in the project directory. Successful output should display a list of integers.

## Project Structure

- **logic.py**: Defines the Expr class and basic logical operations.
- **logicPlan.py**: Contains the implementation of various logical planning functions.
- **pacphysics.py**: Houses the Pacman physics (pacphysics) logic and rules.

## Key Features

### Expr Class

- Creation and manipulation of propositional logic expressions.
- Supports logical operators: `~`, `&`, `|`, `>>`, `%`.

### SAT Solver Integration

- Utilizes the pycosat module for solving satisfiability problems.
- Key for planning, localization, and mapping tasks.

### Logic Functions

- Functions to create logical sentences, such as `sentence1()`, `sentence2()`, and `sentence3()`.
- Includes `findModel()`, `entails()`, and `plTrueInverse()` for logical inference.

### Pacphysics

- Implementation of the rules that govern the Pacman universe.
- Functions like `pacmanSuccessorAxiomSingle()` and `pacphysicsAxioms()` to define pacphysics.

## Usage Examples

- Logic Planning: Use `positionLogicPlan(problem)` to generate action sequences for reaching goals.
- Localization: Implement `localization(problem, agent)` to find Pacman's position based on sensor inputs.
- Mapping: Utilize `mapping(problem, agent)` to discover wall locations.
- SLAM: `slam(problem, agent)` combines localization and mapping to navigate and understand the environment.

## Debugging and Testing

- Test individual components with predefined unit tests.
- Utilize logging and print statements for debugging complex logical expressions.
- Regularly validate the integrity of logical expressions and SAT solver outputs.

## Contributions and Support

- Contributions are welcome. Please submit pull requests for any enhancements.
- For support, raise issues in the project repository or contact the maintainers.
