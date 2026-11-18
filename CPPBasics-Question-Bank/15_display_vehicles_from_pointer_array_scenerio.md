# 15 - Display Vehicles from Pointer Array

## Introduction
Pointer arrays store addresses of heap-allocated objects. This task covers accessing and displaying objects through pointers.

## Scenario
Given an array of `Vehicle*` pointers, each pointing to a heap-allocated `Vehicle`, implement a function that iterates the pointer array and displays each vehicle's details safely (checking for null pointers).

## Tasks to Implement
1. Implement void displayVehiclesInfo(Vehicle* vehicles[], int size).
2. Use the pointer array to iterate through objects.
3. Call displayVehicleInfo() for each Vehicle.
4. Check that all pointer-based objects are displayed.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* arr[2] = { new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), new Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; displayVehiclesInfo(arr, 2); | Both pointer-based vehicles are displayed. |
| TC02 | Vehicle* arr[3] = { new Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), new Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), new Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; displayVehiclesInfo(arr, 3); | All pointer-based vehicles are displayed. |
| TC03 | Vehicle* arr[2] = { new Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), new Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; displayVehiclesInfo(arr, 2); | Both electric vehicles are displayed. |
| TC04 | Vehicle* arr[4] = { new Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), new Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), new Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), new Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; displayVehiclesInfo(arr, 4); | All BMW vehicles are displayed. |
| TC05 | Vehicle* arr[2] = { new Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), new Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; displayVehiclesInfo(arr, 2); | Both Audi vehicles are displayed. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (iterate pointer array and display vehicles safely).
- A short `main()` or test harness that constructs a `Vehicle*` array, populates it with heap-allocated vehicles (or nulls for edge cases), and calls the display function to reproduce the provided test cases (TC01..TC05). Include proper cleanup.
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

