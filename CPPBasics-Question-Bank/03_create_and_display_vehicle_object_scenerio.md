# 03 - Create and Display Vehicle Object

## Introduction
A readable display of an object's state helps inspectors and users quickly understand vehicle details. This task covers object construction and producing formatted output.

## Scenario
A diagnostic console must create vehicle objects and print their attributes for verification. Implement object creation (default and parameterized) and a display method that formats all properties for human-readable output.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Create a Vehicle object.
2. Set each required value for the car.
3. Call the display method to print the object state.
4. Check that the output matches the assigned values.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle car; car.setVehicleID("ABC123"); car.setMake("Toyota"); car.setModel("Camry"); car.setYear(2022); car.setMileage(50000.0f); car.setIsElectric(false); car.setTransmissionType('A'); car.setEngineCapacity(2.5); car.displayVehicleInfo(); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle car; car.setVehicleID("CIVIC55"); car.setMake("Honda"); car.setModel("Civic"); car.setYear(2023); car.setMileage(28000.0f); car.setIsElectric(false); car.setTransmissionType('M'); car.setEngineCapacity(2.0); car.displayVehicleInfo(); | Vehicle ID: CIVIC55, Make: Honda, Model: Civic, Year: 2023, Mileage: 28000, Is Electric: 0, Transmission: M, Engine Capacity: 2 |
| TC03 | Vehicle car; car.setVehicleID("TESLA7"); car.setMake("Tesla"); car.setModel("Model Y"); car.setYear(2024); car.setMileage(1500.0f); car.setIsElectric(true); car.setTransmissionType('A'); car.setEngineCapacity(0.0); car.displayVehicleInfo(); | Vehicle ID: TESLA7, Make: Tesla, Model: Model Y, Year: 2024, Mileage: 1500, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC04 | Vehicle car; car.setVehicleID("NISSAN9"); car.setMake("Nissan"); car.setModel("Altima"); car.setYear(2021); car.setMileage(42000.0f); car.setIsElectric(false); car.setTransmissionType('A'); car.setEngineCapacity(2.5); car.displayVehicleInfo(); | Vehicle ID: NISSAN9, Make: Nissan, Model: Altima, Year: 2021, Mileage: 42000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC05 | Vehicle car; car.setVehicleID("FORD21"); car.setMake("Ford"); car.setModel("EcoSport"); car.setYear(2020); car.setMileage(62000.0f); car.setIsElectric(false); car.setTransmissionType('M'); car.setEngineCapacity(1.5); car.displayVehicleInfo(); | Vehicle ID: FORD21, Make: Ford, Model: EcoSport, Year: 2020, Mileage: 62000, Is Electric: 0, Transmission: M, Engine Capacity: 1.5 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (create and display a `Vehicle` object).
- A short `main()` or test harness that constructs the example vehicle(s) and prints their state to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

