# 04 - Default Constructor Initialization

## Introduction
Objects should start in a valid state without requiring the caller to set every field. This task practices writing default constructors that initialize safe defaults.

## Scenario
A vehicle tracking module must be able to create placeholder vehicle objects before full details arrive. Provide a default constructor that initializes sensible default values (empty strings, zeroed numerics, false booleans) so objects are always usable.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Implement a default constructor for the Vehicle class.
2. Set all attributes to safe default values.
3. Create an object without passing any parameters.
4. Display the object and confirm the default state is correct.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v; v.displayVehicleInfo(); | Vehicle ID: empty, Make: empty, Model: empty, Year: 0, Mileage: 0, Is Electric: 0, Transmission: empty, Engine Capacity: 0 |
| TC02 | Vehicle v; std::cout << v.getVehicleID(); | empty |
| TC03 | Vehicle v; std::cout << v.getYear(); | 0 |
| TC04 | Vehicle v; std::cout << v.getMileage(); | 0 |
| TC05 | Vehicle v; std::cout << v.getTransmissionType(); | empty |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (provide a default constructor and demonstrate default-initialized objects).
- A short `main()` or test harness that constructs default `Vehicle` objects and prints their state to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

