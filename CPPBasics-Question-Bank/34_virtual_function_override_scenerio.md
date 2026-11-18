# 34 - Virtual Function Override

## Introduction
Virtual functions allow derived classes to provide specialized behavior when accessed through base-type references. This question practices overrides.

## Scenario
Create a virtual `describe()` method in `Vehicle` and override it in derived classes to include type-specific details when called through base pointers or references.

## Tasks to Implement
1. Create a base class Vehicle with a virtual displayInfo() method.
2. Override the method in Car and Truck.
3. Use a base pointer to call derived implementations.
4. Verify polymorphic behavior.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* v = new Car("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); v->displayInfo(); | Car make, model, and year displayed. |
| TC02 | Vehicle* v = new Truck("DEF456","Ford","Transit",2021,70000.0f,false,'M',3.5); v->displayInfo(); | Truck make, model, and cargo capacity displayed. |
| TC03 | Vehicle* v = new Car("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); v->displayInfo(); | Car make, model, and year displayed. |
| TC04 | Vehicle* v = new Truck("T1","Mahindra","Bolero",2021,61000.0f,false,'M',1.9); v->displayInfo(); | Truck make, model, and cargo capacity displayed. |
| TC05 | Vehicle* v = new Car("A1","Audi","A4",2019,74000.0f,false,'M',2.0); v->displayInfo(); | Car make, model, and year displayed. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add virtual method(s), override in derived classes, and demonstrate polymorphic calls).
- A short `main()` or test harness that constructs derived objects via base pointers and calls the virtual method to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

