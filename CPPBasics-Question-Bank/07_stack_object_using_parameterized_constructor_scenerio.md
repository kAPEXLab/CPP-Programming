# 07 - Stack Object Using Parameterized Constructor

## Introduction
Understanding object lifecycle on the stack is fundamental in C++. This task uses parameterized construction to create stack-based vehicle objects.

## Scenario
A quick diagnostic tool creates temporary `Vehicle` objects on the stack for transient checks. Implement parameterized constructors and create stack instances that automatically clean up at scope exit.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Create a Vehicle object on the stack.
2. Use the parameterized constructor to initialize its values.
3. Display the vehicle information.
4. Describe the automatic lifetime behavior of stack objects.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle car("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); car.displayVehicleInfo(); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle car("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); std::cout << car.getModel(); | Civic |
| TC03 | Vehicle car("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); std::cout << car.getYear(); | 2020 |
| TC04 | Vehicle car("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); std::cout << car.getMake(); | Tesla |
| TC05 | Vehicle car("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); std::cout << car.getMileage(); | 74000 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (parameterized construction of stack `Vehicle` objects and display).
- A short `main()` or test harness that constructs stack `Vehicle` objects using the parameterized constructor and prints their state to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

