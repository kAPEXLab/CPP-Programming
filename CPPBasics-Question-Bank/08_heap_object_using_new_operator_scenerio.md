# 08 - Heap Object Using New Operator

## Introduction
Heap allocation is used for objects that must outlive the current scope or have dynamic lifetimes. This exercise covers creating and managing heap-based objects with `new` and `delete`.

## Scenario
Implement creating `Vehicle` instances on the heap to simulate records that persist beyond function scope. Ensure proper allocation and deallocation to avoid memory leaks.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Create a Vehicle object using the new operator.
2. Initialize it with values through the parameterized constructor.
3. Call the display method through the pointer.
4. Delete the object after use.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* car = new Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); car->displayVehicleInfo(); delete car; | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Mileage: 50000, Is Electric: 0, Transmission: A, Engine Capacity: 2.5 |
| TC02 | Vehicle* car = new Vehicle("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); std::cout << car->getModel(); delete car; | Civic |
| TC03 | Vehicle* car = new Vehicle("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); std::cout << car->getYear(); delete car; | 2020 |
| TC04 | Vehicle* car = new Vehicle("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); std::cout << car->getMake(); delete car; | Tesla |
| TC05 | Vehicle* car = new Vehicle("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); std::cout << car->getMileage(); delete car; | 74000 |

## Suggested Validation Rules

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (heap allocation with `new` for `Vehicle` objects, correct usage of `delete`, and display via pointer).
- A short `main()` or test harness that allocates `Vehicle` objects on the heap using `new`, demonstrates their use, and prints their state to reproduce the provided test cases (TC01..TC05). Include proper `delete` usage.
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.
