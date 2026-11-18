# 10 - Compare Vehicles Using This Pointer

## Introduction
The `this` pointer provides access to the current object and is useful when implementing comparison or fluent APIs. This exercise uses `this` to compare and return object references.

## Scenario
In a comparison routine, implement a member function that compares the calling `Vehicle` with another passed vehicle using `this` to access the caller's fields and return comparison results.

## Tasks to Implement
1. Implement a compareVehicles() method.
2. Use the this pointer to access the current object.
3. Compare the current vehicle with another vehicle object.
4. Display the result of the comparison.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle myVehicle1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle myVehicle2("XYZ999","Honda","Civic",2021,45000.0f,false,'A',2.0); myVehicle1.compareVehicles(myVehicle2); | Vehicles are different. |
| TC02 | Vehicle myVehicle1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle myVehicle2("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); myVehicle1.compareVehicles(myVehicle2); | Vehicles are equal. |
| TC03 | Vehicle a("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle b("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); a.compareVehicles(b); | Vehicles are equal. |
| TC04 | Vehicle a("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle b("TESLA8","Tesla","Model X",2023,2000.0f,true,'A',0.0); a.compareVehicles(b); | Vehicles are different. |
| TC05 | Vehicle a("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle b("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); a.compareVehicles(b); | Vehicles are equal. |

## Suggested Validation Rules

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement `compareVehicles()` using `this` pointer and display results).
- A short `main()` or test harness that constructs example vehicles and calls the comparison method to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing the comparison outputs match the Expected Output for each test case.
