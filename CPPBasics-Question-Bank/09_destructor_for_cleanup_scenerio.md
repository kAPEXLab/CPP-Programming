# 09 - Destructor for Cleanup

## Introduction
Destructors perform cleanup for objects that own resources. This task ensures proper teardown for heap-allocated data and any acquired resources.

## Scenario
A vehicle object may allocate helper resources or open handles. Implement a destructor that safely releases any resources and prevents memory leaks when objects are destroyed.

## Tasks to Implement
1. Add a destructor to the Vehicle class.
2. Print a cleanup message when the object is destroyed.
3. Create an object in a block scope.
4. Verify that the destructor is called automatically.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | { Vehicle v("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); } | Vehicle object is being destroyed. |
| TC02 | { Vehicle v("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); } | Vehicle object is being destroyed. |
| TC03 | Vehicle* v = new Vehicle("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); delete v; | Vehicle object is being destroyed. |
| TC04 | { Vehicle v("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); } | Vehicle object is being destroyed. |
| TC05 | { Vehicle v("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); } | Vehicle object is being destroyed. |

## Suggested Validation Rules

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add a destructor that performs necessary cleanup and demonstrates its invocation).
- A short `main()` or test harness that creates and destroys `Vehicle` objects (stack and heap) to reproduce the provided test cases (TC01..TC05) and shows the destructor behavior.
- Validation evidence (program output or brief test log) showing the destructor messages appear as expected for each test case.
