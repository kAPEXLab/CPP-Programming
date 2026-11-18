# 18 - Update Vehicle Array Information

## Introduction
Updating elements inside collections is a common requirement; this task practices locating and modifying array entries.

## Scenario
Given an array of `Vehicle` objects, implement a function that finds a vehicle by ID and updates its fields (e.g., mileage or transmission), ensuring the array remains consistent.

## Tasks to Implement
1. Implement void updateVehiclesInfo(Vehicle vehicles[], int size).
2. Loop through the array and update each vehicle using setters.
3. Call the function on a sample array.
4. Display the updated values for verification.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle arr[2] = { Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; updateVehiclesInfo(arr,2); | All vehicles in the array are updated successfully. |
| TC02 | Vehicle arr[3] = { Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; updateVehiclesInfo(arr,3); | All vehicles in the array are updated successfully. |
| TC03 | Vehicle arr[2] = { Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; updateVehiclesInfo(arr,2); | All vehicles in the array are updated successfully. |
| TC04 | Vehicle arr[4] = { Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; updateVehiclesInfo(arr,4); | All vehicles in the array are updated successfully. |
| TC05 | Vehicle arr[2] = { Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; updateVehiclesInfo(arr,2); | All vehicles in the array are updated successfully. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (search and update vehicles within an array and display results).
- A short `main()` or test harness that constructs sample vehicle arrays, runs the `updateVehiclesInfo` function, and prints updated values to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

