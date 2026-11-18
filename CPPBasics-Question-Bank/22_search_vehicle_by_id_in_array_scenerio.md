# 22 - Search Vehicle by ID in Array

## Introduction
Search operations are fundamental for locating records in collections. This task focuses on finding an element by its unique key.

## Scenario
Implement a search function that looks up a `Vehicle` by its ID in an array and returns its index or a sentinel value if not found. Ensure correct handling for edge cases.

## Tasks to Implement
1. Implement void searchVehicles(Vehicle vehicles[], int size, std::string vehicleID).
2. Iterate through the array and compare each vehicleID.
3. Print the matching vehicle details or a not found message.
4. Test with valid and invalid IDs.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle arr[2] = { Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; searchVehicles(arr, 2, "ABC123"); | Vehicle found: ABC123 |
| TC02 | Vehicle arr[3] = { Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; searchVehicles(arr, 3, "V2"); | Vehicle found: V2 |
| TC03 | Vehicle arr[2] = { Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; searchVehicles(arr, 2, "T3"); | Vehicle not found. |
| TC04 | Vehicle arr[4] = { Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; searchVehicles(arr, 4, "B3"); | Vehicle found: B3 |
| TC05 | Vehicle arr[2] = { Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; searchVehicles(arr, 2, "A2"); | Vehicle found: A2 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (search by vehicle ID in an array and print results).
- A short `main()` or test harness that constructs sample arrays and calls the search function to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

