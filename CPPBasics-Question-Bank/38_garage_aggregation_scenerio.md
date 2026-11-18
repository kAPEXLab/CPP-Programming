# 38 - Garage Aggregation

## Introduction
Aggregation models relationships where one object contains or references others without ownership; e.g., a garage holds vehicles but does not own them exclusively.

## Scenario
Create a `Garage` class that aggregates multiple `Vehicle` references, allowing adding and listing vehicles without transferring ownership semantics.

## Tasks to Implement
1. Create a Garage class.
2. Implement addVehicle(Vehicle vehicle), removeVehicle(Vehicle vehicle), and displayVehicles().
3. Store multiple vehicles in the garage.
4. Display all items in the collection.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC05 | Garage garage; garage.addVehicle(Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0)); garage.addVehicle(Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0)); garage.displayVehicles(); | Two Audi vehicles printed from the garage. |

- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement `Garage` aggregation and demonstrate listing of vehicles).
- Implement the following `Garage` public API:
	- `Garage();`
	- `void addVehicle(const Vehicle& vehicle);`
	- `void removeVehicle(const std::string& vehicleID);`
	- `void displayVehicles() const;`
- A short `main()` or test harness that constructs a `Garage`, adds/removes vehicles, calls `displayVehicles()`, and reproduces the provided test cases (TC01..TC05 or the provided examples).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

