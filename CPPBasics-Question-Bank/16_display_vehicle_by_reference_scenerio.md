# 16 - Display Vehicle by Reference

## Introduction
Passing objects by reference avoids copying and allows direct modification. This question focuses on reference semantics for functions.

## Scenario
Implement a function `displayVehicleByReference` that accepts a `Vehicle&` and prints its fields. Demonstrate calling it with existing stack and heap objects without copying.

## Tasks to Implement
1. Implement void displayVehicleInfo(Vehicle& vehicle).
2. Pass a Vehicle object by reference.
3. Use the method displayVehicleInfo() within the function.
4. Validate the result with a sample object.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); displayVehicleInfo(v); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle v("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); displayVehicleInfo(v); | Vehicle ID: XYZ999, Make: Honda, Model: Civic, Year: 2021, Mileage: 45000, Is Electric: 0, Transmission: M, Engine Capacity: 1.8 |
| TC03 | Vehicle v("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); displayVehicleInfo(v); | Vehicle ID: BMW77, Make: BMW, Model: X5, Year: 2020, Mileage: 68000, Is Electric: 0, Transmission: A, Engine Capacity: 3 |
| TC04 | Vehicle v("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); displayVehicleInfo(v); | Vehicle ID: TESLA7, Make: Tesla, Model: Model Y, Year: 2024, Mileage: 1500, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC05 | Vehicle v("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); displayVehicleInfo(v); | Vehicle ID: AUDI08, Make: Audi, Model: A4, Year: 2019, Mileage: 74000, Is Electric: 0, Transmission: M, Engine Capacity: 2 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement a function that accepts a `Vehicle&` and displays it).
- A short `main()` or test harness that constructs vehicles and calls the display-by-reference function to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

