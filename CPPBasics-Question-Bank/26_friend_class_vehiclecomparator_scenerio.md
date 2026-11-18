# 26 - Friend Class VehicleComparator

## Introduction
A friend class can encapsulate related utilities that need private access to multiple instances. This pattern centralizes specialized logic.

## Scenario
Create a `VehicleComparator` friend class that can access private members of `Vehicle` to perform complex comparisons or filtering tasks used by the system.

## Tasks to Implement
1. Create a friend class VehicleComparator.
2. Implement bool compareVehicles(Vehicle& vehicle1, Vehicle& vehicle2).
3. Implement void displayVehicleDetails(Vehicle& vehicle).
4. Use the comparator to compare two valid vehicles.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); VehicleComparator c; c.compareVehicles(v1,v2); | true |
| TC02 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); VehicleComparator c; c.compareVehicles(v1,v2); | false |
| TC03 | Vehicle v1("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle v2("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); VehicleComparator c; c.compareVehicles(v1,v2); | true |
| TC04 | Vehicle v1("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle v2("TESLA8","Tesla","Model X",2023,2000.0f,true,'A',0.0); VehicleComparator c; c.compareVehicles(v1,v2); | false |
| TC05 | Vehicle v1("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle v2("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); VehicleComparator c; c.compareVehicles(v1,v2); | true |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement a friend comparator class with compare/display methods and demonstrate it).
- A short `main()` or test harness that constructs example vehicles, creates a `VehicleComparator`, calls its methods, and prints results to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

