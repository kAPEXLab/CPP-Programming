# 35 - Pure Virtual Function and Abstract Class

## Introduction
Abstract classes define interfaces and shared behavior while preventing direct instantiation. Pure virtual functions declare required derived behavior.

## Scenario
Design an abstract base `Vehicle` with at least one pure virtual method (e.g., `serviceChecklist()`) that derived vehicles must implement to provide type-specific checklists.

## Tasks to Implement
1. Declare a pure virtual function in Vehicle.
2. Implement displayInfo() in Car and Truck.
3. Use pointers or references to call the derived implementations.
4. Confirm that Vehicle itself cannot be instantiated.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* v = new Truck("DEF456","Ford","Transit",2021,70000.0f,false,'M',3.5); v->displayInfo(); | Truck make, model, and cargo capacity displayed. |
| TC02 | Vehicle* v = new Car("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); v->displayInfo(); | Car make, model, and year displayed. |
| TC03 | Vehicle* v = new Truck("B1","BMW","X5",2020,68000.0f,false,'A',3.0); v->displayInfo(); | Truck make, model, and cargo capacity displayed. |
| TC04 | Vehicle* v = new Car("T1","Tesla","Model 3",2024,12000.0f,true,'A',0.0); v->displayInfo(); | Car make, model, and year displayed. |
| TC05 | Vehicle* v = new Truck("A1","Audi","A4",2019,74000.0f,false,'M',2.0); v->displayInfo(); | Truck make, model, and cargo capacity displayed. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (declare a pure virtual method in `Vehicle`, implement it in derived classes, and demonstrate usage).
- A short `main()` or test harness that constructs derived objects and calls the implemented methods to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

