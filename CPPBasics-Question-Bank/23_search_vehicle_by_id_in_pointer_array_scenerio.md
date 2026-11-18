# 23 - Search Vehicle by ID in Pointer Array

## Introduction
Searching pointer-based collections requires null safety and dereferencing. This problem practices that pattern.

## Scenario
Given an array of `Vehicle*`, write a function to search for a vehicle with a specific ID, returning the pointer if found or `nullptr` otherwise. Handle null pointers in the array gracefully.

## Tasks to Implement
1. Implement void searchVehicles(Vehicle* vehicles[], int size, std::string vehicleID).
2. Access each object through the array of pointers.
3. Display the matching vehicle or indicate no match.
4. Handle null pointers and invalid IDs proactively.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* arr[2] = { new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), new Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; searchVehicles(arr, 2, "DEF456"); | Vehicle found: DEF456 |
| TC02 | Vehicle* arr[3] = { new Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), new Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), new Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; searchVehicles(arr, 3, "V1"); | Vehicle found: V1 |
| TC03 | Vehicle* arr[2] = { new Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), new Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; searchVehicles(arr, 2, "T3"); | Vehicle not found. |
| TC04 | Vehicle* arr[4] = { new Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), new Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), new Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), new Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; searchVehicles(arr, 4, "B4"); | Vehicle found: B4 |
| TC05 | Vehicle* arr[2] = { new Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), new Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; searchVehicles(arr, 2, "A1"); | Vehicle found: A1 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (search a pointer array for a vehicle ID and return/display the pointer or nullptr).
- A short `main()` or test harness that constructs a `Vehicle*` array, runs the search function, and prints the results to reproduce the provided test cases (TC01..TC05). Include cleanup.
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

