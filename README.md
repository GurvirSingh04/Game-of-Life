# Game of Life

This repository contains a Java implementation of Conway's Game of Life, a cellular automaton devised by mathematician John Conway. The simulation models the life and death of cells on a grid based on simple rules, leading to complex and often unpredictable patterns.

## Features

- **Graphical User Interface (GUI)**: Visual representation of the simulation grid.
- **Multiple Organisms**: Simulates various types of organisms, including bacteria, viruses, and chameleons.
- **Dynamic Simulation**: Real-time updates of the grid based on predefined rules for each organism.

## Prerequisites

- Java Development Kit (JDK) installed on your system.
- An Integrated Development Environment (IDE) like IntelliJ IDEA or Eclipse (optional but recommended).

## Installation

1. **Clone this repository:**

   ```bash
   git clone https://github.com/GurvirSingh04/Game-of-Life.git
   cd Game-of-Life
   ```

2. **Compile the application:**

   If you're using an IDE, open the project and build it. If you prefer the command line:

   ```bash
   javac *.java
   ```

3. **Run the application:**

   ```bash
   java SimulatorView
   ```

## File Structure

- `Bacteria.java` - Defines the behavior of bacteria cells.
- `Cell.java` - Abstract class representing a generic cell.
- `Chameleon.java` - Defines the behavior of chameleon cells.
- `Counter.java` - Utility class for counting instances.
- `Field.java` - Represents the simulation grid.
- `FieldCanvas.java` - Handles the graphical rendering of the field.
- `FieldStats.java` - Collects and provides statistics about the field.
- `Location.java` - Represents a location within the grid.
- `Mycoplasma.java` - Defines the behavior of mycoplasma cells.
- `Randomizer.java` - Provides randomization utilities for the simulation.
- `Simulator.java` - The main class that runs the simulation.
- `SimulatorView.java` - Manages the user interface and user interactions.
- `Virus.java` - Defines the behavior of virus cells.

## How It Works

- The simulation initializes a grid (`Field`) populated with various organisms (`Cell` subclasses like `Bacteria`, `Virus`, etc.).
- Each organism follows specific rules determining its survival, reproduction, or death in each generation.
- The `Simulator` class manages the progression of generations, updating the state of the grid and organisms.
- The `SimulatorView` provides a graphical interface, allowing users to observe the evolution of the simulation in real-time.
