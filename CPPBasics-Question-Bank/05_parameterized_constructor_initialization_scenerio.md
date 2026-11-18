# 05 - Parameterized Constructor Initialization

## Introduction
Parameterized constructors allow creating fully-initialized objects in a single statement. This improves clarity and reduces error-prone partially-initialized states.

## Scenario
A fleet importer reads CSV records and needs to convert each row into a fully-initialized `Vehicle` object. Implement a parameterized constructor that accepts all relevant fields and sets them correctly on construction.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Create a parameterized constructor for Vehicle.
2. Accept values for ID, make, model, year, mileage, electric status, transmission type, and engine capacity.
3. Initialize all member variables in the constructor body.
4. Create and print a sample object.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v("ABC123", "Toyota", "Camry", 2022, 50000.0f, false, 'A', 2.5); v.displayVehicleInfo(); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle v("XYZ999", "Honda", "Civic", 2021, 45000.0f, false, 'M', 1.8); v.displayVehicleInfo(); | Vehicle ID: XYZ999, Make: Honda, Model: Civic, Year: 2021, Mileage: 45000, Is Electric: 0, Transmission: M, Engine Capacity: 1.8 |
| TC03 | Vehicle v("EV001", "Tesla", "Model 3", 2024, 12000.0f, true, 'A', 0.0); v.displayVehicleInfo(); | Vehicle ID: EV001, Make: Tesla, Model: Model 3, Year: 2024, Mileage: 12000, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC04 | Vehicle v("BMW77", "BMW", "X5", 2020, 68000.0f, false, 'A', 3.0); v.displayVehicleInfo(); | Vehicle ID: BMW77, Make: BMW, Model: X5, Year: 2020, Mileage: 68000, Is Electric: 0, Transmission: A, Engine Capacity: 3 |
| TC05 | Vehicle v("AUDI08", "Audi", "A4", 2019, 74000.0f, false, 'M', 2.0); v.displayVehicleInfo(); | Vehicle ID: AUDI08, Make: Audi, Model: A4, Year: 2019, Mileage: 74000, Is Electric: 0, Transmission: M, Engine Capacity: 2 |

## Suggested Validation Rules

## Expected Deliverables

