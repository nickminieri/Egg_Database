# Egg Shipment Database

## Overview
This project is a C program that manages an egg shipment database. The program demonstrates basic concepts of C programming by allowing users to input, manage, and display data related to companies, shipments, and eggs. It features a menu-driven interface and robust input validation.

## Features
- **Input Data:**
  - Company information: Name and state.
  - Shipment details: Shipment number, date, and cost.
  - Egg information: Grade, size, and cost.

- **Data Management:**
  - View entered data for companies, shipments, and eggs.
  - Clear all entered data.
  - Exit the program.

- **User Interaction:**
  - Menu-driven system for user-friendly navigation.
  - Input validation to ensure data consistency.

## How to Use
### Compilation
1. Ensure you have a C compiler installed (e.g., GCC).
2. Compile the program using the following command:
   ```bash
   gcc -o egg_database egg_database.c -Wall -g -lm
   ```

### Running the Program
1. Run the compiled program:
   ```bash
   ./egg_database
   ```
2. Follow the on-screen prompts to:
   - Enter company, shipment, or egg data.
   - View or clear data.
   - Exit the program when finished.

## Assumptions
1. The program accepts the following inputs:
   - Company name (up to 32 characters).
   - Two-letter state abbreviation.
   - Shipment number (integer).
   - Shipment date (in the format `mm-dd-yyyy`).
   - Shipment cost (decimal).
   - Egg grade ("AA", "A", or "B").
   - Egg size ("Small", "Medium", "Large", "Extra-Large", or "Jumbo").
   - Egg cost (decimal).
2. The program cycles through the menu until the user chooses to quit.

## Limitations
- When clearing data, the company state resets to 0, displaying "Alabama" by default.
- Input validation may prompt for re-entry if invalid data is provided.

## Code Structure
- **Struct Definitions:**
  - `struct company`: Stores company name and state.
  - `struct shipment`: Stores shipment number, date, and cost.
  - `struct egg`: Stores egg grade, size, and cost.

- **Functions:**
  - `getCompanyData`: Collects company information.
  - `getShipmentData`: Collects shipment details.
  - `getEggData`: Collects egg information.
  - `displayCompanyData`, `displayShipmentData`, `displayEggData`: Displays entered data.
  - `main`: Implements the menu-driven system and handles program flow.

## Development Notes
- Code was written and tested in Visual Studio Code.
- Compilation was verified using GCC on both local and CES Ubuntu systems.
- No warnings or errors were found during compilation.

## Author
Nicholas Minieri
