# 21 - Compare Two Vehicle Pointers

## Introduction
Pointer comparisons often involve checking for `nullptr` and then comparing object contents. This task practices pointer-safe comparisons.

## Scenario
Write a function that accepts two `Vehicle*` pointers and compares them: handle `nullptr`, then compare year and mileage to determine which vehicle is newer or better.

## Tasks to Implement
1. Implement void compareVehicles(Vehicle* vehicle1, Vehicle* vehicle2).
2. Use pointer dereferencing to access the object methods.
3. Display the comparison result.
4. Delete the objects after the comparison.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* v1 = new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle* v2 = new Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); compareVehicles(v1, v2); delete v1; delete v2; | Vehicles are different. |
| TC02 | Vehicle* v1 = new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle* v2 = new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); compareVehicles(v1, v2); delete v1; delete v2; | Vehicles are equal. |
| TC03 | Vehicle* v1 = new Vehicle("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle* v2 = new Vehicle("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); compareVehicles(v1, v2); delete v1; delete v2; | Vehicles are equal. |
| TC04 | Vehicle* v1 = new Vehicle("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle* v2 = new Vehicle("TESLA8","Tesla","Model X",2023,2000.0f,true,'A',0.0); compareVehicles(v1, v2); delete v1; delete v2; | Vehicles are different. |
| TC05 | Vehicle* v1 = new Vehicle("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle* v2 = new Vehicle("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); compareVehicles(v1, v2); delete v1; delete v2; | Vehicles are equal. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement pointer-based comparison routine and show results).
- A short `main()` or test harness that allocates `Vehicle` objects, calls the pointer comparison routine, and cleans up to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case and that `nullptr` cases are handled appropriately.

