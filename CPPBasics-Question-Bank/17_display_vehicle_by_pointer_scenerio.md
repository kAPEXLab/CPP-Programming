# 17 - Display Vehicle by Pointer

## Introduction
Using pointers to pass objects enables optional ownership and dynamic lifetime management. This exercise demonstrates pointer-based access.

## Scenario
Write `displayVehicleByPointer` that accepts a `Vehicle*` and prints its details, handling `nullptr` safely. Show usage with both valid and null pointers.

## Tasks to Implement
1. Implement void displayVehicleInfo(Vehicle* vehicle).
2. Use pointer access to call displayVehicleInfo().
3. Pass the address of a dynamically allocated Vehicle object.
4. Delete the object after display.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* v = new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); displayVehicleInfo(v); delete v; | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle* v = new Vehicle("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); displayVehicleInfo(v); delete v; | Vehicle ID: XYZ999, Make: Honda, Model: Civic, Year: 2021, Mileage: 45000, Is Electric: 0, Transmission: M, Engine Capacity: 1.8 |
| TC03 | Vehicle* v = new Vehicle("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); displayVehicleInfo(v); delete v; | Vehicle ID: BMW77, Make: BMW, Model: X5, Year: 2020, Mileage: 68000, Is Electric: 0, Transmission: A, Engine Capacity: 3 |
| TC04 | Vehicle* v = new Vehicle("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); displayVehicleInfo(v); delete v; | Vehicle ID: TESLA7, Make: Tesla, Model: Model Y, Year: 2024, Mileage: 1500, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC05 | Vehicle* v = new Vehicle("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); displayVehicleInfo(v); delete v; | Vehicle ID: AUDI08, Make: Audi, Model: A4, Year: 2019, Mileage: 74000, Is Electric: 0, Transmission: M, Engine Capacity: 2 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement a function that accepts a `Vehicle*`, handles null safely, and displays it).
- A short `main()` or test harness that allocates `Vehicle` objects, calls the pointer-based display function, and cleans up to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case and that null pointers are handled safely.

