# 13 - Display All Vehicles Function

## Introduction
A helper function that displays multiple objects centralizes output logic and avoids duplication. This task practices writing such utility functions.

## Scenario
Given an array of vehicles, implement a `displayAllVehicles` function that accepts the array and its size, then formats and prints each vehicle's data in a readable table.

## Tasks to Implement
1. Create a function displayAllVehicles(Vehicle vehicles[], int size).
2. Loop through the array and print each record.
3. Use the Vehicle display method inside the function.
4. Pass an array and its size to the function for testing.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle arr[2] = { Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; displayAllVehicles(arr, 2); | Both vehicles are printed in order. |
| TC02 | Vehicle arr[3] = { Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; displayAllVehicles(arr, 3); | All three vehicles are printed in order. |
| TC03 | Vehicle arr[2] = { Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; displayAllVehicles(arr, 2); | Both electric vehicles are printed in order. |
| TC04 | Vehicle arr[4] = { Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; displayAllVehicles(arr, 4); | All BMW vehicles are printed in order. |
| TC05 | Vehicle arr[2] = { Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; displayAllVehicles(arr, 2); | Both Audi vehicles are printed in order. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement `displayAllVehicles()` and use it to print an array of vehicles).
- A short `main()` or test harness that constructs the example arrays and calls `displayAllVehicles()` to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

