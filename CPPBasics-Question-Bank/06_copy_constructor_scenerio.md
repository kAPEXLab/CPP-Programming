# 06 - Copy Constructor

## Introduction
Copy constructors enable creating a new object as a copy of an existing one, ensuring member-wise duplication and correct ownership handling for resources.

## Scenario
When cloning vehicle records for temporary edits or simulations, the system must duplicate an existing `Vehicle` instance while keeping original intact. Implement a copy constructor that correctly copies all fields.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Implement a copy constructor for Vehicle.
2. Copy all member values from the source object.
3. Create a duplicate vehicle and display both values.
4. Confirm that the copy matches the original object.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2(v1); v2.displayVehicleInfo(); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle v1("MNO345","Ford","Mustang",2021,60000.0f,false,'M',3.0); Vehicle v2(v1); v2.setMileage(65000.0f); v2.displayVehicleInfo(); | Vehicle ID: MNO345, Make: Ford, Model: Mustang, Year: 2021, Mileage: 65000, Is Electric: 0, Transmission: M, Engine Capacity: 3 |
| TC03 | Vehicle v1("GHI789","Honda","Civic",2020,70000.0f,false,'A',2.0); Vehicle v2(v1); v2.setModel("City"); v2.displayVehicleInfo(); | Vehicle ID: GHI789, Make: Honda, Model: City, Year: 2020, Mileage: 70000, Is Electric: 0, Transmission: A, Engine Capacity: 2 |
| TC04 | Vehicle v1("JKL012","Tesla","Model S",2019,80000.0f,true,'A',0.0); Vehicle v2(v1); v2.setYear(2020); v2.displayVehicleInfo(); | Vehicle ID: JKL012, Make: Tesla, Model: Model S, Year: 2020, Mileage: 80000, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC05 | Vehicle v1("PQR678","Audi","A5",2022,34000.0f,false,'A',2.0); Vehicle v2(v1); v2.setVehicleID("NEW111"); v2.displayVehicleInfo(); | Vehicle ID: NEW111, Make: Audi, Model: A5, Year: 2022, Mileage: 34000, Is Electric: 0, Transmission: A, Engine Capacity: 2 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (copy constructor behavior and demonstration).
- A short `main()` or test harness that constructs objects using the copy constructor and prints their state to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

