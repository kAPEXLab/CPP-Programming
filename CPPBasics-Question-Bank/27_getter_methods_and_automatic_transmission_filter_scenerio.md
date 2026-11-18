# 27 - Getter Methods and Automatic Transmission Filter

## Introduction
Getter methods expose safe, read-only access to object properties. They are essential for encapsulation and controlled data retrieval.

## Scenario
Implement getters for vehicle attributes and demonstrate using them to filter a collection for vehicles with automatic transmission.

## Tasks to Implement
1. Create getter methods for all private data members.
2. Implement void displayVehiclesWithAutomaticTransmission(Vehicle vehicles[], int size).
3. Iterate over the array and print vehicles whose transmission type is 'A'.
4. Use the getters instead of direct field access.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle arr[2] = { Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0) }; displayVehiclesWithAutomaticTransmission(arr,2); | Only ABC123 Toyota Camry is displayed. |
| TC02 | Vehicle arr[3] = { Vehicle("V1","Honda","Civic",2021,45000.0f,false,'A',1.8), Vehicle("V2","Kia","Seltos",2022,33000.0f,false,'M',1.5), Vehicle("V3","Hyundai","Verna",2020,50000.0f,false,'A',1.6) }; displayVehiclesWithAutomaticTransmission(arr,3); | Only V1 Honda Civic and V3 Hyundai Verna are displayed. |
| TC03 | Vehicle arr[2] = { Vehicle("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0), Vehicle("T2","Tesla","Model Y",2024,10000.0f,true,'A',0.0) }; displayVehiclesWithAutomaticTransmission(arr,2); | Both Tesla vehicles are displayed. |
| TC04 | Vehicle arr[4] = { Vehicle("B1","BMW","X5",2020,68000.0f,false,'A',3.0), Vehicle("B2","BMW","3-Series",2022,55000.0f,false,'M',2.8), Vehicle("B3","BMW","M5",2021,48000.0f,false,'A',4.4), Vehicle("B4","BMW","Z4",2023,21000.0f,false,'M',2.0) }; displayVehiclesWithAutomaticTransmission(arr,4); | B1 BMW X5 and B3 BMW M5 are displayed. |
| TC05 | Vehicle arr[2] = { Vehicle("A1","Audi","A4",2019,74000.0f,false,'M',2.0), Vehicle("A2","Audi","Q5",2022,36000.0f,false,'A',2.0) }; displayVehiclesWithAutomaticTransmission(arr,2); | Only A2 Audi Q5 is displayed. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement getters and a filter-by-automatic function and demonstrate it).
- A short `main()` or test harness that constructs sample vehicles, uses the getters and the filter function to reproduce the provided test cases (TC01..TC05), and prints results.
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

