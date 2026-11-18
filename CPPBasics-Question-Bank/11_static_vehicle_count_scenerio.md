# 11 - Static Vehicle Count

## Introduction
Static class members let all instances share data such as global counters. This problem practices using static variables to track class-level information.

## Scenario
Maintain a running count of how many `Vehicle` instances have been created. Implement a static counter that increments on construction and decrements (if appropriate) on destruction, and a static accessor to read the count.

## Canonical Vehicle Attributes
Refer to the canonical Vehicle attributes defined in Question 01. This scenario requires adding one class-level member to `Vehicle`:
- `static int vehicleCount` — tracks number of Vehicle instances (increment in constructors, decrement in destructor as applicable)

## Tasks to Implement
1. Add a static integer to the Vehicle class.
2. Increment it in each constructor.
3. Implement a method to return the current value.
4. Create several objects and verify the count.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); std::cout << Vehicle::getVehicleCount(); | 2 |
| TC02 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); Vehicle v3("GHI789","Honda","Civic",2020,70000.0f,false,'A',2.0); std::cout << Vehicle::getVehicleCount(); | 3 |
| TC03 | Vehicle v1("XYZ999","Honda","Civic",2021,45000.0f,false,'A',1.8); std::cout << Vehicle::getVehicleCount(); | 1 |
| TC04 | Vehicle v1("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle v2("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle v3("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); std::cout << Vehicle::getVehicleCount(); | 3 |
| TC05 | Vehicle v1("PQR678","Nissan","Altima",2023,40000.0f,false,'A',2.2); Vehicle v2("STU901","BMW","3-Series",2022,55000.0f,false,'M',2.8); Vehicle v3("VWX234","Audi","A4",2021,65000.0f,false,'A',2.0); Vehicle v4("MNO345","Volkswagen","Golf",2018,90000.0f,false,'M',2.0); std::cout << Vehicle::getVehicleCount(); | 4 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add and manage a `static int vehicleCount` and provide a static accessor).
- A short `main()` or test harness that creates/destroys `Vehicle` objects and prints the vehicle count to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing the vehicle count behaves as expected for each test case.

