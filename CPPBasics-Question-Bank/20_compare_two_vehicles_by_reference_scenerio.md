# 20 - Compare Two Vehicles by Reference

## Introduction
Comparing objects by reference enables efficient equality and ordering checks without copying. This task focuses on reference-based comparisons.

## Scenario
Implement a `compareByReference` function that takes two `Vehicle&` parameters and returns whether they are equal by value, or which one is newer based on year and mileage.

## Tasks to Implement
1. Implement void compareVehicles(Vehicle& vehicle1, Vehicle& vehicle2).
2. Use the class compareVehicles() method to compare the two objects.
3. Display the comparison result.
4. Check both equal and non-equal examples.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); compareVehicles(v1, v2); | Vehicles are equal. |
| TC02 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); compareVehicles(v1, v2); | Vehicles are different. |
| TC03 | Vehicle v1("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle v2("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); compareVehicles(v1, v2); | Vehicles are equal. |
| TC04 | Vehicle v1("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle v2("TESLA8","Tesla","Model X",2023,2000.0f,true,'A',0.0); compareVehicles(v1, v2); | Vehicles are different. |
| TC05 | Vehicle v1("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle v2("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); compareVehicles(v1, v2); | Vehicles are equal. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement compare-by-reference functionality and display results).
- A short `main()` or test harness that constructs sample vehicles and calls the comparison function to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

